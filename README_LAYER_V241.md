# PR Explorer · Layer-Integration V2.4.1

## Fix gegenüber V2.4

Die Overpass-Abfrage wurde robuster gebaut. Statt nur `out tags geom` direkt auf Relationen zu verwenden, lädt V2.4.1 zuerst die Hiking-/Foot-Routenrelationen und danach rekursiv deren Way-Geometrien:

```overpass
[out:json][timeout:120];
rel["type"="route"]["route"~"^(hiking|foot)$"](32.55,-17.35,32.95,-16.55);
out body;
way(r);
out tags geom;
```

Der Parser ordnet die Way-Geometrien anschließend wieder den jeweiligen Relationen zu. Dadurch wird der Fehler vermieden, dass ein erfolgreicher Overpass-Abruf als „0 Linien“ gespeichert wird, obwohl Relationen vorhanden sind.

## Bedienung

1. App/PWA nach Upload komplett neu laden.
2. Einstellungen → OSM Hiking Vektorlinien.
3. „OSM-Rohdaten laden / aktualisieren“ antippen.
4. Danach „OSM Hiking Vektor“ als Ebene aktivieren.

Cache-Key: `prHikingVectorGeojsonV241`. Leere V2.4-Caches werden nicht weiterverwendet.
