# Changelog

## [0.4.0] – 2026-07-30

### Hinzugefügt

- eigenständiger Aufgabenmodus
- eingebettete, erweiterbare JSON-Aufgabenstruktur
- fünf Startaufgaben für Spektren und Eichkurven
- geführte, teiloffene und offene Aufgaben
- automatische Übergabe vorbereiteter Messparameter an den jeweiligen Messmodus
- Aufgabenkennung und aktive Aufgabenanzeige
- Markdown-Export eines Aufgabenblatts
- Markdown-Export einer kompakten Messübersicht ohne Auswertung
- Protokoll-Checkliste für den externen Arbeitsprozess
- getrennte LehrerInnenhinweise
- Aufgaben-ID und Aufgabenkennung im CSV-Rohdatenexport

### Didaktische Entscheidung

- Die App enthält keine Textverarbeitung für das Protokoll.
- Diagramme, Regressionen, Rechnungen, Interpretation und Fehlerdiskussion bleiben im SchülerInnenmodus vollständig extern.
- Die Checkliste speichert nur den Bearbeitungsstand.

## [0.3.2] – 2026-07-30

### Geändert

- Spektralscan von etwa 3,2 auf etwa 5 Sekunden verlangsamt
- Farbintensität der Küvettenfüllung wird didaktisch an die Konzentration gekoppelt
- Standardlösungen erscheinen mit abgestufter Farbintensität
- Blindprobe bleibt nahezu farblos
- unbekannte Probe verwendet dieselbe Konzentrationsskala wie die Standards

### Unverändert

- Absorbanzberechnung und Messstreuung
- Eichkurven- und Rohdatenlogik
- CSV-Export und LehrerInnenauswertung

## [0.3.1] – 2026-07-30

### Hinzugefügt

- schematisches SVG-Photometer in Spektren- und Eichkurvenmodus
- kombinierte Messanimation: Küvette einsetzen, Licht aktivieren, Abschwächung darstellen und Messwert anzeigen
- didaktisch angenäherte Lichtfarbe aus der Wellenlänge
- absorbanzabhängige Abschwächung des austretenden Lichtstrahls
- eigene Darstellungen für Blindprobe, Standards und unbekannte Probe
- barrierearme Kurztexte und Unterstützung reduzierter Bewegung

### Unverändert

- fachliche Berechnungen und Rohdatenlogik von v0.3.0
- externer Protokollworkflow
- keine automatische SchülerInnen-Auswertung

## [0.3.0] – 2026-07-29

### Hinzugefügt

- aktivierter Eichkurvenmodus
- fünf editierbare Standardkonzentrationen pro Stoff
- verpflichtender Nullabgleich mit Blindprobe
- Einzel- und Wiederholungsmessungen
- unbekannte Probe mit Sitzungs- und Probenkennung
- Messwerttabelle mit getrennten Rohwerten
- CSV-Rohdatenexport im deutschsprachigen Tabellenformat
- reproduzierbare kleine Messstreuung
- LehrerInnen-Kontrolle mit linearer Regression, R², Kontrollkonzentration und Kontrolldiagramm
- Dokumentation `photometrie-eichkurven.md`

### Didaktische Entscheidung

- Im SchülerInnenmodus werden weder Regressionsgleichung noch R² oder berechnete Konzentration angezeigt.
- Der CSV-Export enthält ausschließlich Messbedingungen und Rohdaten, keine fertige Auswertung.

## [0.2.0] – 2026-07-29

- fünf didaktisch parametrisierte Spektralmodelle
- sichtbarer Spektralscan
- Messwellenlänge und Spektrenüberlagerung

## [0.1.1] – 2026-07-29

- animierter Scanverlauf

## [0.1.0] – 2026-07-29

- technisches Single-HTML-Grundgerüst
