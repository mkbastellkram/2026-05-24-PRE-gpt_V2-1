# PR Explorer · V2.4.4 Hinweise

## Upload

Im GitHub-Hauptverzeichnis ersetzen/hochladen:

- `index.html`
- `app-claude-v244.js`
- `style-claude-v244.css`
- `service-worker.js`

Bestehende Dateien wie `pr-data.js`, `manifest.webmanifest` und die Icons bleiben erhalten.

## Testmodus

Der Funktionstest speichert Notizen sofort unter dem stabilen Schlüssel `prTestResults`. Notizen bleiben deshalb auch nach Versionswechseln erhalten. Der Button `Leeren` entfernt nur die Notiz des jeweiligen Testfeldes. `Zurücksetzen` löscht nur den Teststatus, nicht die Notizen.

## Linien

GPX: rot `#FF3B30`, 5 px, durchgezogen, weißes Casing.
KML: blau `#007AFF`, 5 px, durchgezogen, weißes Casing.

KML-Geometriesprünge über ca. 1,8 km werden getrennt, damit keine direkte Luftlinie zwischen zwei nicht zusammengehörenden Liniensegmenten gezeichnet wird.

## Termine / Kalender

Jede PR-Detailseite enthält:

- Geplanter Termin
- IFCN gebucht

Beide Felder verwenden `datetime-local` mit 30-Minuten-Raster. Beim IFCN-Termin wird der PR-Status auf `Gebucht` gesetzt. Der Button `Gebucht als iOS-Kalender` erzeugt eine `.ics`-Datei mit zwei Erinnerungen: 1 Tag vorher und 3 Stunden vorher.
