# PR Explorer · Änderungslogbuch V2.4.2

## V2.4.2 · 2026-05-31 · Clean Release und Cache-Fix

- `index.html` ist jetzt die aktive Startdatei und verweist eindeutig auf `app-claude-v242.js` und `style-claude-v242.css`.
- `service-worker.js` verwendet den neuen Cache `pr-explorer-claude-v2-4-2`.
- Der OSM-Hiking-Loader speichert keine 0-Linien-Antwort mehr als gültigen Cache.
- Bei fehlenden verwertbaren OSM-Geometrien wird eine Fehlermeldung angezeigt.
- Alte Versionsdateien sind nicht Bestandteil dieses Release-Pakets.
