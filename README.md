# World of Witcher

**Online svet pre Zaklínača 3: Divoký hon.** Život v Skellige spolu s ďalšími hráčmi: remeslá, questy, obchod, domy a spoločné dobrodružstvá.

> Neoficiálny, bezplatný fanúšikovský mód. Nie je spojený s CD PROJEKT RED.
> Hra je zatiaľ **iba pre pozvaných hráčov**: na prihlásenie potrebuješ pozvánku (e-mail a osobný kód).

## ⬇️ Stiahnuť

### [**Stiahnuť WOW-Setup.zip**](https://github.com/janban-netizen/world-of-witcher/releases/latest/download/WOW-Setup.zip)

Všetky verzie: [Releases](https://github.com/janban-netizen/world-of-witcher/releases)

## Čo potrebuješ

- **Zaklínač 3: Divoký hon** (Steam alebo GOG), aktuálna verzia, spúšťaná v **DirectX 12**
- Windows 10 alebo 11
- **Pozvánku** od správcu servera (e-mail + osobný kód)
- Asi 1 GB voľného miesta a internet

## Inštalácia

1. Stiahni **WOW-Setup.zip**, rozbaľ ho a spusti **WOW-Setup.exe**.
2. Inštalátor sám nájde Zaklínača 3. Ak nie, klikni na **Change…** a vyber priečinok hry.
3. Klikni na **INSTALL**. Na konci nechaj zaškrtnuté *Start World of Witcher now* a klikni na **FINISH**.
4. V launcheri zadaj **e-mail a kód** z pozvánky a klikni na **PLAY**.
   Launcher overí prístup, stiahne hru (asi 1 GB, prvýkrát pár minút) a spustí ju.
   Pri ďalších spusteniach sťahuje iba novinky.
5. V hlavnom menu hry vyber **Play World of Witcher**.

Odinštalovanie: *Nastavenia Windows → Aplikácie → World of Witcher → Odinštalovať*.
Všetko sa presunie do zálohy `WOW_zaloha_<dátum>` v priečinku hry, základná hra ostane nedotknutá.

## Antivírus a Windows hlásia varovanie. Prečo?

World of Witcher je malý komunitný projekt a jeho programy **nie sú digitálne podpísané** (certifikát stojí stovky eur ročne).
Antivírusy preto nové súbory najprv preverujú. Nie je to nález vírusu.

- **Windows: „Windows ochránil váš počítač“** → klikni na *Ďalšie informácie* → *Spustiť aj tak*.
- **Chrome: „Tento súbor sa bežne nesťahuje“** → v zozname stiahnutí klikni na *Ponechať*.
- **AVG / Avast: „CyberCapture – na toto sa musíme pozrieť podrobnejšie“** → súbor poslali na kontrolu do laboratória.
  Počkaj (zvyčajne do pár hodín), alebo zvoľ *Ďalšie možnosti* → spustiť. Po kontrole ho antivírus pustí všetkým.
- Ak antivírus súbor presunul do karantény: obnov ho a pridaj výnimku pre priečinok hry
  (napr. `...\steamapps\common\The Witcher 3`).

### Čo jednotlivé súbory robia

| Súbor | Čo robí |
|---|---|
| `WOW-Setup.exe` | Inštalátor: nájde hru, nainštaluje launcher, vytvorí odkazy a záznam na odinštalovanie. |
| `WOWOnlineLauncher.exe` | Launcher: prihlásenie (e-mail + kód), stiahnutie a aktualizácia súborov módu, spustenie hry. |
| `WOWOnline.asi` | Sieťová časť módu, ktorú hra načíta (pripojenie k serveru, ostatní hráči). |
| `WitcherNativeBridge.asi` | Open-source most (MIT) medzi skriptami hry a natívnym kódom. |
| `dinput8.dll` | [Ultimate ASI Loader](https://github.com/ThirteenAG/Ultimate-ASI-Loader) (MIT), štandardný spôsob, ako hra načíta módy `.asi`. |

Nič z toho nezbiera osobné údaje a nemení nič mimo priečinka hry, okrem odkazov na ploche a v ponuke Štart.
Mód sa sťahuje iba z nášho servera a iba s platnou pozvánkou.

### Kontrolné súčty (SHA-256)

Overíš ich v PowerShelli: `Get-FileHash .\WOW-Setup.exe`

| Súbor | SHA-256 |
|---|---|
| WOW-Setup.exe (v1.0.0) | `884f43c84e73b5cac8cf47459b2f953e0c3138e27f12656b8769c4d6911d187d` |

---

### English

**World of Witcher** is a free, unofficial online fan modification for *The Witcher 3: Wild Hunt* (not affiliated with CD PROJEKT RED).
Playing requires an invitation (e-mail + personal code).
[Download WOW-Setup.zip](https://github.com/janban-netizen/world-of-witcher/releases/latest/download/WOW-Setup.zip), unzip, run `WOW-Setup.exe`, then sign in in the launcher.
The programs are not code-signed, so Windows SmartScreen or antivirus tools (AVG/Avast CyberCapture) may hold them for a check first. This is a reputation check for new files, not a malware detection.
