<div align="center">

# 👑 Roblox Account Manager+

### **Manage and run a bunch of Roblox accounts from one place.**
*Launch any account into any game, keep it alive while you're away, watch its resource usage, and skin the whole thing to look how you want.*

<p>
  <img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Windows">
  <img src="https://img.shields.io/badge/.NET%20Framework-4.7.2-512BD4?style=for-the-badge&logo=dotnet&logoColor=white" alt=".NET Framework 4.7.2">
  <img src="https://img.shields.io/github/v/release/Cynx21309/RobloxAccountManagerPlus?style=for-the-badge&label=Version&color=2ecc71" alt="Latest version">
  <img src="https://img.shields.io/badge/Status-Active-2ecc71?style=for-the-badge" alt="Active">
  <img src="https://img.shields.io/badge/Access-Public%20%2F%20Key%20Only-3498db?style=for-the-badge" alt="Public download, key only">
</p>

[✨ Features](#-features) • [📊 Comparison](#-ram-vs-the-original-vs-other-basic-managers) • [🔑 Getting a Key](#-getting-a-key) • [🚀 Getting Started](#-getting-started) • [🔒 Security](#-security-and-privacy) • [❓ FAQ](#-faq)

</div>

---

The download is **public**, but the app is **key only** — it won't open without a license key (see
[Getting a Key](#-getting-a-key)). It's not open source and isn't accepting outside contributions;
this README is here so anyone who gets a key knows what the app actually does. Every version is on the
[Releases](../../releases) page.

## ✨ Features

### Accounts
- Add, group, launch, and manage any number of Roblox accounts from one list
- Live Memory/CPU usage and an online-in-game status dot per running account
- Ctrl+K search box to filter the account list instantly
- Per-account description, alias, and display name editing
- Uptime shown as Xd Xh Xm Xs once an account's been running 24h+
- Account Generator (Add Account → Account Generator) — fills in Roblox's sign-up page and presses Sign Up while you solve each CAPTCHA by hand, then saves the new account with its password. Pick a username style (Name+No., Adj+Noun, GamerTag, Counting like `Name0001`, `Name0002`, or Custom), an automatic or custom password, a birth-year range, a delay range between accounts, retries, and up to 49 accounts. Made accounts are listed with Copy all and Save to file buttons
- Drag accounts into Account Control to manage them from a separate panel (and drag the cards into any order) — a card for every account with a round picture, its name and @username, an online/offline status and a check box, grouped like the main list

### Launching
- Launch into a Place ID, a specific server (job ID), or a private server/share link
- Tick several accounts to launch them one after another
- Saved game/server presets so you don't have to re-paste the same link every time
- Server browser with player counts, and a Follow-a-player option
- Restore Window Position — remembers each account's window position and size and puts it back exactly where it was on its next launch; an account with nothing saved yet gets centered on screen instead of landing wherever Roblox/Windows happens to put it

### Anti-AFK
- Its own sidebar section, reliable across every open window (not just the first one), with automatic retries
- Auto Reconnect — clicks through Roblox's own disconnect/rejoin dialog if a client gets kicked, jumping straight to the Rejoin button and only reacting to the real disconnect box
- Anti-AFK Statistics window — total AFK time, actions performed, last action, auto-reconnects, longest session, last-cycle success count, and a live "next cycle" countdown
- Optional "Always On Top" for the statistics window

### Alerts & Updates
- Discord alerts — paste your own webhook and get a message when an account disconnects or crashes (with its name, profile picture, how long it was open and its game), when the watchdog restarts a frozen window, or when Auto Relaunch reopens one; each can be switched off, with an optional ping
- Health watchdog (off by default) — a Roblox window that stops responding or uses no CPU for a set number of minutes is closed and reopened in the game it was last in
- Update question — when a newer version exists RAM+ asks Yes / No a few seconds after it starts; nothing is downloaded or installed without a yes

### Quality of Life
- Tools & Fixes — ghost process cleanup, memory trimming (manual or on an interval), and installer popup prevention (quarantines Roblox's bundled installer executables while the app is open)
- Window Tools — tile/resize every open Roblox window below its own normal minimum size, drag-assist for shrunk windows, auto-mute Roblox audio, force low graphics, and window position/size restore
- Logs & Diagnostics — auto-clean old Roblox logs, remove outdated Roblox version folders, clean up Roblox's own crash dumps
- Misc — Discord Rich Presence while the app is open (account count, total RAM/CPU, elapsed time)
- Global FPS cap, or a per-account override set independently for any account, editing Roblox's own settings file directly (not a FastFlag, so it isn't affected by Roblox's FastFlag allowlist)
- Optional RAM/CPU/Time overlay on each Roblox window, positioned over its own top bar

### OpenMultiBoxing+
- Built-in multiboxing, in its own sidebar entry ("OMB") — assign each account a fixed slot and its Roblox window is moved there as soon as it opens, in any launch order, instead of depending on whatever order windows happened to appear in
- Grid layout automatically picks the columns/rows closest to the chosen monitor's own shape for however many accounts are slotted — matched against old OpenMultiBoxing's own grid calculator across every count from 1 to 32 so it lays out exactly the same way; up to 49 slots are supported, and when a crowded monitor can't hold that many windows at a readable size they keep a minimum size and overlap instead of shrinking away
- Click a monitor on the built-in map to arrange windows on it; multi-monitor setups can hide the monitors they're not using from the map, with one-click Hide others / Show all buttons; each monitor shows a small number badge so they're never ambiguous
- A "Use all shown monitors" tick box spreads the windows over every monitor shown in the Show: row, shared out by screen size — hide the 4th monitor and they spread over the other 3, and so on down to one
- Drag a square on the map onto another to swap the two accounts' slots
- Type a slot number that's already taken to insert there — everyone from that slot on shifts down one; an Exclude checkbox per account dims it, clears its slot, and closes the gap for everyone after it, without deleting the account
- A slider numbers the first N accounts (in the same order as the main list) 1, 2, 3... in one drag, with a divider between groups so a multi-group account list stays readable
- Snap into slot on launch — on by default; an account's window moves into its slot the moment it's detected running, no need to press Arrange yourself. Toggleable per setup if you'd rather arrange manually
- Click an account name or its slot on the map to bring that window to the front; double-click to pop it back out to a normal window (its original frame, size, and position restored exactly) instead of staying locked in the grid. Arrange Running Windows / Unarrange Running Windows buttons do the same for every running window at once
- Optional fullscreen mode (clicking an account fills its monitor), borderless windows, and the Ctrl+Shift+C hotkey to arrange every running account into its slot
- Its own window, independent of the main one, so it keeps running when the main window is minimized

### Theming
- Full Theme Editor — colors, borders, and backgrounds for every part of the UI
- Optional custom background image (cover-fit, see-through sidebar/labels)
- Match Colors — auto-recolor the whole theme from a background image's dominant hue, with Unmatch to revert
- Optional animated RGB border on the main window
- Accounts list transparency slider
- Theme changes apply instantly across every open window, not just the main one
- Smooth, non-laggy window resizing/dragging even with a custom background image set

### Utilities
- Browse Games (keyword search or trending), Servers, Favorites, and Universe info
- Private Server Manager — resizable, properly anchored list of saved private servers
- Account Control — multi-account browser-style panel with presence indicators (green dot when actually in-game)
- Account Utilities — change display name, avatar, block/unblock a player, send a friend request, per account

### Remote Dashboard
- A website built into RAM+: open it from your phone or another PC on any network, with no router setup (a free private tunnel), protected by a password you choose
- Live tiles for every account, stat cards, and a graph of how many accounts were running over time
- Launch or close one account, a whole group, or everything (always with an "Are you sure?" step), and pick a game or private server preset for each group
- Switches for Anti-AFK, Auto-Reconnect, Ghost Cleanup, Memory Trim, and Auto Relaunch
- Accent colors, light/dark mode, and backgrounds you can change

## 📊 RAM+ vs. the Original vs. Other Basic Managers

RAM+ started as a fork of the original Roblox Account Manager and kept building from there. The **RAM+** and
**Original RAM** columns are based on each project's own README, not a
full code audit of either. **Other Basic Managers** is a generic stand-in for the bare-bones alt managers floating
around — add/launch accounts and not much else. Not a knock on the original — it's a solid base and still actively
maintained — just what's different here.

<!-- Badge cells render as colored pills inside the table on GitHub -->
[yes]: https://img.shields.io/badge/-Yes-2ecc71?style=flat-square
[no]: https://img.shields.io/badge/-No-e74c3c?style=flat-square

<div align="center">

| Feature | 👑 **RAM+** | 🐺 **Original RAM** | 📦 **Other Basic Managers** |
|---|:---:|:---:|:---:|
| Add, launch, and manage multiple accounts | ![Yes][yes] | ![Yes][yes] | ![Yes][yes] |
| Cookie import (bulk, one per line) | ![Yes][yes] | ![Yes][yes] | ![Yes][yes] |
| Bulk import via username:password | ![Yes][yes] | ![Yes][yes] | ![No][no] |
| Drag-to-sort accounts | ![Yes][yes] | ![Yes][yes] | ![No][no] |
| Account grouping | ![Yes][yes] | ![Yes][yes] | ![No][no] |
| **Custom group ordering** (type any name) | ![Yes][yes] | ![No][no] — needs `1Main`, `007 Bank`-style prefixes | ![No][no] |
| **Live Memory/CPU per account** | ![Yes][yes] | ![No][no] | ![No][no] |
| **Online-in-game status dot** | ![Yes][yes] | ![No][no] | ![No][no] |
| **Ctrl+K account search** | ![Yes][yes] | ![No][no] | ![No][no] |
| **Per-account window position/size restore** | ![Yes][yes] | ![No][no] | ![No][no] |
| **Built-in multiboxing grid (OpenMultiBoxing+)** | ![Yes][yes] | ![No][no] | ![No][no] — usually needs a separate third-party tool |
| Launch into a Place ID / server / VIP link | ![Yes][yes] | ![Yes][yes] | ![Yes][yes] |
| Saved game/server presets | ![Yes][yes] | ![Yes][yes] | ![No][no] |
| Server browser with player counts | ![Yes][yes] | ![Yes][yes] | ![No][no] |
| **Lowest Ping Server** — one-click preset | ![Yes][yes] | ![No][no] — manual, sort the server list yourself | ![No][no] |
| Shuffle JobId | ![Yes][yes] | ![Yes][yes] | ![No][no] |
| **Anti-AFK** (keeps a session alive while idle) | ![Yes][yes] | ![No][no] — not in their feature list | ![No][no] |
| Reconnect/relaunch after getting kicked | ![Yes][yes] — clicks through the rejoin dialog directly | ![Yes][yes] — "Auto Relaunch," closes and reopens the whole client instead | ![No][no] |
| **Anti-AFK Statistics window** | ![Yes][yes] | ![No][no] | ![No][no] |
| FPS unlock | ![Yes][yes] | ![No][no] — documented, but doesn't actually work | ![No][no] |
| **Per-account FPS override** | ![Yes][yes] | ![No][no] — global only | ![No][no] |
| **Discord Rich Presence** | ![Yes][yes] | ![No][no] | ![No][no] |
| Local HTTP API | ![Yes][yes] | ![Yes][yes] | ![No][no] |
| **Per-account RAM/CPU/time overlay** | ![Yes][yes] | ![No][no] | ![No][no] |
| **Ghost process cleanup / memory trimming** | ![Yes][yes] | ![No][no] | ![No][no] |
| Theme editor | ![Yes][yes] | ![Yes][yes] — basic, "not much I can do about it with WinForms" by their own README | ![No][no] |
| **Auto-recolor from a background image** | ![Yes][yes] | ![No][no] | ![No][no] |
| **Animated RGB window border** | ![Yes][yes] | ![No][no] | ![No][no] |
| **Smooth resizing with a background image set** | ![Yes][yes] | ![No][no] | ![No][no] |

</div>

## 🔑 Getting a Key

Release builds require a key before the app opens at all. Keys are issued by the owner and bound to one device the first time they're used — make a ticket in the Discord server if you don't have one: https://discord.gg/5ErzTB4qvP

Once activated, the title bar shows how much time is left on your key.

## 🚀 Getting Started

1. Get the exe and a license key (see above).
2. Run it, enter your key, and choose **Add account**.

### Adding an account

- **Browser** (recommended) opens Roblox's own login page in a real, separate browser window. Sign in as usual — captchas and 2-step verification just work, and your password never passes through the app.
- **Password** signs in through Roblox's login service directly (`user:pass`, one per line for bulk adds). Quick, but if Roblox throws a captcha at it you'll need Browser instead.
- **Cookie** takes a `.ROBLOSECURITY` value you already have — paste one per line to bulk-import.

### Launching

Select an account, paste a Place ID or game link, and press **Launch**. Add a server ID or a private server link to join a specific server.

### Updating

RAM+ checks for a newer version a few seconds after it starts and asks **Yes / No** — nothing is downloaded or installed without a yes. You can also press **Check for updates** in Settings → General. Updating downloads the new version from this page, checks it, replaces the exe, and restarts — your key, settings, and accounts are left alone. (Versions older than 1.0.2 need one manual update: download the newest zip from [Releases](../../releases) and replace the exe.)

## 🔒 Security and Privacy

Session cookies are the keys to your accounts, so the app treats them that way.

- Encrypted at rest, password-protected on first run.
- No telemetry, no external server. The app talks to Roblox's own API, to GitHub for the app's own updates, and to Discord only if a webhook is configured (for release announcements, or for the alerts you set up yourself). The optional Remote Dashboard uses a free private tunnel, and only while you have it turned on.
- Access is key-gated, and every key is bound to one device.

## ❓ FAQ

**Where do my cookies go?**
Nowhere but your own disk, encrypted, and Roblox's official endpoints when the app checks a session or launches a game — the same as your browser does.

**Can I run more than one Roblox client at once?**
Yes, that's the whole point — launch as many accounts as you want side by side.

**Is there an auto-updater?**
Yes. RAM+ checks for a newer version a few seconds after it starts and offers to install it for you. You can also press **Check for updates** in Settings → General. Versions older than 1.0.2 need one manual update first: download the newest zip from [Releases](../../releases) and replace the exe.

**Does this break Roblox's Terms of Service?**
The app does what you could do by hand in a browser: sign in and launch games, through official endpoints. Automation features (Anti-AFK, etc.) are a grey area, so use them responsibly and at your own risk.

---

<div align="center">

*Not affiliated with Roblox Corporation. You are responsible for your own accounts.*

</div>
