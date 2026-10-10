# Visubase – kattintható demó

Gyártáskövető platform (gépek, munkalapok, felhasználók) kattintható demója. Élőben: a repó GitHub Pages címén (`index.html`).

Egyetlen HTML-fájl, böngészőben megnyitva fut (internet csak a betűtípusokhoz kell). Minden adat szimulált mintaadat; a demó ideje 1 mp = 1 perc.

## Mit lehet kipróbálni

- **Iroda → Gépek:** két gép (Citizen L20 – Camshaft, Citizen L20 – Needle) élő adatokkal: üzemállapot, gyártási teljesítmény az elvárthoz képest (db/óra), áramfelvétel (A), teljesítményfelvétel (kW), fogyasztás (kWh), hibanapló.
- **Iroda → Munkalapok:** munkalap-böngésző szűrővel és kereséssel, **Import (JSON)** gombbal. A `minta-munkalap-import.json` szándékosan tartalmaz hibás sorokat is (hiányzó határidő, már létező munkalap, szabály nélküli típus) – ezeket az import kihagyja.
- **Kész munkalap riportja:** `ML-2026-1041` (lezárt) – állásidők, teljesítmény az elvárthoz képest, fogyasztás, űrlapválaszok (egy tartományon kívüli méréssel), CSV-export. `ML-2026-1036` megszakított munkalap indoklással.
- **Gépterminál:** bejelentkezés → pending munkalap indítása a kezdő űrlappal → „Leállás szimulálása” / „Hiba szimulálása” → ok megadása → lezárás a befejező űrlappal → a riport megjelenik az irodában.

## Demóban rögzített értékek

| Gép | Elvárt teljesítmény | Állásidő-korlát |
|---|---|---|
| Citizen L20 – Camshaft | 42 db/óra | 180 s |
| Citizen L20 – Needle | 120 db/óra | 180 s |
