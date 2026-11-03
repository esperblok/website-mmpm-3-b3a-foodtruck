# POFEERTJESHUYS — website foodtruck

Donkere, glow-y one-page website voor de poffertjesfoodtruck **POFEERTJESHUYS** (project `mmpm-3-b3a-foodtruck`).
Visueel en interactief in dezelfde stijl als [esperblok.github.io](https://esperblok.github.io): zwarte achtergrond,
neon-gloed, glitch-titels, particles, 3D-tilt-kaarten en een loader — maar dan in het cosmic-palet van de eigen logo
(paus `#9b30ff`, neon-roze `#ff2ea6`, boter-goud `#ffc25e`).

## Live bekijken

De site is puur statisch: `index.html` bevat HTML, CSS én JavaScript in één bestand (net als de referentiesite).

```bash
# lokaal
python3 -m http.server 8000
# open http://localhost:8000
```

Of publiceer via GitHub Pages: **Settings → Pages → Branch: `main` / folder `/ (root)`** — de site draait dan op
`https://esperblok.github.io/website-mmpm-3-b3a-foodtruck/`.

## Bestanden

| Bestand | Wat |
| --- | --- |
| `index.html` | De hele website (styling + interacties in één bestand) |
| `flyer.html` | Promotie-flyer 1080×1920, voor- én achterzijde, print-klaar |
| `images/` | Logo, productfoto's, hero-beeld en QR-code (gegenereerd voor dit project) |
| `.nojekyll` | Zet Jekyll-verwerking uit zodat `_`-bestanden en mappen intact blijven op Pages |

## Wat zit erin

- **Intro-loader** met pulserend logo en laadbalk, **cursor-glow** en een **particle-canvas** met onderling verbindende lijnen.
- **Hero** met zoomende achtergrond, glitch-titel `POFEERTJESHUYS`, zwevend logo, **live countdown naar de eerstvolgende standplaats**, klik-om-te-kopiëren infobalk en share-knoppen.
- **Menu** als filterbare timeline (Klassiek / Deluxe / Vegan & Vrij / Dranken / Extra's) — klik een gerecht open voor het verhaal, zet het daarna **in het mandje**.
- **Mandje & bestellen**: live bedragen, plus/min per regel, ophaaltijd kiezen, bestel-modal met QR-code, "nog X porties vandaag"-schaarste. Het mandje blijft bewaard (`localStorage`).
- **Standplaatsen**: zes agendakaarten met datum, plek, tijden en status (live / gepland / volgeboekt), klikbaar naar Google Maps.
- **Inhuren**: drie pakketkaarten met 3D-tilt **plus een prijsbereker** (pakket, aantal gasten, uren, opties) met live totaal en aanvraag-modal.
- **Locatie** met donker gekleurde kaartembed, **galerij** met lightbox (pijltjes/Escape), **dieetwensen**-checklist met voortgangsbalk (ook opgeslagen), **FAQ**-accordeon, nieuwsbrief, toasts, back-to-top.
- **Verborgen details**: 5× op het footer-logo klikken, en de Konami-code. 🥞

## Tekst & cijfers

Alle data (agenda, prijzen, pakketprijzen, KVK) zijn voorbeeldwaarden voor de oplevering van het schoolproject. Vervang ze door echte waarden;
de agenda staat bovenin het `<script>`-blok van `index.html` in de constante `STOPS`.
