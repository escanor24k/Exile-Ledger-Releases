<div align="center">

# Exile Ledger

**Trade companion & wealth tracker overlay for Path of Exile 1**

Price check items, handle trade whispers with one click and keep track of what your trades actually earn, without ever leaving the game.

`Version 0.2.0` · `Windows 10 / 11` · `Path of Exile 1`

</div>

---

## Download

**[⬇ Download the latest version](https://github.com/escanor24k/Exile-Ledger-Releases/releases/latest)**

| File | Description |
|---|---|
| `ExileLedger-Setup.exe` | Installer: start menu & desktop shortcut, optional start with Windows. No admin rights needed. |
| `ExileLedger-Portable.exe` | Portable version: no installation, just run it. |

Once running, Exile Ledger keeps itself up to date automatically.

---

## What is Exile Ledger?

Exile Ledger is a desktop app that sits on top of Path of Exile 1 as an overlay. It combines two things players usually need separate tools for:

- **Trading in the game**: price checks, trade search and handling incoming and outgoing trade whispers.
- **Keeping track of your wealth**: a trade log and farming sessions with profit per hour, with net-worth tracking as the next step (see [Roadmap](#roadmap)).

Everything happens in a dark, Path-of-Exile-inspired interface. The app, its overlays and its installer all use their own design instead of the standard Windows look.

### Who is it for?

- **Traders** who sell a lot and want to invite, trade and thank buyers without typing commands.
- **Buyers** who want to price check items and whisper sellers straight from the game.
- **Farmers** who want to know which content is actually worth their time.

> Exile Ledger is for **Path of Exile 1** only. Path of Exile 2 is not supported.

### Pricing

All current features can be used at no cost. Additional or extended features may be offered as part of a paid plan or subscription in the future.

---

## Features

### Trade overlay
When someone whispers you from the official trade site, a trade card appears at the top right of your game window.

- **Selling:** Invite · Trade · Kick → Thanks · quick replies (*Busy*, *Sold*, *Still interested?*)
- **Buying:** Visit hideout · Trade · Thanks → Leave party
- Shows item, price, league and the buyer's note.
- A small stash grid on the card shows the exact stash position of the requested item.
- Shows when the player has entered your area.
- Repeated requests are grouped instead of piling up.
- Follow-up messages from the same player appear on the card.
- Optional sound for new sale requests.
- Completed trades are kept in a trade history.

### Stash highlight
Find sold items instantly. One click on the stash button of a trade card (or a hotkey) marks the requested item's cell directly over your stash in game, shows the stash tab name in large letters and types the item name into the stash search, so the game highlights it as well.

- Works with normal and quad stash tabs.
- One-time calibration in *Settings → Overlay*: drag and resize a frame onto your stash grid so it matches your resolution and UI scale.
- Exile Ledger does not switch stash tabs for you. That would require several inputs per key press, which GGG's rules do not allow.

### Price check
Hover an item in game and press **Ctrl+D**. A price panel opens directly over the game.

- **Quick price from poe.ninja**: value in Chaos and Divine, 7-day trend and number of listings. Covers currency, fragments, scarabs, essences, divination cards, uniques (incl. 5/6-link), gems and maps.
- **Trade search** using the official trade site:
  - Item mods are matched automatically, including mod tiers (T1, T2, …).
  - Totals for life and resistances are calculated for you.
  - The strongest mods of rare items are pre-selected. Every filter and minimum value can be adjusted.
- **Results:**
  - Lowest price, median price and online status of each seller.
  - **Whisper button** for every listing. The purchase then shows up in the trade overlay automatically.
- Open the same search on the trade website with one click.

### Sessions
Find out which farming strategy really pays off. Start a session, name your strategy (e.g. *Essence*, *Expedition*, *Harbinger*) and play as usual.

- **Maps are tracked automatically:** every new map instance counts as a run, with its tier and the time spent inside it. Trips to your hideout are not counted as map time.
- **Deaths** are counted per session and per map.
- **Profit** is calculated from your completed trades during the session, converted with current poe.ninja prices. You can add manual income or expenses, e.g. a bulk sale outside of whispers.
- **Profit per hour**, average map time and session time, live while you play.
- **Strategy comparison:** all sessions grouped by strategy, ranked by profit per hour.
- **Session HUD:** a small bar at the top of the game window shows session time, current map and profit per hour. It does not react to clicks, so it never gets in your way.
- Pause and resume at any time. An unfinished session survives an app restart.

### Hotkeys
Every action can be bound to one or more key combinations (e.g. `Ctrl+D` *and* `Alt+Q`).

| Action | Default |
|---|---|
| Price check item under cursor | `Ctrl+D` |
| Go to own hideout | `F5` |
| Open main window | – |
| Show / hide trade overlay | – |
| Leave party | – |
| Invite / kick / thank newest buyer | – |
| Show requested item in stash | – |
| Dismiss newest request | – |
| Start / end session · pause / resume session | – |
| Visit seller's hideout · send trade request | – |

Hotkeys are only active while Path of Exile is in the foreground, so the same keys keep working normally in every other program.

### Languages
English (default), Deutsch, Français, Español, Português (BR) and Русский. Switch at any time in the settings. The choice is remembered.

### Automatic updates
Exile Ledger checks for new versions on start and every 6 hours. When an update is available, a notice appears in the app. One click downloads it and restarts the app.

- Every update is digitally signed. The app only installs updates whose signature matches, so a tampered file is rejected.
- Works for both the installed and the portable version. Your settings and trade history are kept.
- Automatic checks can be turned off in *Settings → General → Updates*. You can still check manually there.

---

## Fair play

Exile Ledger is built to follow GGG's [third-party tool policy](https://www.pathofexile.com/developer/docs):

- **One action per key press or click.** Every button and hotkey sends at most one chat command. Multi-step actions such as *Kick → Thanks* are split into separate clicks on purpose.
- **No memory reading, no packet sniffing and no automation of gameplay.**
- Item data comes from the game's own copy function (`Ctrl+Alt+C`). Trade whispers and zone changes are read from the game's log file `Client.txt`.
- The official trade API is used within GGG's rate limits. The app slows itself down before a limit is reached.

---

## Requirements

- Windows 10 or 11 (64-bit)
- Microsoft Edge WebView2. It is preinstalled on Windows 11 and up-to-date Windows 10. If it is missing, the installer and the portable version offer to install it automatically (internet connection required).
- Path of Exile 1 with the **English** game client
- Game display mode **Windowed** or **Windowed Fullscreen**. Overlays cannot be drawn over exclusive fullscreen.

---

## Installation

Download the latest version from the **[release page](https://github.com/escanor24k/Exile-Ledger-Releases/releases/latest)**. There are two versions. Use whichever you prefer:

| | Setup | Portable |
|---|---|---|
| File | `ExileLedger-Setup.exe` | `ExileLedger-Portable.exe` |
| Installation | Yes, for your Windows user only (no admin rights) | No, just run the file |
| Start menu & desktop shortcut | ✓ | – |
| Start with Windows (optional) | ✓ | – |
| Listed in *Apps & features* | ✓ | – |

The installer asks for your language first, and the app then starts in that language.

> **Windows SmartScreen:** the app is not code-signed yet, so Windows may show a warning on first start. Click *More info* → *Run anyway*.

---

## Getting started

1. **Start Exile Ledger.** It lives in the system tray. Closing the window keeps it running in the background.
2. **Settings → General:**
   - Pick your language.
   - Enter your **character name**. It is needed for *Leave party*.
   - `Client.txt` is detected automatically while the game is running. If not, enter its path manually (usually `…\Path of Exile\logs\Client.txt`).
3. **Settings → Price Check:** the league is selected automatically (current challenge league). You can also pick one.
4. **Settings → Hotkeys:** adjust the key bindings if you like.
5. Start Path of Exile in windowed or windowed fullscreen mode, and you are ready.

Want to see it before playing? Use **Test: Sale** / **Test: Purchase** on the *Trades* page to create example trades, and the example items on the *Price Check* page.

---

## Usage

### Selling
1. A buyer whispers you, and a card appears in the overlay.
2. Press the **stash button** to find the item, then **Invite** → the buyer arrives (the card shows *Here*) → **Trade**.
3. After the trade: **Kick**, then **Thanks**. The trade moves to your history.

### Farming sessions
1. Open **Sessions**, enter a strategy and press **Start session** (or use a hotkey).
2. Play as usual. Maps, time, deaths and trades are tracked automatically, and the HUD shows your progress in game.
3. Press **End session** when you are done. The session appears in the strategy comparison.

### Buying
1. Price check an item with `Ctrl+D` and run a **Search**, or whisper a seller from the trade website.
2. Press the whisper button next to a listing. The purchase appears in the overlay.
3. **Hideout** → **Trade** → **Thanks** → **Leave**.

---

## Data & privacy

- Settings and trade history are stored **locally** on your PC in `%APPDATA%\de.exileledger.app`.
- The app contacts only:
  - **poe.ninja**, for quick prices
  - **pathofexile.com**, for the official trade search and league list
  - **github.com**, to check for and download updates
- No account login is needed for the current features, and no data is sent anywhere else.
- When uninstalling, you can choose to keep or remove your settings and trade history.

---

## Troubleshooting

| Problem | Solution |
|---|---|
| Overlay does not appear | Set the game to *Windowed* or *Windowed Fullscreen*. Check that the overlay is enabled in *Settings → Overlay*. |
| Trades are not detected | Check that *Log connected* is shown in the title bar. Otherwise set the path to `Client.txt` in the settings. |
| Price check does nothing | Hover the item before pressing the hotkey. Only the English game client is supported. |
| "Trade API temporarily unavailable" | GGG's trade site is under maintenance (e.g. around league launches). Try again later. |
| "Rate limit reached" | Wait the shown number of seconds. The app protects you from being temporarily locked out by the trade site. |
| *Leave* button is disabled | Enter your character name in *Settings → General*. |
| Stash highlight is in the wrong place | Open your stash and use *Settings → Overlay → Calibrate*. |

---

## Roadmap

- [x] Trade overlay with one-click trade actions
- [x] Price check overlay (poe.ninja + official trade search)
- [x] Configurable hotkeys
- [x] Six languages
- [x] Automatic, signed updates
- [x] Sessions: maps, time per map and profit per hour, compared per strategy, with in-game HUD
- [x] Stash highlight with stash search
- [ ] **Wealth**: stash snapshots and net-worth history (waiting for GGG's OAuth approval)
- [ ] Support for non-English game clients

---

## License

Exile Ledger is proprietary software. All rights reserved. You may download and use the official releases for personal use. Copying, modifying or redistributing the software or its source code requires permission. See [LICENSE](LICENSE) for details.

## Disclaimer

Exile Ledger is a fan-made tool. It is not affiliated with or endorsed by Grinding Gear Games. *Path of Exile* is a trademark of Grinding Gear Games.
