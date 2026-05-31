# PR Explorer · Layer-Integration V2.4.3

## Ziel der Änderung

Die Hiking-Ebenen werden nicht mehr als zwei unabhängige Schalter dargestellt. Dadurch soll die unbeabsichtigte Doppeloptik aus Raster-Layer und Vektor-Layer vermieden werden.

## Neuer Modus „Hiking-Darstellung“

- **Aus**: keine zusätzliche Hiking-Ebene.
- **Raster-Referenz**: Waymarked Trails als externe PNG-Kachel. Gute Orientierung, aber nicht editierbar.
- **Editierbare Linien**: OSM-/Overpass-Rohdaten als Leaflet-Vektorlinien. Farbe, Kontur, Deckkraft, Stärke und Labels sind steuerbar.
- **Vergleich**: Raster und Vektor bewusst gemeinsam sichtbar, um Abweichungen zu prüfen.

## Farbmodus der editierbaren Linien

- **Einheitlich**: alle Vektorlinien in einer wählbaren Farbe. Empfohlener Standard für ruhige Kartendarstellung.
- **OSM-Farbe**: verwendet vorhandene OSM-Farbwerte, wenn vorhanden; sonst Fallback.
- **Netzwerk**: färbt nach OSM-Netzwerk (`iwn`, `nwn`, `rwn`, `lwn`).

## Verhalten bei vorhandenen Alt-Einstellungen

Wenn aus V2.4.2 noch Raster und Vektor gleichzeitig aktiv waren, wird beim Start auf **Editierbare Linien** migriert. Der Vergleichsmodus kann danach gezielt wieder ausgewählt werden.
