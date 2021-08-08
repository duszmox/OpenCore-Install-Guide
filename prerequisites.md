# Első lépések az OpenCore-al

Mielőtt belekezdenénk az OpenCore-os rendszer felépítésébe, át kell nézni pár dolgot. 

## Előfeltételek

1. <span style="color:red">_**[FONTOS]**_</span> Idő és türelem.
   * Ne kezdj bele ebbe, ha nincs sok szabadidőd vagy határidőkkel dolgozol. A Hackintosh-olt számítógép nem egy munkára használható eszköz, a rendszer nem elég stabil és megbízható, ezt tartsd észben.
2. <span style="color:red">_**[FONTOS]**_</span> **ISMERD A HARVERED**
   * A processzorod nevét és generációját
   * A videókártyád
   * A tárolóeszközeid (HDD/SSD, NVMe/AHCI/RAID/IDE konfiguráció)
   * A laptopod/asztali géped modelljét, ha előre öszzeállított gépről van szó
   * Az **Ethernet chipset-ed**
   * A WLAN/Bluetooth chipset-ed
3. <span style="color:red">_**[FONTOS]**_</span> **EGY ALAPTUDÁS A PARACSSORHOZ ÉS, HOGY HOGYAN KELL HASZNÁLNI A TERMINÁLT**
   * Ez nem csak <span style="color:red">_**[FONTOS]**_</span>, ez az egész útmutató alapja. Nem tudunk segíteni akkor ha egy alap `cd` paranccsal se tudsz belépni egy mappába.
4. <span style="color:red">_**[FONTOS]**_</span> Egy számítógép ami megfelel a _**Kompatibilitási**_ oldalon leírtaknak.
   * [Hardver limitációk oldal](macos-limits.md)
5. <span style="color:red">_**[FONTOS]**_</span> Egy minimum:
   * 16GB pendrive, ha macOS-en szeretnéd elkészíteni a telepítőt
   * 4GB pendrive, ha Windows-on vagy Linux-on szeretnéd elkészíteni a telepítőt
6. <span style="color:red">_**[FONTOS]**_</span> Egy **Vezetékes Internetkapcsolat** és tudnod is kell a LAN kártyád modelljét.
   * Rendelkezned kell egy fizikai LAN porttal, vagy egy macOS-el kompatibilis adapterrel. Ha van egy [kompatibilis WiFi kártyád](https://duszmox.github.io/Wireless-Buyers-Guide/), akkor azt is használhatod.
     * Megjegyzés: A wifi kártyák nagy része nem, vagy nem teljesen kompatibilis a macOS-el.
   * Ha nincs vezetékes internetkapcsolatod, de rendelkezel egy Androidos mobiltelefonnal, akkor csatlakoztathatod azt is wifihez és tovább oszthatod annak a jelét USB-n keresztül a [HoRNDIS](https://joshuawise.com/horndis#available_versions) segítségével.
7. <span style="color:red">_**[FONTOS]**_</span> **Egy megfelelő operációs rendszerre:**
   * Be it:
     * macOS (egy viszonylag újabb jobb lenne)
     * Windows (Windows 10, 1703 vagy újabb)
     * Linux (Egy tiszta, megfelelően működő rendszer, Python 2.7 vagy újabbal rajta)
   * Windows vagy Linux felhasználóknak, **15GB** szabad tárhelyre a lemezen amin dolgozol. Windows-on, az Operációs rendszered lemezén (C:) rendelkezned kell **15GB** szabad tárhellyel.
   * macOS felhasználóknak, **30GB** szabad táhelyre a lemezen.
   * A legtöbb terminál eszköz ami ebben az útmutatóban van használva igényeli a [Python](https://www.python.org/downloads/)-t.