# PR Explorer · Änderungslogbuch V2.4.3

## V2.4.3 · 2026-05-31 · Hiking-Modus und Farbmodus

- Die bisherigen zwei freien Schalter „Waymarked Trails Raster“ und „OSM Hiking Vektor“ wurden aus der normalen Ebenenliste herausgenommen.
- Neue eindeutige Auswahl „Hiking-Darstellung“:
  - Aus
  - Raster-Referenz
  - Editierbare Linien
  - Vergleich
- Altzustände mit gleichzeitig aktivem Raster und Vektor werden automatisch auf „Editierbare Linien“ migriert, damit die unbeabsichtigte Doppeloptik verschwindet.
- Der Vergleichsmodus bleibt bewusst verfügbar, wenn Raster- und Vektordaten gegeneinander geprüft werden sollen.
- Für OSM-Hiking-Vektorlinien wurde ein Farbmodus ergänzt:
  - Einheitlich
  - OSM-Farbe
  - Netzwerk
- Standard für editierbare Linien: einheitliche Madeira-grüne Darstellung mit Konturlinie.
- Service-Worker-Cache auf `pr-explorer-claude-v2-4-3` erhöht.
