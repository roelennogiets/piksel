# Colour Pixel — Android-project

De game werkt offline als Android-app via een ingebouwde WebView. De swipe-selector gebruikt de absolute positie van de vinger/muis in het kleurvlak.

## APK maken zonder Android Studio (via GitHub Actions)

1. Maak op GitHub een nieuw, leeg repository aan.
2. Pak deze ZIP uit en upload alle bestanden en mappen naar dat repository (inclusief de verborgen map `.github`).
3. Open in GitHub het tabblad **Actions**.
4. Kies **Build Android APK** en druk op **Run workflow** (of wacht tot de automatische build klaar is na upload naar `main`).
5. Open de geslaagde workflow-run. Onderaan bij **Artifacts** download je `ColourPixel-debug-apk`.
6. Pak die artifact-ZIP uit. Daarin staat `app-debug.apk`.
7. Zet de APK op je Android-toestel en open hem. Android kan vragen om installatie vanuit die bron toe te staan.

Dit is een debug-APK om zelf te installeren en testen, geen Play Store-release.

## Gamebediening
- Horizontaal slepen: saturatie (links minder, rechts meer).
- Verticaal slepen: hue (boven/onder verandert de kleurtoon).
- 10 seconden per pixel.
- De muis/vingerpositie wordt rechtstreeks naar de kleurpositie vertaald.
