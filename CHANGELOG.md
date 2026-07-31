# Changelog

## [0.9.1] – 2026-07-31

### Hinzugefügt

- nachträgliche Auswahl gespeicherter Kristallviolett-, Bleich- und Uhrreaktionsläufe als Datenbasis der LehrerInnenauswertung
- Schaltfläche zur Rückkehr auf die aktuelle Messung
- zwei Scan-Geschwindigkeiten: Normal und Beobachtungsmodus
- einheitliche Exportdateinamen mit PHOT-Präfix, Versuchstyp und Zeitstempel
- einheitlicher Metadatenblock in CSV-Exporten
- Sprunglink zur Hauptnavigation
- Unterstützung erhöhter Kontraste und zusätzliche Regeln für reduzierte Bewegung

### Verbessert

- responsive Darstellung der dynamischen und kinetischen Arbeitsbereiche
- Tabellen bleiben auf kleinen Bildschirmen innerhalb lokaler horizontaler Scrollbereiche
- LehrerInnenansicht zeigt die aktuell verwendete Datenbasis eindeutig an
- bestehende Sitzungen aus v0.9.0 bleiben durch denselben Local-Storage-Schlüssel grundsätzlich kompatibel

### Geprüft

- Spektrenscan und beide Scan-Geschwindigkeiten
- Eichkurven-Nullabgleich und Standardmessung
- Bromthymolblau-Einzelscan
- vollständige Messungen aller drei Kinetikmodule
- gespeicherte Vergleichsläufe und nachträgliche LehrerInnenauswertung
- CSV-Dateinamen und Metadaten
- Darstellung bei 320 px Breite
- JavaScript-Syntax, doppelte HTML-IDs und ZIP-Integrität

## [0.9.0] – 2026-07-31

### Hinzugefügt

- dritter Kinetikversuch: Iod-/Vitamin-C-Uhrreaktion
- variable Anfangskonzentrationen von H₂O₂, I⁻ und Vitamin C
- photometrischer Verlauf bei 600 nm mit Induktionsphase und raschem Farbumschlag
- definierte Auswerteschwelle A = 0,200
- Umschlagszeit und Geschwindigkeitsersatzwert 1/t
- Speicherung, Vergleich und CSV-Export von bis zu drei Messreihen
- LehrerInnenkontrolle mit Modell- und Schwellenzeit
- Aufgaben KI-UHR-01 und KI-UHR-02

### Vorgemerkt

- Auswahl gespeicherter Messreihen als Datenbasis der LehrerInnenauswertung
- optionales fortgeschrittenes Kinetiksystem mit tatsächlich linearer 1/A-Auftragung

## [0.8.0] – 2026-07-31

### Hinzugefügt

- zweiter Kinetikversuch: Brillantblau FCF + Hypochlorit
- eigene Versuchsauswahl innerhalb des Kinetikbereichs
- variable Farbstoff- und Hypochloritkonzentration
- animierte Absorbanz-Zeit-Messung bei 630 nm
- einklappbare Rohwerttabelle und reiner CSV-Rohdatenexport ohne Modell-k_obs
- Speicherung und Überlagerung von bis zu drei Bleichläufen
- LehrerInnenkontrolle mit A, ln(A−A∞) und 1/(A−A∞) gegen t
- zwei neue Aufgaben KI-BB-01 und KI-BB-02
- Dokumentation und Datenquellen zur Farbstoffbleiche

### Unverändert

- Kristallviolett-Kinetik
- Bromthymolblau-Gleichgewichtsmodul
- Spektren-, Eichkurven-, Fehler- und Aufgabenfunktionen
