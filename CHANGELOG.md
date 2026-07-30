# Changelog

Alle wesentlichen Änderungen am Projekt werden in dieser Datei dokumentiert.

## [0.5.0] – 2026-07-30

### Hinzugefügt

- moderat stärkere natürliche Messstreuung in allen Eichmessungen
- optionaler Lernmodus mit unmittelbarer Benennung einer Laborstörung
- optionaler Diagnosemodus mit zunächst verborgener Fehlerursache
- einstellbare Fehlerhäufigkeit: gering, mittel oder hoch
- reproduzierbare, zufällige Laborprobleme innerhalb einer Sitzung
- einmalig erzwingbare Störung für LehrerInnen
- Fehlerarten: ungeeignete Blindprobe, verschmutzte Küvette, Luftblase beziehungsweise unvollständige Füllung, Pipettier-/Verdünnungsfehler, Wellenlängenabweichung, Nullpunktdrift und Streulicht
- persistierende Wirkung eines fehlerhaften Blindwerts oder einer Nullpunktdrift
- Auflösung der zuletzt gemessenen Probe im Diagnosemodus
- internes Fehlerprotokoll im LehrerInnenmodus
- Laborhinweis in Rohwerttabelle, CSV-Export und Messübersicht
- neue teiloffene Diagnoseaufgabe `FE-KM-01`

### Geändert

- Messwerte liegen im Normalbetrieb nicht mehr nahezu perfekt auf der idealen Geraden
- CSV-Export wurde um die Spalte `Laborhinweis` ergänzt
- Versions- und Speicherkennung auf v0.5.0 aktualisiert

### Bewusst noch nicht enthalten

- grafische Darstellung von Fingerabdruck, Luftblase oder fehlender Küvette im Geräteschema
- automatische Bewertung der Fehlerdiagnose
- Fehler in dynamischen Messungen
