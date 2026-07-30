# SpektralLab – Virtuelles Photometer

Browserbasierte Single-HTML-App für Spektren, Eichkurven, Messfehler, Säure-Base-Gleichgewichte und später Reaktionskinetik im Chemieunterricht.

**Repository:** `VIRTUELLES_PHOTOMETER`  
**Sichtbarer Titel:** **SpektralLab – Virtuelles Photometer**  
**Aktueller Stand:** `v0.7.0 – photometrische Kinetik mit Kristallviolett`

## Neu in v0.6.0

- aktiver Bereich **Dynamische Messung**
- Bromthymolblau als pH-abhängiges Zwei-Spezies-Modell
- Schnellauswahl pH 4, 7 und 10
- freie pH-Wahl zwischen 3 und 11
- animierte Aufnahme einzelner Spektren
- automatische Einführungsserie pH 4 / 7 / 10
- Überlagerung von bis zu sechs pH-Spektren
- Anzeige der modellierten Anteile von HIn und In⁻
- Messwerte bei 433 und 616 nm
- Markierung eines isosbestischen Bereichs
- CSV-Export der gespeicherten Spektren
- zwei neue Aufgaben zum Säure-Base-Gleichgewicht

## Modellhinweis

Das Bromthymolblau-Modul verwendet ein transparentes, didaktisch parametrisiertes Zwei-Spezies-Modell. Es ist kein digitalisiertes Originalspektrum. Als apparenter Modellwert wird `pKa = 7,1` verwendet. Literaturwerte hängen unter anderem von Ionenstärke und Messbedingungen ab.

## Bestehende Bereiche

- Spektrenaufnahme mit schematischem Photometer
- Eichkurven, Blindprobe und unbekannte Probe
- realistische Messstreuung
- Lern- und Diagnosemodus für Laborfehler
- JSON-basierte Messaufgaben
- externe Protokollführung und Rohdatenexport

## Nächster Hauptschritt

`v0.7.0` – photometrische Kinetik am Beispiel der Entfärbung von Kristallviolett mit Hydroxid.
