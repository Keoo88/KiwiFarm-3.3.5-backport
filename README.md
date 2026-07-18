# KiwiFarm - WotLK 3.3.5 backport

<p align="center">
  <img src="https://github.com/user-attachments/assets/701c53e2-71ca-4fc8-8044-048bb3f525a3" alt="KiwiFarm icon" width="64" height="64"/>
</p>

<p align="center">
  <b>Gold &amp; loot tracker with instance-reset timer for World of Warcraft 3.3.5a (WotLK).</b>
</p>

<p align="center">
  <a href="#features">Features</a> ·
  <a href="#installation">Installation</a> ·
  <a href="#usage">Usage</a> ·
  <a href="#license">License</a>
</p>

---

## About

**KiwiFarm** tracks gold and items looted during farming sessions, estimates their value, and monitors instance resets to stay within the 5 per hour limit.

This is a **backport of KiwiFarm to WoW 3.3.5a (WotLK)**.

## Features

- 💰 **Gold/hour tracking** - live earnings, session totals, per-zone stats.
- 📜 **Loot log** - every item recorded with estimated value.
- ⏱ **Instance reset timer** - time until next reset, resets left this hour.
- 🔄 **One-click instance reset** - reset all dungeons from the main window.
- 🏷 **Price sources** - pulls prices from Auctionator when installed.
- 📦 **Movable, lockable window** with minimap button (LibDBIcon).
- 🌍 **Localized** via AceLocale-3.0.

## Installation

1. Download the latest release (or clone this repository).
2. Extract the archive.
3. Move the KiwiFarm folder into:
   `
   \Interface\AddOns\
   `
4. Make sure the folder is named exactly KiwiFarm with KiwiFarm.toc at root.
5. Restart the game (or /reload) and enable KiwiFarm in the addon list.

## Usage

| Command | Action |
| --- | --- |
| /kfarm or /kiwifarm | Toggle the main window |

| Input | Action |
| --- | --- |
| **Left-click + drag** | Move the main window |
| **Shift + Left-click** | Reset all instances |
| **Right-click** | Open configuration menu |

## License

Released under the [LICENSE](LICENSE) file.

## Credits

- Original addon: **michaelsp**
- WotLK 3.3.5 backport: **Keoo**
- Discord: https://discord.gg/sKpJbUrsvR
- Libraries: LibStub, CallbackHandler-1.0, LibDataBroker-1.1, LibDBIcon-1.0, AceLocale-3.0
