# SpektralLab – Virtuelles Photometer

Browserbasierte Single-HTML-App für Spektren, Eichkurven, Gleichgewichte und Reaktionskinetik im Chemieunterricht.

**Version:** v0.9.0

## Neu

Der Kinetikbereich enthält nun drei getrennte Versuche:

- Kristallviolett + Hydroxid
- Brillantblau FCF + Hypochlorit
- Iod-/Vitamin-C-Uhrreaktion

Alle Module erzeugen Rohdaten für eine externe Auswertung und erlauben Vergleichsläufe. Die beiden kontinuierlichen Entfärbungsreaktionen stellen im LehrerInnenmodus Kontrollauftragungen bereit; die Uhrreaktion zeigt Modell- und Schwellenzeit sowie 1/t.

## Start

`index.html` direkt öffnen oder über GitHub Pages veröffentlichen.


## Neu in v0.9.0

- dritter Kinetikversuch: Iod-/Vitamin-C-Uhrreaktion
- Induktionsphase und rascher Anstieg der Iod-Stärke-Absorbanz bei 600 nm
- variable Konzentrationen von Wasserstoffperoxid, Iodid und Vitamin C
- einheitlicher Absorbanz-Schwellenwert zur Bestimmung der Umschlagszeit
- Speicherung und Überlagerung von bis zu drei Uhrreaktionsläufen
- CSV-Rohdatenexport
- LehrerInnenkontrolle mit Modellzeit, gemessener Schwellenzeit und 1/t
- zwei neue Aufgaben zur Uhrreaktion

Die Auswahl bereits gespeicherter Messreihen als Datenbasis der LehrerInnenauswertung ist für den finalen Feinschliff vorgemerkt.
