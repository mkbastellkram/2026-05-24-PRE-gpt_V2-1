# PR Explorer · Layer-Integration V2.4

## Neue Ebene

**OSM Hiking Vektor** lädt die Wander-/Fußrouten für Madeira direkt aus OpenStreetMap über Overpass und rendert sie als editierbare Leaflet-Vektorlinien.

## Rohdaten-Abfrage

```overpass
[out:json][timeout:120];
(
  relation["type"="route"]["route"~"^(hiking|foot)$"](32.55,-17.35,32.95,-16.55);
);
out tags geom;
```

## Einstellbare Darstellung

- OSM Hiking Vektor ein/aus
- Labels ein/aus
- Linienstärke
- Deckkraft
- Fallback-Farbe
- Konturlinie: Auto / Weiß / Schwarz / Aus

## Hinweis

Die Daten werden beim ersten Aktivieren/Laden per Overpass abgerufen und im lokalen Browser-Speicher zwischengespeichert. Externe Overpass-Server können zeitweise langsam oder nicht erreichbar sein. Der bisherige Waymarked-Trails-Rasterlayer bleibt als Fallback vorhanden.
