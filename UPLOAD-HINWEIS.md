# Upload-Hinweis V2.4.3

Diese Dateien im GitHub-Hauptverzeichnis hochladen bzw. ersetzen:

- `index.html`
- `app-claude-v243.js`
- `style-claude-v243.css`
- `service-worker.js`

Bestehende Dateien weiterhin behalten:

- `pr-data.js`
- `manifest.webmanifest`
- `icon-180.png`
- `icon-192.png`
- `icon-512.png`

Alte Versionsdateien wie `app-claude-v242.js`, `style-claude-v242.css`, `CHANGELOG_V242.md`, `README_LAYER_V242.md` können später gelöscht oder in einen Archivordner verschoben werden. Für den Betrieb von V2.4.3 werden sie nicht mehr benötigt.

Nach dem Upload auf dem iPhone die PWA/Safari vollständig neu laden. Der Service-Worker nutzt den neuen Cache `pr-explorer-claude-v2-4-3`.
