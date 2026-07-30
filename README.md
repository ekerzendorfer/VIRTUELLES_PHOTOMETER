# SpektralLab – Virtuelles Photometer

Browserbasierte Single-HTML-App für Photometrie, Spektren, Eichkurven, Gleichgewichte und Reaktionskinetik im Chemieunterricht.

**Repository:** `VIRTUELLES_PHOTOMETER`  
**Sichtbarer App-Titel:** `SpektralLab – Virtuelles Photometer`  
**Aktueller Stand:** `v0.4.0 – Aufgabenmodus und externer Protokollworkflow`

## Neu in Version 0.4.0

- aktivierter Hauptbereich **Aufgaben**
- Aufgaben aus einer eingebetteten, erweiterbaren JSON-Struktur
- fünf Startaufgaben für Spektren und Eichkurven
- drei Anspruchsniveaus: geführt, teiloffen und offen
- automatische Vorbereitung geeigneter Versuchsparameter beim Start
- eindeutige Aufgabenkennungen
- aktive Aufgabenanzeige in Spektren- und Eichkurvenmodus
- Aufgabenblatt als Markdown-Export
- kompakte Messübersicht als Markdown-Export
- CSV-Rohdaten enthalten Aufgaben-ID und Aufgabenkennung
- Protokoll-Checkliste ohne interne Texteingabe oder automatische Bewertung
- getrennte LehrerInnenhinweise

## Didaktisches Grundprinzip

Die App strukturiert den Messauftrag, simuliert die Messung und stellt Rohdaten bereit. Die SchülerInnen führen außerhalb der App ein vollständiges naturwissenschaftliches Protokoll mit Fragestellung, Messbedingungen, Daten, Diagrammen, Berechnungen, Interpretation und Fehlerdiskussion.

Die Checkliste in der App dokumentiert nur den Arbeitsfortschritt. Sie ersetzt kein Protokoll.

## Bereits enthalten

- fünf didaktisch parametrisierte Spektralmodelle
- sichtbarer Spektralscan mit Geräteschema
- konzentrationsabhängige Farbtiefe der Küvette
- Spektrenvergleich
- Eichkurvenmodus mit Blindprobe, Standards und unbekannter Probe
- Einzel- und Wiederholungsmessungen
- CSV-Rohdatenexport
- LehrerInnenansicht mit Regression und Kontrollwerten

## Dateien

```text
VIRTUELLES_PHOTOMETER/
├── index.html
├── README.md
├── CHANGELOG.md
├── .nojekyll
└── docs/
    └── physikalische_chemie/
        ├── photometrie-spektren.md
        ├── photometrie-eichkurven.md
        ├── photometer-geraeteschema.md
        └── photometrie-aufgabenmodus.md
```

## Geplante nächste Version

### v0.5.0 – Labor- und Fehlermodus

- kontrollierbare Messfehler
- Lern- und Diagnosemodus
- zufällige und systematische Fehler
- spätere Kopplung ausgewählter Fehlerbilder an das Geräteschema
