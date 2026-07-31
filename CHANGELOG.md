# Changelog

## [0.7.2] – 2026-07-31

### Hinzugefügt

- Auswahl zwischen drei Kontrolldiagrammen im LehrerInnen-Kinetikbereich:
  - `A` gegen `t`
  - `ln(A − A∞)` gegen `t`
  - `1/(A − A∞)` gegen `t`
- lineare Anpassung, Regressionsgleichung und `R²` für die jeweils gewählte Auftragung
- Ableitung von `k_obs` aus der logarithmischen Auftragung
- Speicherung der zuletzt gewählten LehrerInnen-Auftragung innerhalb der Sitzung

### Geändert

- Die lange Messdatentabelle der Kristallviolett-Kinetik ist nun einklappbar.
- Die Überschrift der Tabelle zeigt laufend die Zahl der bereits erfassten Messwerte.
- Die Tabelle bleibt während der Messung standardmäßig geschlossen, sodass das Diagramm im Mittelpunkt bleibt.

### Unverändert

- SchülerInnenmodus, Rohdaten und CSV-Export
- kinetisches Reaktionsmodell und Messstreuung
- Aufgaben KI-CV-01 und KI-CV-02
- statische Spektren, Eichkurven, Fehlermodus und Gleichgewichtsmodul

## [0.7.1] – 2026-07-31

### Hinzugefügt

- Fast Green FCF als sechste Lösung in Spektren- und Eichkurvenmodus
- didaktisches Zwei-Banden-Modell mit sichtbaren Banden um etwa 423 und 622 nm
- grüne Lösungsdarstellung und eigene Konzentrationsreihe
- hervorgehobener Messpunkt der unbekannten Probe im LehrerInnen-Eichdiagramm
- gestrichelte Hilfslinien und Beschriftung der berechneten Konzentration

### Geändert

- Auswahltexte in Dropdowns und Eingabefeldern verwenden normale Schriftstärke
- Schaltflächen und Navigationsfelder sind typografisch etwas zurückhaltender
- Überschriften und Feldbeschriftungen bleiben deutlich hervorgehoben

### Unverändert

- SchülerInnenmodus zeigt im Eichdiagramm weiterhin keine unbekannte Konzentration
- Regression, Rohdaten, Fehlerkultur und dynamische Messungen arbeiten unverändert

## [0.7.0] – 2026-07-30

### Hinzugefügt

- Kinetik-Untermodus innerhalb der dynamischen Messungen
- Entfärbung von Kristallviolett mit Hydroxid
- pseudo-erste Ordnung bei Hydroxidüberschuss
- variable Anfangskonzentrationen, Messdauer und Messintervall
- animierte Absorbanz-Zeit-Kurve
- Rohwerttabelle und CSV-Export
- Speicherung und Vergleich von bis zu drei Messreihen
- LehrerInnen-Kontrollwerte für k_obs, Halbwertszeit und ln(A−A∞)-Fit
- Aufgaben KI-CV-01 und KI-CV-02

### Didaktische Entscheidung

- Im SchülerInnenmodus werden weder die geeignete Linearisierung noch k_obs automatisch ausgegeben.
- Das schematische Photometer bleibt in den fortgeschrittenen dynamischen Messungen ausgeblendet.

## [0.6.0] – 2026-07-30

### Hinzugefügt

- Hauptbereich „Dynamische Messung“ aktiviert
- pH-abhängige Bromthymolblau-Spektren
- Zwei-Spezies-Gleichgewichtsmodell HIn / In⁻
- pH-Schnellauswahl 4, 7 und 10
- freie pH-Einstellung von 3 bis 11
- animierte Einzelscans und automatische Dreierserie
- Speicherung und Überlagerung von bis zu sechs Spektren
- Speziesanteile, Lösungsfarbe und charakteristische Absorbanzwerte
- Markierung eines isosbestischen Bereichs
- CSV-Export der überlagerten Spektren
- Aufgaben EQ-BTB-01 und EQ-BTB-02
- LehrerInnenansicht mit Modellparametern
- Sitzungswiederherstellung für pH-Einstellungen und gespeicherte Spektren

### Fachliche Modellierung

- saure Form: Maximum um 433 nm
- basische Form: Maximum um 615,5 nm
- apparenter didaktischer Modellwert pKa = 7,1
- transparente Kennzeichnung als parametrisiertes Modell

### Unverändert

- statische Spektren
- Eichkurven und CSV-Rohdaten
- Labor- und Fehlermodus
- Aufgaben- und Protokollworkflow
