# Finansų harmonija V22

2026-11-13 užfiksuota testavimo versija (šaltinių žyma `v22`). Įtraukti visi dabartiniai V22 pakeitimai. Tolesnis tobulinimas atliekamas tik atskiroje V23 versijoje; V22 ir ankstesni leidimai nekeičiami.

V22 testavimas: https://albertborkovski-cmd.github.io/finansu-harmonija-v22/

## Paleidimas

```bash
npm ci
npm run dev
```

V22 vietinis adresas: http://127.0.0.1:5203/. Tolesnės V23 versijos adresas: http://127.0.0.1:5204/. Vietiniai duomenys laikomi atskirai ir nepublikuojami.

## Leidimo turinys

Įtraukta visa dabartinė programa: dokumentai ir sąskaitų kūrimas, bankas, kasa, sandėlis, sudengimas, BŽ ir susietų dokumentų redagavimas, OCR darbuotojo / TeamLead eiga ir mokymo taisyklės, administravimas bei lietuvių ir anglų kalbų perjungimas.

GitHub saugykloje publikuojama sukompiliuota svetainė ir tikslus `source-v22.zip` archyvas, `source-manifest.json` bei `release.json` su SHA-256 ir patikrų rezultatais. Vietinė šaltinių Git istorija nepakeičia GitHub artefaktų istorijos. V21 ir ankstesnės publikacijos nekeičiamos.

## Demonstracinis prisijungimas

- Vidinis administratorius: `albertborkvski@gmail.com`.
- Išorinis naudotojas: `aurika.z@meso.lt`.
- Slaptažodžio laukas prototipe tikrina formatą: bent 6 simboliai, didžioji raidė ir specialus simbolis. Naudokite išgalvotą testinę reikšmę, ne tikrą slaptažodį.

Tai demonstracinis prototipas, ne produkcinė apskaitos sistema. GitHub Pages neturi saugaus serverinio autentifikavimo, bendros duomenų bazės, tikro OCR, banko, apskaitos sistemos ar el. laiškų siuntimo API. Mokėjimai išsaugomi kaip juodraščiai, ne siunčiami į banką. Connect bank išsaugo teikėjo pasirinkimą, tačiau nepradeda banko autorizacijos ir nepakeičia būsenos į Connected. Demonstracinės prijungimo būsenos nėra tikras banko ryšys.

Vietiniai `.env`, `.meso-shared-data.json`, `node_modules` ir kiti privatūs darbo failai nepublikuojami. Nenaudokite konfidencialių dokumentų ar tikrų slaptažodžių. To paties GitHub Pages domeno leidimai gali dalytis naršyklės saugykla; izoliuotam testavimui naudokite atskirą naršyklės profilį.

## Patikros

TypeScript patikra, leidimo kompiliavimas ir tiksliniai banko / mokėjimų / DK priskyrimo testai tikrinami prieš publikavimą. Pilno testų rinkinio rezultatai ir žinomi senesnių testinių pakaitalų neatitikimai dokumentuojami `release.json`; nesėkmingi testai nelaikomi praėjusiais.
