# PR Explorer · Änderungslogbuch

## V2.4.1 · 2026-05-31 · OSM-Hiking Loader-Fix

- Overpass-Abfrage von direktem Relations-`out tags geom` auf robuste Relation-plus-Way-Abfrage umgestellt.
- Parser ordnet separat geladene Way-Geometrien den OSM-Relationen zu.
- Neuer Cache-Key `prHikingVectorGeojsonV241`, damit ein alter 0-Linien-Cache nicht weiter genutzt wird.
- Statusanzeige bleibt erhalten, aber die Datenbasis ist zuverlässiger.

## V2.4 · 2026-05-31 · OSM-Hiking als Vektorlayer

- Zusätzliche Ebene „OSM Hiking Vektor“.
- Editierbare Leaflet-Vektorlinien mit Kontur, Farbe, Deckkraft, Linienstärke und deutschen Popups.
