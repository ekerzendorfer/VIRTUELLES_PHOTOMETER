# SpektralLab – Virtuelles Photometer

Browserbasierte Single-HTML-App für Spektren, Eichkurven, chemische Gleichgewichte und Reaktionskinetik im Chemieunterricht.

**Version:** v0.9.3  
**Status:** v0.9.2 fachlich unverändert, ergänzt um optionalen Analytik-Hub-Adapter

## Funktionsumfang

- Absorptionsspektren von sechs farbigen Lösungen
- schematisches Photometer mit Lichtfarbe und Abschwächung
- Eichkurven, unbekannte Proben und LehrerInnen-Kontrollauswertung
- Messstreuung sowie Lern- und Diagnosemodus für Laborfehler
- JSON-basierte Aufgaben mit externer Protokollführung
- pH-abhängige Spektren von Bromthymolblau
- Kristallviolett-Kinetik
- Brillantblau-Hypochlorit-Kinetik
- Iod-/Vitamin-C-Uhrreaktion

## Korrekturen in v0.9.2

- Die Kinetikbereiche sind nun korrekt innerhalb des Kinetik-Panels verschachtelt; die Uhrreaktion kann nicht mehr unter Bromthymolblau erscheinen.
- Beim Wechsel von einem anderen Kinetikversuch zur Uhrreaktion wird eine nicht gespeicherte alte Messung verworfen.
- „Zurücksetzen“ löscht im Uhrreaktions-Modul jetzt Messung, Diagramm, Vergleichsläufe und stellt die Standardparameter wieder her.


- gespeicherte Läufe aller drei Kinetikversuche können im LehrerInnenmodus nachträglich als Datenbasis ausgewählt werden
- Rückkehr zur aktuellen Messung über eine eigene Schaltfläche
- zwei Geschwindigkeiten für den sichtbaren Spektralscan:
  - Normal: etwa 5 Sekunden
  - Beobachtungsmodus: etwa 8 Sekunden
- vereinheitlichte Exportdateinamen mit Präfix `PHOT`, Versuchstyp und Zeitstempel
- CSV-Exporte enthalten einen einheitlichen Metadatenblock mit App-Version und Exportzeit
- Verbesserungen für kleine Bildschirme, hohen Kontrast und reduzierte Bewegung
- Sprunglink zur Hauptnavigation für Tastaturnutzung

## Start

`index.html` direkt im Browser öffnen oder über GitHub Pages veröffentlichen.

## Daten und Auswertung

Die SchülerInnenfassung der aktuellen Entwicklungsdatei erzeugt Rohdaten, ersetzt aber kein externes Protokoll. Kontrollwerte und Linearisierungen sind ausschließlich im umschaltbaren LehrerInnenmodus sichtbar. Eine getrennte SchülerInnen- und LehrerInnenfassung ist erst bei nachgewiesenem Bedarf vorgesehen.

## Dokumentation

- `docs/physikalische_chemie/photometrie-kinetik.md`
- `docs/physikalische_chemie/DATENQUELLEN.md`
- `docs/physikalische_chemie/abschluss-feinschliff.md`


## Analytik-Hub-Adapter (v0.9.3)

SpektralLab bleibt vollständig als unabhängige Single-HTML-App nutzbar. Nur ein expliziter Start mit

```text
?bridge=1&run=RUN_...
```

aktiviert den zusätzlichen Hub-Modus.

Im Hub-Modus:

- wird die gemeinsame `CHEMIE_ANALYTIK_BRIDGE` aus `CHEMIE_ANALYTIK_HUB` dynamisch geladen,
- wird der Analyse-Run aus `localStorage` gelesen,
- kann der Hub einen kleinen, app-spezifischen `input`-Kontext übergeben,
- bleibt die interne Stoffidentität einer unbekannten Probe im normalen UI verborgen,
- werden Hub-Sitzungsdaten getrennt vom bisherigen SpektralLab-Single-State gespeichert,
- kann nach einem abgeschlossenen Scan ein standardisiertes `RESULT` an den Hub zurückgegeben werden.

Die erste reale Integration verwendet `VCOE01_SOLID_AQ` im **qualitativen Spektrenmodus**. Da die Fallkonzentration noch nicht festgelegt ist, wird intern lediglich die vorhandene didaktische Modellkonzentration zur Erzeugung der Spektrenform verwendet. Sie wird nicht als quantitative Fallinformation ausgegeben.
