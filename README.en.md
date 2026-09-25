<div align="center">

<img src="docs/logo.svg" width="88" alt="DotaAccept logo">

# DotaAccept

**Fewer clicks. More game.**

Accept a match and pick your hero using hotkeys or Telegram.

![Windows](https://img.shields.io/badge/Windows-10%20%2F%2011%20x64-ffdb4d?style=flat-square&labelColor=171717)
![Version](https://img.shields.io/badge/version-2.0-ffdb4d?style=flat-square&labelColor=171717)
![Interface](https://img.shields.io/badge/UI-Russian-ffdb4d?style=flat-square&labelColor=171717)

[Русский](README.md) · **English**

[**Download for Windows**](https://github.com/wuttashi1/DotaAccept/releases/latest) · [Quick start](#quick-start) · [Screenshots](#screenshots) · [Report an issue](https://github.com/wuttashi1/DotaAccept/issues)

<img src="docs/screenshots/home.png" alt="DotaAccept home: match acceptance and hero pick sequences" width="100%">

</div>

## Your match. One touch away.

DotaAccept is a Windows app that runs configured actions for accepting a match and selecting a hero in Dota 2. Capture a button position or record a click sequence, then trigger it using a hotkey or your own Telegram bot.

- **Match acceptance** — a dedicated action triggered with F6.
- **Hero profiles** — save click sequences and run the selected profile with F7.
- **Telegram control** — connect your bot and manage which users can access it.
- **Action settings** — click recording, a step editor, capture countdown and mouse movement modes.
- **System tray** — hide the window, enable Windows startup and start the bot with the app.
- **Execution controls** — an activity log, F8 to stop and F9 to enable or pause.

> This repository distributes a ready-to-run build and documentation. It does not contain the application's full source code. The app interface is in Russian; documentation is available in Russian and English.

## Quick start

1. Download **DotaAccept-2.0-Windows-x64.zip** from the [latest release](https://github.com/wuttashi1/DotaAccept/releases/latest).
2. Extract the **entire archive** into a separate folder. Keep `DotaAccept.exe` next to the `_internal` folder.
3. Run `DotaAccept.exe`. You do not need to install Python.
4. On the home page, choose **«Указать кнопку»** (Capture button) in the match acceptance card, or **«Настроить принятие»** (Set up acceptance) if no action is configured yet.
5. Switch to Dota 2, point at the desired button and wait for the capture sound. The countdown can be set to 3, 5 or 8 seconds.
6. Press **F6** to run the action. To configure a hero pick, create a profile, choose **«Записать клики»** (Record clicks), perform your sequence and press **F8** to finish recording. Press **F7** to run the selected profile.

**Requirements:** Windows 10/11 x64 and Microsoft Edge WebView2 Runtime. Actions triggered from the app window allow 3 seconds to switch to the game.

Actions use recorded positions and click sequences. Check and re-record them when the game's resolution or layout changes. Acceptance is triggered by the user; automatic match detection is not advertised here.

## Hotkeys

- **F6** — accept a match.
- **F7** — run the selected hero sequence.
- **F8** — stop an action / finish recording clicks.
- **F9** — enable or pause the app; this binding can be changed in settings.

You can also move the mouse to the upper-left corner of the screen to stop an action. Hotkeys can be enabled in settings.

## Telegram setup

1. Create a bot using **@BotFather** in Telegram and obtain its token.
2. Open **Telegram**, paste the token and enable the connection.
3. Send `/start`, then `/id` to your bot to get your user ID.
4. Add your ID or `@username` under **«Доступ к управлению»** (Access control).

The token and personal settings are stored locally in `config.json`. Do not publish or share that file. The download does not include the author's personal configuration. Telegram details in the screenshots are examples; use your own bot.

## Screenshots

### Telegram — connection and access

<img src="docs/screenshots/telegram.png" alt="Telegram bot connection and access management" width="100%">

### Settings — make it yours

<img src="docs/screenshots/settings.png" alt="Capture countdown, mouse movement, hotkeys and startup settings" width="100%">

### Activity log — see what happened

<img src="docs/screenshots/history.png" alt="Application activity log" width="100%">

## System tray and settings migration

Closing the window hides it in the system tray. Choose **«Выход»** (Exit) to quit completely. Launching the app again restores its window from the tray.

To migrate settings, close both copies of the app and copy your `config.json` next to the new EXE. Toggle Windows startup off and back on if you previously used it. Keep configuration backups private: they may contain your bot token.

## Feedback

Open an [Issue](https://github.com/wuttashi1/DotaAccept/issues) with a description, your Windows version and steps to reproduce. Remove tokens and personal information from screenshots and logs before sharing them.

---

<div align="center">

**DotaAccept · Ready when you are.**

An unofficial project, not affiliated with Valve. Dota 2 is a trademark of Valve Corporation.

</div>
