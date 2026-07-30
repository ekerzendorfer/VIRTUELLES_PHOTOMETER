# SpektralLab – Virtuelles Photometer

Browserbasierte Single-HTML-App für Photometrie, Spektren, Eichkurven, Gleichgewichte und Reaktionskinetik im Chemieunterricht.

**Repository:** `VIRTUELLES_PHOTOMETER`  
**Sichtbarer App-Titel:** `SpektralLab – Virtuelles Photometer`  
**Aktueller Stand:** `v0.3.2 – langsamerer Scan und konzentrationsabhängige Probenfarbe`

## Neu in Version 0.3.2

- Spektralscan auf etwa fünf Sekunden verlangsamt
- Farbintensität der Küvettenfüllung folgt didaktisch angenähert der Konzentration
- Standards einer Eichreihe werden mit abgestufter Farbintensität dargestellt
- Blindprobe bleibt nahezu farblos
- unbekannte Probe wird innerhalb derselben visuellen Skala dargestellt
- keine Änderung der Messwerte, Regression oder Exportlogik

## Bereits enthalten seit Version 0.3.0

- aktivierter Hauptbereich **Eichkurve**
- fünf editierbare Standardkonzentrationen je Stoff
- verpflichtender Nullabgleich mit Blindprobe
- Einzel- und Wiederholungsmessungen
- unbekannte Probe mit eindeutiger Probenkennung
- getrennte Rohwerte in einer Messwerttabelle
- CSV-Export mit deutschem Semikolon-/Dezimalkomma-Format
- keine automatische Auswertung im SchülerInnenmodus
- LehrerInnenansicht mit Regression, R², Kontrollkonzentration und einfachem Ausreißertest
- reproduzierbare, kleine Messstreuung innerhalb einer Sitzung

## Didaktisches Grundprinzip

Die App simuliert den Messvorgang. Die SchülerInnen übertragen die Werte in ein externes Protokoll oder exportieren die Rohdaten. Eichgerade, Regressionsgleichung, Konzentrationsbestimmung und Interpretation werden außerhalb der App durchgeführt.

## Dateien

```text
VIRTUELLES_PHOTOMETER/
├── index.html
├── README.md
├── CHANGELOG.md
├── .nojekyll
└── docs/
    └── physikalische_chemie/
        ├── DATENQUELLEN.md
        ├── photometrie-spektren.md
        └── photometrie-eichkurven.md
```

## Geplante nächste Version

### v0.4.0 – Aufgabenmodus und externer Protokollworkflow

- Aufgaben aus einer eingebetteten JSON-Struktur
- geführte, teiloffene und offene Aufgaben
- klare Trennung von Aufgaben- und LehrerInneninformationen
- Versuchskennungen und exportierbare Messbedingungen
- noch keine vollständige Protokoll- oder Textverarbeitung in der App


## Bereits enthalten seit v0.3.1

- schematisches SVG-Photometer in Spektren- und Eichkurvenmodus
- erkennbare LED-Lichtquelle, Küvette, Detektor und Anzeige
- Küvette wird beim Messstart in den Schacht eingesetzt
- Lichtfarbe folgt der aktuellen Wellenlänge
- Lichtabschwächung folgt der berechneten beziehungsweise gemessenen Absorbanz
- Nullabgleich, Standards und unbekannte Probe werden sichtbar unterschieden
- Unterstützung von `prefers-reduced-motion`
