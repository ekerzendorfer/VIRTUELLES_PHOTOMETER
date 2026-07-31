# Photometrische Kinetik mit Kristallviolett

## Ziel

Version 0.7.2 enthält die photometrische Absorbanz-Zeit-Messung des Virtuellen Photometers. Verfolgt wird die Entfärbung von Kristallviolett durch Hydroxid-Ionen.

## Reaktionsmodell

Bei großem Hydroxidüberschuss wird die Hydroxidkonzentration während eines einzelnen Laufs als annähernd konstant behandelt. Die Abnahme des farbigen Kristallvioletts wird deshalb als pseudo-erste Ordnung modelliert:

```text
A(t) = A∞ + (A0 − A∞) · exp(−kobs · t)
```

Der didaktische Modellwert von `kobs` steigt proportional mit der eingestellten Hydroxidkonzentration. Die konkreten Zahlen sind auf schulisch gut beobachtbare Zeiträume abgestimmt und bilden kein bestimmtes Literaturprotokoll exakt nach.

## Messung

Einstellbar sind:

- Anfangskonzentration von Kristallviolett
- Hydroxidkonzentration
- Messdauer
- Messintervall
- Schichtdicke

Die Messung erfolgt modellhaft bei 590 nm. Die Zeitachse zeigt die reale Modellzeit; die Wiedergabe im Browser ist auf ungefähr neun Sekunden komprimiert.

## SchülerInnenmodus

Angezeigt und exportiert werden ausschließlich:

- Zeit
- Absorbanz
- Versuchsbedingungen
- einklappbare Rohwerttabelle mit laufender Messpunktzahl

Die SchülerInnen prüfen extern:

- `A` gegen `t`
- `ln(A)` beziehungsweise genauer `ln(A − A∞)` gegen `t`
- `1/A` beziehungsweise genauer `1/(A − A∞)` gegen `t`

Die passende Linearisierung, die Geschwindigkeitskonstante und die Interpretation bleiben Teil des externen Protokolls.

## LehrerInnenmodus

Nach einer vollständigen Messung werden Kontrollwerte angezeigt:

- Modellwert von `kobs`
- Halbwertszeit
- Fit von `ln(A − A∞)` gegen `t`
- Bestimmtheitsmaß

Zusätzlich kann jeweils eines von drei Kontrolldiagrammen eingeblendet werden:

1. `A` gegen `t` als Kontrollauftrag für nullte Ordnung
2. `ln(A − A∞)` gegen `t` als Kontrollauftrag für erste Ordnung
3. `1/(A − A∞)` gegen `t` als Kontrollauftrag für zweite Ordnung

Für jede Auswahl zeigt die LehrerInnenansicht die Messpunkte, eine lineare Anpassung, die Geradengleichung und `R²`. Bei der logarithmischen Auftragung wird zusätzlich `kobs` aus der negativen Steigung bestimmt.

## Aufgaben

### KI-CV-01 – Welche Reaktionsordnung beschreibt die Entfärbung?

Geführter Vergleich der drei klassischen Auftragungen und Bestimmung von `kobs`.

### KI-CV-02 – Wie beeinflusst Hydroxid die beobachtete Geschwindigkeit?

Offene Messplanung mit mehreren Hydroxidkonzentrationen und Bestimmung der Reaktionsordnung bezüglich Hydroxid.

## Grenzen

- Es wird eine homogene Lösung ohne Misch- und Startverzögerung angenommen.
- Temperatur und Ionenstärke bleiben konstant.
- Das Modell berücksichtigt keine detaillierten Mechanismen oder Nebenreaktionen.
- Die Messstreuung ist didaktisch parametrisiert.


## Bedienkomfort ab v0.8.0

Die Rohwerttabelle ist standardmäßig eingeklappt. Dadurch bleiben Zeitdiagramm und laufende Messung auch bei kleinen Bildschirmen im sichtbaren Bereich. Die Tabellenüberschrift zeigt dennoch fortlaufend, wie viele Messwerte bereits aufgenommen wurden. CSV-Export und weitere Messfunktionen sind unabhängig vom Zustand der Tabelle verfügbar.


