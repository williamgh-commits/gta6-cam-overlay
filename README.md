# connieheinz cam overlay

Et gennemsigtigt overlay til kameraet i OBS: en animeret kant i GTA VI-farver, et lille GTA VI-logo i et hjørne og navnet nederst.

## Filer

- `connieheinz-cam-overlay.html` – selve overlayet (logoet er indlejret).
- `config.js` – navn, logo-hjørne, animationshastighed og kantens tykkelse.

Hold begge filer i samme mappe.

## Brug i OBS

1. Tilføj en **Browser**-kilde med **Lokal fil**, og vælg HTML-filen.
2. Sæt bredden og højden til **præcis samme størrelse som kamera-kilden**. Overlayet fylder hele kilden og skalerer med, så kanten rammer kameraet. Forholdet er ca. 1,74:1, fx 1920×1103.
3. Læg browser-kilden oven på kameraet.

Skriften hentes fra Google Fonts, så computeren skal have internet.

## Indstillinger (`config.js`)

| Indstilling | Standard | Beskrivelse |
|---|---|---|
| `name` | `connieheinz` | Navnet nederst |
| `logo` | `true` | Vis GTA VI-logoet |
| `logoCorner` | `tl` | `tl`, `tr`, `bl` eller `br` |
| `speed` | `7` | Sekunder pr. omgang for kanten |
| `borderWidth` | `1.5` | Kantens tykkelse i % af bredden |

Parametre efter filnavnet overstyrer config, fx `?navn=connieheinz&logo=off`.

## Ophavsret

GTA VI-logoet tilhører Rockstar Games / Take-Two Interactive. Projektet er et fan-projekt og ikke tilknyttet Rockstar.
