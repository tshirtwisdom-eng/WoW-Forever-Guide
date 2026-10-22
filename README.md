<p align="center"><img src="docs/images/icon.png" width="96" alt="WoW Forever Guide icon"></p>

# WoW Forever Guide

Horde leveling guides for **World of Warcraft: Forever**, one per class, levels 1–60, with a live link that keeps the guide in step with the character you're playing. Created by UMJ.

![The guide following a level 22 Shadow Priest](docs/images/overview.png)

**[Download the latest installer](https://github.com/tshirtwisdom-eng/WoW-Forever-Guide/releases/latest)** (Windows 10/11, `WoW-Forever-Guide-<version>.msi`)

---

## Install

1. Download the `.msi` from [Releases](https://github.com/tshirtwisdom-eng/WoW-Forever-Guide/releases/latest) and run it.
   The installer isn't code-signed yet, so Windows may say *"Windows protected your PC"*: click **More info → Run anyway**.
2. Choose where to install (default: `Documents\WoW Forever Guide`). No admin rights are needed.
3. Check the game folder. Setup looks for WoW Forever on your drives; if it shows the wrong folder, click **Browse** (the standard location is `C:\Program Files (x86)\World of Warcraft`).
4. **Start with Windows** is off unless you tick it.
5. Finish with *Open WoW Forever Guide now* ticked.

**What the installer does:** copies the guides and the app into the folder you chose, adds Start menu and desktop shortcuts, and remembers your game folder. That's all. The app installs the in-game addon the first time it runs, and again after every update so the two always match.

**Uninstall** (Settings › Apps) removes everything: the install folder including your saved characters, the shortcuts, the addon in your game folder, and the startup entry if you turned it on.

## Using the guide

Start **WoW Forever Guide** from the Start menu. It opens the class index in your browser and sits in the tray next to the clock.

![Class index](docs/images/index.png)

- **Log into a character** and its class guide opens by itself. Each character keeps its own progress. A character you haven't played before is added the first time you log in.
- **Leveling route:** each chapter is a list of quest steps. Steps tick themselves off as you complete quests in game, and the next step is always at the top. Quests tagged *Worth it* are especially good; *Skip unless you need the XP* ones can be left out.
- **Character & Inventory:** your gear, bags, bank and stats as the game reports them, with the upgrades worth chasing at your level. Quest items name their quest, and ones whose quest isn't in your quest log are marked red so you know they're probably safe to delete.
- **Quests:** open any quest for where to pick it up, where its mobs and items are on the map, what drops the quest items, who takes it back, and what to do first.
- **Dungeons:** the Prep tab lists every quest for the dungeon (and the ones you need first) with numbered pickup pins; the Bosses tab shows boss portraits on the map, with a gold **!** on bosses that drop something you still need. Click a boss for its drops.
- **Mounts:** riding at 40 and 60 for your race, where to train and buy, and every mount you can collect.
- **Talents & abilities:** the talent calculator matches the in-game trees. Hover a talent to see what it does and, if it gives an ability, its cost, range and cooldown before you spend the point. Below it are your full spellbook (every rank, by level) and ready-to-copy macros.
- **Equipment:** besides the upgrades list, it names the random green suffixes worth looking for, like *…of the Owl* for casters.
- **Professions, maps, flight paths, reputations** are all in the left menu, filtered to your class.
- Offline, a guide opens on the character of that class you played last. Pick another one in the **CHARACTER** box at the top.

| Leveling route | Character & inventory |
|---|---|
| ![Leveling route](docs/images/route.png) | ![Character and inventory](docs/images/character.png) |

## The tray app

The book icon next to the clock is the live link. Hover over it to see who's in game. Click it to open the guide. Right-click for:

- **Open characters folder**: one file per character, so you can back them up or delete them.
- **Show log**: what the app is doing, for when something doesn't work.
- **Tablet & phone access…**: opens a page on your PC to turn it on (off by default). Scan the QR code with your tablet or phone and type the 4-digit code shown on the PC; the device then gets the full live guide on your home network. Remove paired devices on the same page. If Windows asks, allow the app on private networks only.
- **Check for updates**
- **Start with Windows**: off unless you turn it on.
- **Quit**

## The in-game addon

**WoW Forever Guide Live Link** (folder `WoWForeverGuide`) is installed for you. It adds a book button on the minimap: click it for the sync window, **Alt+click** to open the guide, right-click for settings (also under *Esc › Options › AddOns*).

Useful commands: `/wfg` (sync window), `/wfg open` (open the guide), `/wfg panel` (in-game panel), `/wfg options`, `/wfg live` (live stream on/off), `/wfg help`.

### The in-game panel (optional)

A small panel in the game with your next quest steps from the class guide and reminders you would otherwise miss: new class spells, a profession rank to train, riding at 40 and 60. It is **off until you type `/wfg panel`**.

![The in-game panel and its settings](docs/images/ingame-panel.png)

- Each line says what to do and where; quests in progress show the objective and where the mobs or items are.
- **Click** a line to put a pin on your map (TomTom if you have it). **x** skips a quest or dismisses a reminder; `/wfg panel restore` brings them back.
- **Drag** it anywhere (or lock it). The title bar collapses it, opens its settings, or hides it.
- **Settings** (`/wfg panel settings`, or the cog): size, width, text size, background opacity, number of steps, what it shows, hide in combat or in dungeons.

### Why is there a pixel strip?

WoW addons can't send anything out of the game: no internet, no files. Their saved data only reaches the disk when you `/reload` or log out. To keep the guide live anyway, the addon draws a **small coded strip of colored pixels in the bottom-left corner** of the game window. The app reads that strip, and only that 256×10-pixel corner of the WoW window, a few times a second. It carries your position, level and XP, plus your quests, gear, bags, talents and professions, sent in small pieces as they change.

- It hides itself during combat.
- Play in **Windowed** or **Windowed (Fullscreen)** mode, and don't cover the bottom-left corner of the game.
- Don't want it? Type `/wfg live` to turn it off. The guide then updates when you `/reload` or log out.

## Updates

The app checks this page for new releases. When there's one, the guide shows a small dialog with the release notes. Click **Install now** and the app downloads the installer, checks it against the published checksum, installs it, and restarts. The open guide page reloads itself into the new version. **Later** hides the dialog until your next session.

![Update dialog](docs/images/update.png)

## Good to know

- **Horde only.** Alliance characters are never saved, and the guide will kindly suggest you roll Horde.
- Nothing about your characters is uploaded anywhere. Everything stays in your install folder and your browser.
- The guides work without the app too. Open `WoW Forever Guide.html` in the install folder; you just won't get live updates.
- Game data comes from [ForeverDB](https://foreverdb.net). Fan-made: not affiliated with or endorsed by Blizzard Entertainment. World of Warcraft is a trademark of Blizzard Entertainment.

---

Created by UMJ.