# Kinetik II: Entfärbung von Brillantblau mit Hypochlorit

## Reaktionsidee

Brillantblau FCF wird durch Hypochlorit oxidativ entfärbt. Das sichtbare Signal wird bei 630 nm verfolgt. Hypochlorit wird im Modell im Überschuss eingesetzt; dadurch kann die Abnahme des Farbstoffs als pseudo-erste Ordnung ausgewertet werden.

Die Entfärbung zeigt den Verlust des sichtbaren Chromophors. Sie ist nicht gleichbedeutend mit einer vollständigen Mineralisierung des organischen Farbstoffs.

## Bedienung

Im Bereich **Dynamische Messung → Kinetik** kann zwischen Kristallviolett und Brillantblau/Hypochlorit gewechselt werden. Einstellbar sind Farbstoffkonzentration, Hypochloritkonzentration, Messdauer, Intervall und Schichtdicke. Bis zu drei Läufe können gespeichert und verglichen werden.

## SchülerInnenauswertung

Die App exportiert ausschließlich die Rohwerte. Extern werden A gegen t, ln(A−A∞) gegen t und 1/(A−A∞) gegen t geprüft. Für mehrere Hypochloritkonzentrationen kann anschließend der Zusammenhang zwischen k_obs und [OCl−] untersucht werden.

## Modellgrenzen

Das Kinetikmodell ist didaktisch parametrisiert. Reale Reaktionsgeschwindigkeiten hängen unter anderem von Zusammensetzung und Alter der Bleichlösung, pH-Wert, Temperatur und Farbstoffformulierung ab.


# Kinetik III: Iod-/Vitamin-C-Uhrreaktion

## Didaktische Idee

Die Uhrreaktion ergänzt die beiden kontinuierlichen Entfärbungsreaktionen um ein grundsätzlich anderes Zeitverhalten: Zunächst bleibt die Absorbanz nahezu konstant. Gebildetes Iod wird durch Ascorbinsäure sofort wieder reduziert. Erst nach Verbrauch der Vitamin-C-Reserve kann Iod beziehungsweise Triiodid akkumulieren und mit Stärke eine intensive blaue Färbung erzeugen.

Die App verfolgt die Iod-Stärke-Färbung bei 600 nm. Wegen der breiten und von den Bedingungen abhängigen sichtbaren Absorption ist dies eine didaktische Messwellenlänge, kein Anspruch auf einen universellen exakten Literaturwert.

## Modell

Die Iodbildungsrate wird vereinfacht proportional zu

```text
[H2O2] · [I-]
```

modelliert. Die Induktionszeit steigt proportional mit der Vitamin-C-Konzentration. Nach dem berechneten Umschlag steigt die Absorbanz rasch auf einen Plateauwert. Das Modell bildet das beobachtbare Schwellenverhalten ab, nicht den vollständigen elementaren Mechanismus.

## Auswertung

Die erste Überschreitung von `A = 0,200` definiert die Umschlagszeit. Für Vergleichsreihen kann `1/t` als einfacher Geschwindigkeitsersatzwert verwendet werden. Dies ist keine momentane Reaktionsgeschwindigkeit.

## Aufgaben

- `KI-UHR-01`: Umschlagszeit bestimmen und Induktionsphase deuten
- `KI-UHR-02`: Konzentrationseinfluss mit mehreren Läufen untersuchen

## Quellen und fachliche Orientierung

- Burgess, A. E.: *Kinetics of the Rapid Reaction between Iodine and Ascorbic Acid in Aqueous Solution Using UV–Visible Absorbance and Titration by an Iodine Clock*, Journal of Chemical Education, 2014.
- Wright, S. W.: *A Student Laboratory Experiment Based on the Vitamin C Clock Reaction*, Journal of Chemical Education.
- Chemistry LibreTexts: Unterrichtsversuche zur Iod-Uhr und zur Anfangsgeschwindigkeitsmethode.
