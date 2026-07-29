# SpektralLab – Virtuelles Photometer

Browserbasierte Single-HTML-App für Photometrie, Spektren, Eichkurven, Gleichgewichte und Reaktionskinetik im Chemieunterricht.

**Repository:** `VIRTUELLES_PHOTOMETER`  
**App-Titel:** `SpektralLab – Virtuelles Photometer`  
**Version:** `v0.2.0 – Statische Spektren und Vergleich`

## Inhalt von v0.2.0

- fünf kuratierte Modellsysteme:
  - Kaliumpermanganat
  - Kupfer(II)-sulfat / Kupfer(II)-Aquoion
  - Tetraamminkupfer(II)
  - Eisen(III)-thiocyanat
  - Brillantblau FCF (E133)
- substanzabhängige Konzentrationsbereiche
- sichtbarer Scan von niedrigen zu hohen Wellenlängen
- Anzeige und Markierung des Maximums im Scan
- frei wählbare Messwellenlänge mit Anzeige von `A(λ)`
- Speicherung und Überlagerung von bis zu drei Spektren
- Hinweise zum Zusammenhang von Lösungsfarbe und absorbiertem Spektralbereich
- LehrerInnenmodus mit Modellparametern
- lokale Speicherung der aktuellen Einstellungen

## Wichtiger Modellhinweis

Die Kurven sind **didaktisch parametrisierte Spektralmodelle**. Lage und Größenordnung der Hauptbanden orientieren sich an publizierten Messwerten; die dargestellten Kurven sind jedoch keine digitalisierten Originalspektren. Sie sind für Vergleich, Parameterstudien und spätere Eichkurven konsistent aufgebaut.

## Dateien

```text
VIRTUELLES_PHOTOMETER/
├── index.html
├── README.md
├── CHANGELOG.md
├── .nojekyll
└── docs/
    ├── REPO_EINRICHTUNG.md
    └── physikalische_chemie/
        ├── README.md
        ├── photometrie-spektren.md
        └── DATENQUELLEN.md
```

## Veröffentlichung

GitHub Pages wird aus dem Branch `main` und dem Verzeichnis `/ (root)` veröffentlicht.

Voraussichtliche Adresse:

```text
https://ekerzendorfer.github.io/VIRTUELLES_PHOTOMETER/
```

## Nächster Hauptschritt

### v0.3.0 – Eichkurven

- Standards und Blindprobe
- Messung einzelner Eichwerte
- unbekannte Probe
- Rohdatenexport als CSV
- externe Auswertung als didaktisches Grundprinzip
