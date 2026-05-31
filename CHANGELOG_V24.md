# PR Explorer · Änderungslogbuch

## V2.4 · 2026-05-31 · OSM-Hiking als editierbarer Vektorlayer

- Zusätzliche Ebene „OSM Hiking Vektor“ ergänzt.
- Rohdatenquelle: OpenStreetMap-Routenrelationen per Overpass-Abfrage (`route=hiking` und `route=foot`) für den Madeira-Bereich.
- Darstellung als echte Leaflet-Vektorlinien statt PNG-Tile-Overlay.
- Separate Konturlinie ergänzt: Auto / Weiß / Schwarz / Aus.
- Einstellbar: Linienstärke, Deckkraft, Fallback-Farbe und Labels.
- Deutsche Linien-Info per Popup: Bezeichnung, Referenz, Routentyp, Netzwerk, Betreiber, OSM-Symbol, Quelle und OSM-Relation.
- Bestehender Waymarked-Trails-Rasterlayer bleibt als Vergleichs-/Fallback-Layer erhalten.

## V2.3 · 2026-05-31 · Kartenansichten und freie Overlays

- Kartenansichten auf OSM Standard, OpenTopoMap und Satellit reduziert.
- Freie Zusatzebenen Waymarked Trails Hiking und OpenSeaMap Seezeichen ergänzt.
