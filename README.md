# KiwiFarm — WotLK 3.3.5 backport

<p align="center">
  <img src="KiwiFarm.tga" alt="KiwiFarm icon" width="64" height="64"/>
</p>

<p align="center">
  <b>Gold &amp; loot tracker with instance-reset timer for World of Warcraft 3.3.5a (WotLK).</b>
</p>

<p align="center">
  <a href="#features">Features</a> ·
  <a href="#installation">Installation</a> ·
  <a href="#usage">Usage</a> ·
  <a href="#price-sources">Price sources</a> ·
  <a href="#license">License</a>
</p>

---

## About

**KiwiFarm** is a small movable window that tracks the gold and items you loot
during farming sessions and estimates their value using the price source you
choose. It also tracks instance resets and lockout timers, so you can stay
within the **5 resets per hour** limit and time your runs efficiently.

This repository is a **backport of the original KiwiFarm addon to WoW 3.3.5a
(WotLK 3.3.5 client)**. The retail/Classic version lives at the author's
upstream project.

## Features

- 💰 **Gold / hour tracking** — live earnings, session totals and per-zone stats.
- 📦 **Loot log** — every item you loot is recorded with its estimated value.
- ⏱ **Instance reset timer** — shows time until your next reset and how many
  resets are left in the current hour.
- 🔁 **One-click instance reset** — reset all dungeons straight from the main
  window.
- 🧩 **Price sources** — pulls item prices from **Auctionator** when installed.
- 🖱 **Movable, lockable window** with a minimap button (via LibDBIcon).
- 🌐 **Localized** via AceLocale-3.0.
- 🪶 Lightweight — no heavy dependencies beyond the bundled libs.

## Installation

1. Download the latest release (or clone this repository).
2. Extract / copy the `KiwiFarm` folder into:
   ```
   World of Warcraft\Interface\AddOns\KiwiFarm
   ```
3. Make sure the folder is named exactly `KiwiFarm` and contains
   `KiwiFarm.toc` at its root.
4. Restart the game (or `/reload`) and enable **KiwiFarm** in the addon list.

### Optional dependencies

| Addon | Purpose |
| --- | --- |
| [Auctionator](https://www.curseforge.com/wow/addons/auctionator) | Item price source |
| LibSharedMedia-3.0 | Extra fonts / textures |
| LibItemUpgradeInfo-1.0 | Better item info |

## Usage

### Slash commands

| Command | Action |
| --- | --- |
| `/kfarm` | Toggle the main window |
| `/kiwifarm` | Same as above |

### Mouse controls

| Input | Action |
| --- | --- |
| **Left-click + drag** | Move the main window |
| **Shift + Left-click** | Reset all instances |
| **Right-click** | Open the configuration menu |

From the configuration menu you can pick the price source, change fonts and
colors, toggle the minimap button, clear session data and more.

## Price sources

KiwiFarm currently supports:

- **Auctionator** — uses your local scan database for item valuations.

If no price source is available, items are still logged but valued at vendor
price only.

## Compatibility

- Built and tested on **WoW 3.3.5a** (Interface `30300`).
- Also runs on Vanilla / TBC clients with per-character reset tracking.

## License

Released under the terms of the [LICENSE](LICENSE) file in this repository.

## Credits

- Original addon: **Keoo**
- WotLK 3.3.5 backport: **Keoo**
- Libraries: LibStub, CallbackHandler-1.0, LibDataBroker-1.1, LibDBIcon-1.0,
  AceLocale-3.0.
