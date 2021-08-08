---
home: true
heroImage: /dortania-logo-clear.png
heroText: Dortania OpenCore Telepítési Útmutatója
actionText: Előkészületek →
actionLink: prerequisites.md

meta:
- name: description
  content: "Jelenleg támogatott verzió: 0.7.2"
---
#### _**Megjegyzés:**_ Ez az útmutató egy nem hivatalos fordítása az angol [Dortania Guide](https://dortania.github.io/OpenCore-Install-Guide)-nak. Ha bármit nem értesz, akkor azért elnézést, nehéz mindent értelmesen lefordítani, ilyen esetben keresd ki az angol fordításban, hátha ott jobban érthető.
# Mi az az OpenCore és kinek lett 
kitalálva?

Az OpenCore egy úgynevezett "boot loader" –  egy komplex szoftver ami előkészíti a gépet az operációs rendszer betöltésére – pontosabban a feladata az, hogy új adatot szolgáltasson a macOS számára, mint például SMBIOS, ACPI táblák és kext-ek. Amiben ez az eszköz különbözik a többi megoldástól, az az, hogy az OpenCore a biztonságra és a minőségre lett tervezve az alapoktól, ezzel lehetővé teszi nekünk olyan biztonsági beállítások használatát mint a [System Integrity Protection](https://support.apple.com/en-ca/HT204899) és a [FileVault](https://support.apple.com/en-ca/HT204837). Mélyebben ebben a cikkben tudsz róla olvasni: [Miért az OpenCore mindenek felett](why-oc.md)

Ez az útmutató két fő dologra fókuszál:

* macOS telepítése X86 alapú számítógépeken
* Elmagyarázni neked, mi teszi műkdő képessé a Hackintosh-od.

Emiatt készülj fel, hogy sokat fogsz olvasni, tanulni és Google-n keresni. Ez nem egy két kattintásos telepítés lesz.

Kérlek tartsd szem előtt, hogy az OpenCore még mindig egy új fejlesztésnek számít és még bétában van. Ez nem azt jelenti, hogy nem stabil, sőt szinte minden szempontban sokkal stabilabb, mint más megoldások, mint például a Clover, ezen kívül még mindig aktívan fejlesztés alatt áll, szóval a konfigurációs fájl elég gyakran változik is (pl. új beállítások jönnek régiek helyére).
Ha bármilyen problémád akad, akkor keress rá a [Hibaelhárítási oldalon](/troubleshooting/troubleshooting.md), ha nem találsz semmi hozzákapcsolódót, akkor kérj segítséget az [r/Hackintosh subreddit](https://www.reddit.com/r/hackintosh/)-en vagy az [r/Hackintosh Discord](https://discord.gg/u8V7N5C) szerveren.