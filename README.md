# World of Witcher

**An online world for The Witcher 3: Wild Hunt.** Live a life in Skellige together with other players: trades and crafts, quests, trading, houses and shared adventures.

> A free, unofficial fan modification. Not affiliated with CD PROJEKT RED.
> The world is currently **invitation only**: you need an invitation (e-mail + personal code) to sign in.

## ⬇️ Download

### [**Download WOW-Setup.zip**](https://github.com/janban-netizen/world-of-witcher/releases/latest/download/WOW-Setup.zip)

All versions: [Releases](https://github.com/janban-netizen/world-of-witcher/releases)

## Requirements

- **The Witcher 3: Wild Hunt** (Steam or GOG), current version, running in **DirectX 12**
- Windows 10 or 11
- An **invitation** from the server admin (e-mail + personal code)
- About 1 GB of free disk space and an internet connection

## Installation

1. Download **WOW-Setup.zip**, unzip it and run **WOW-Setup.exe**.
2. The installer finds The Witcher 3 on its own. If it does not, click **Change…** and choose the game folder.
3. Click **INSTALL**. At the end, leave *Start World of Witcher now* checked and click **FINISH**.
4. In the launcher, enter the **e-mail and code** from your invitation and click **PLAY**.
   The launcher checks your access, downloads the game files (about 1 GB, a few minutes the first time) and starts the game.
   After that it only downloads what is new.
5. In the game's main menu, choose **Play World of Witcher**.

## Is World of Witcher safe?

World of Witcher is made by one person as a **free fan project** for The Witcher 3. We sell nothing, we do not collect your data, and you do not pay to play. Below we explain openly what the installer does, why your antivirus may warn you, and how you can check everything yourself.

### Why your antivirus or Windows may show a warning

Larger companies buy a **digital signature** for their programs. It costs hundreds of euros a year, which is too much for a free community project for now. Without a signature, Windows and antivirus programs do not know a new file yet, so they check it first. **This is not a virus detection.** It is a check of an unknown file.

What you may see:

- **Windows: "Windows protected your PC"** → *More info* → *Run anyway*.
- **Chrome: "This file isn't commonly downloaded"** → in the downloads list, choose *Keep*.
- **AVG / Avast: "CyberCapture"** → the file was sent to their lab for a check. Once it is cleared, it is allowed for every player. You can wait, or choose *More options* to run it right away.
- If your antivirus moved a file to quarantine: restore it and add an exception for the game folder
  (for example `...\steamapps\common\The Witcher 3`).

Online game mods need their own program that connects to a server. Antivirus tools check such programs more strictly, so these warnings are common for them.

### What the installer does

- finds your copy of The Witcher 3 (Steam or GOG),
- installs the launcher into the game folder (the newest launcher from this page over HTTPS; if that cannot be reached, the copy inside the installer),
- creates a desktop shortcut (only if you want one) and a Start menu entry,
- adds World of Witcher to the list of installed apps in Windows, so you can uninstall it the normal way.

The mod itself (about 1 GB) is downloaded by the launcher only after you sign in with the e-mail and code from your invitation. **Without a valid invitation, nothing is downloaded.**

### What we do NOT do

- we do not collect personal data or passwords,
- we do not change anything outside the game folder (apart from the desktop and Start menu shortcuts),
- we do not install any other programs, ads or browser add-ons,
- nothing runs in the background while you are not playing.

### What each file does

| File | What it does |
|---|---|
| `WOW-Setup.exe` | The installer: finds the game, installs the launcher, creates the shortcuts and the uninstall entry. |
| `WOWOnlineLauncher.exe` | The launcher: sign-in (e-mail + code), downloads and updates the mod files, starts the game. |
| `WOWOnline.asi` | The mod's network part loaded by the game (connection to the server, other players). |
| `WitcherNativeBridge.asi` | An open-source bridge (MIT) between the game's scripts and native code. |
| `dinput8.dll` | [Ultimate ASI Loader](https://github.com/ThirteenAG/Ultimate-ASI-Loader) (MIT), the standard way the game loads `.asi` mods. |

### How to check it yourself

- **Download only from this page.** Do not use copies from anywhere else.
- **See the [VirusTotal page for WOW-Setup.exe](https://www.virustotal.com/gui/file/2fb5d9e7b3ebc92bdd894d11fef0adb1caaa1e42cece29b7208c41c1559afebc)**, where about 70 antivirus engines check it at once
  (if the page says the file is unknown, upload your downloaded copy there). For version 1.0.0, 67 of 70 found nothing, including AVG, Avast, Bitdefender, Avira and ClamAV.
  The three flags are typical for new, unsigned programs: Bkav Pro (flags most unknown programs), McAfee Scanner
  (`Ti!…` means "not seen before", based on the file's checksum) and Trapmine (a machine-learning guess, not a specific finding).
- **Verify the checksum.** In PowerShell, run `Get-FileHash .\WOW-Setup.exe` and compare the result:

| File | SHA-256 |
|---|---|
| WOW-Setup.exe (v1.0.1) | `2fb5d9e7b3ebc92bdd894d11fef0adb1caaa1e42cece29b7208c41c1559afebc` |
| WOWOnlineLauncher.exe (v1.0.1, downloaded by the installer) | `f41124ef828d2ec77772bace49dda320ae004c72ff6df4d3fc78a0d30a425cee` |

If it matches, you have exactly our file and nobody has changed it.

## Uninstalling

*Windows Settings → Apps → World of Witcher → Uninstall.*
Everything is moved into a backup folder (`WOW_zaloha_<date>`) inside the game folder. Your copy of The Witcher 3 and your saved games stay untouched.

## Questions or concerns?

Open an [issue on GitHub](https://github.com/janban-netizen/world-of-witcher/issues). We are happy to explain anything.

---

*World of Witcher is an unofficial fan modification and is not affiliated with CD PROJEKT RED. The Witcher 3 is a trademark of CD PROJEKT S.A.*
