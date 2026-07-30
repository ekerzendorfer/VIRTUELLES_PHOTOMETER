# SpektralLab – Virtuelles Photometer

Browserbasierte Single-HTML-App für Photometrie, Spektren, Eichkurven, Gleichgewichte und Reaktionskinetik im Chemieunterricht.

**Repository:** `VIRTUELLES_PHOTOMETER`  
**Sichtbarer App-Titel:** `SpektralLab – Virtuelles Photometer`  
**Aktueller Stand:** `v0.5.0 – Labor- und Fehlermodus`

## Neu in v0.5.0

- realistischere natürliche Messstreuung im Normalbetrieb
- optionaler Lernmodus mit sofort sichtbarer Fehlerursache
- optionaler Diagnosemodus mit zunächst verborgener Ursache
- zufällige Laborstörungen mit einstellbarer Häufigkeit
- reproduzierbare Störungen innerhalb einer Messreihe
- einmalige gezielte Fehlerwahl im LehrerInnenmodus
- Fehlerarten:
  - ungeeignete Blindprobe
  - verschmutzte Küvette
  - Luftblase oder unvollständige Füllung
  - Pipettier- beziehungsweise Verdünnungsfehler
  - Wellenlängenabweichung
  - Nullpunktdrift
  - Streulicht bei hoher Absorbanz
- neue Diagnoseaufgabe `FE-KM-01`
- Laborhinweis in Rohwerttabelle, CSV-Export und Messübersicht

Die visuellen Fehlerbilder am schematischen Gerät sind bewusst noch nicht Bestandteil dieser Version. Sie können später gezielt ergänzt werden.

## Drei Betriebsarten

### Normalbetrieb

Die Werte enthalten eine moderate natürliche Streuung, aber keine zusätzlichen systematischen Störungen.

### Lernmodus

Zufällige Laborprobleme können auftreten und werden nach der Messung sofort benannt.

### Diagnosemodus

Laborprobleme wirken auf die Messwerte, ihre Ursache bleibt jedoch zunächst verborgen. Erst nach eigener Prüfung kann die letzte Messung aufgelöst werden.

## Didaktisches Grundprinzip

Die App simuliert die Messung und stellt Rohdaten bereit. Die SchülerInnen führen außerhalb der App ein vollständiges naturwissenschaftliches Protokoll mit Fragestellung, Messbedingungen, Daten, Diagrammen, Berechnungen, Interpretation und Fehlerdiskussion.

## Bereits enthalten

- fünf didaktisch parametrisierte Spektralmodelle
- sichtbarer Spektralscan mit Geräteschema
- konzentrationsabhängige Farbtiefe der Küvette
- Spektrenvergleich
- Eichkurvenmodus mit Blindprobe, Standards und unbekannter Probe
- Einzel- und Wiederholungsmessungen
- Aufgabenmodus mit mehreren Anspruchsniveaus
- Markdown- und CSV-Rohdatenexport
- LehrerInnenansicht mit Regression, Kontrollwerten und internem Fehlerprotokoll

## Dateien

```text
VIRTUELLES_PHOTOMETER/
├── index.html
├── README.md
├── CHANGELOG.md
├── .nojekyll
└── docs/
    └── physikalische_chemie/
        ├── photometrie-aufgabenmodus.md
        └── photometrie-fehlermodus.md
```

## Geplanter nächster Hauptschritt

### v0.6.0 – pH-abhängige Spektren und Gleichgewicht

- Bromthymolblau bei ausgewählten pH-Werten
- Überlagerung der Spektren
- freie pH-Einstellung
- Modellierung der sauren und basischen Form
- Vorbereitung einer unbekannten pH-Probe
