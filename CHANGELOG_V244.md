# PR Explorer · Änderungslogbuch V2.4.4

## V2.4.4 · 2026-06-01 · Teststabilisierung, Linien-Casing und Kalenderfelder

- Funktionstest als stabilere Vollhöhen-Ansicht umgesetzt.
- Wisch-Schließen des Hauptpanels im Testmodus deaktiviert, damit Scrollen nicht versehentlich den Test beendet.
- Testnotizen werden sofort bei Eingabe in `localStorage` gespeichert und bleiben versionsübergreifend erhalten.
- Teststatus `Anmerkung` ergänzt; Schaltfläche blau umrandet.
- Je Testfeld wurde ein `Leeren`-Button für die jeweilige Notiz ergänzt.
- GPX-Grundeinstellung: `#FF3B30`, Stärke 5 px, durchgezogen, weißes Casing.
- KML-Grundeinstellung: `#007AFF`, Stärke 5 px, durchgezogen, weißes Casing.
- KML-Anfahrten werden bei großen Geometriesprüngen getrennt, um unerwünschte Luftlinien zu vermeiden.
- Detailseiten erhalten Terminplanung mit `Geplanter Termin` und `IFCN gebucht`, jeweils mit 30-Minuten-Raster.
- IFCN-gebuchte Termine setzen den Status auf `Gebucht` und können als `.ics` mit Erinnerungen 1 Tag und 3 Stunden vorher exportiert werden.
- Reise-Tab zeigt eine zentrale Kalenderliste aus geplanten und gebuchten PR-Terminen.
- Bottom-Navigation und Test-Pill wurden näher an die iOS-Safe-Area geschoben.
