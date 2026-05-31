# PR Explorer · V2.4.2 Clean Release

Diese Version bereinigt die vorherige V2.4/V2.4.1-Mischlage.

## Aktive Dateien

Diese Dateien gehören direkt ins Root-Verzeichnis von GitHub Pages:

- `index.html`
- `app-claude-v242.js`
- `style-claude-v242.css`
- `service-worker.js`

Die vorhandenen Dateien `pr-data.js`, `manifest.webmanifest` und Icons bleiben bestehen.

## Wichtig

GitHub Pages startet `index.html`. Deshalb enthält dieses Paket keine `index-v242.html`, sondern direkt die aktive `index.html`.

Der Service Worker verwendet einen neuen Cache `pr-explorer-claude-v2-4-2`, damit alte V2.4-/V2.4.1-Dateien nicht weiter ausgeliefert werden.

## OSM Hiking Vektor

Der Loader speichert keine 0-Linien-Antwort mehr als gültigen Cache. Falls Overpass Daten liefert, aber keine verwertbaren Geometrien gefunden werden, erscheint eine klare Fehlermeldung statt eines scheinbar erfolgreichen 0-Linien-Status.
