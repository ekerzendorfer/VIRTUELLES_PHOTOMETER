# SpektralLab – Virtuelles Photometer

Browserbasierte Single-HTML-App für Photometrie, Spektren, Eichkurven, Gleichgewichte und Reaktionskinetik im Chemieunterricht.

**Repo-Name:** `VIRTUELLES_PHOTOMETER`  
**Sichtbarer App-Titel:** `SpektralLab – Virtuelles Photometer`  
**Aktueller Stand:** `v0.1.0 – Grundgerüst und Techniktest`

## Ziel von Version 0.1.0

Diese erste Version ist bewusst noch kein fertiges Photometer. Sie prüft die technische Basis:

- Single-HTML-Betrieb
- responsive Oberfläche
- Hauptnavigation
- SchülerInnen- und LehrerInnenmodus
- eingebettete JSON-Stoffdaten
- zentrale Diagrammkomponente
- Eingabevalidierung
- lokale Sitzungsverwaltung
- Zurücksetzen der App
- Betrieb über GitHub Pages

Der enthaltene Kaliumpermanganat-Datensatz ist ein **technischer Demo-Datensatz** und noch kein fachlich validierter Referenzdatensatz.

## Dateien

```text
VIRTUELLES_PHOTOMETER/
├── index.html
├── README.md
├── CHANGELOG.md
├── .nojekyll
└── docs/
    └── REPO_EINRICHTUNG.md
```

## GitHub Pages

Die Einrichtung ist in [`docs/REPO_EINRICHTUNG.md`](docs/REPO_EINRICHTUNG.md) beschrieben.

Die spätere Adresse lautet voraussichtlich:

```text
https://ekerzendorfer.github.io/VIRTUELLES_PHOTOMETER/
```

## Nächste Version: v0.2.0

- fachlich kuratierte Stoffdaten
- mehrere farbige Lösungen
- Spektrumaufnahme im sichtbaren Bereich
- Markierung von `λmax`
- Speicherung und Überlagerung ausgewählter Spektren
- didaktische Hinweise zu absorbierter und beobachteter Farbe

## Didaktischer Grundsatz

Die App erzeugt Messdaten, ersetzt aber nicht das externe Versuchsprotokoll. Eichwerte, Auswertung, Diagramme und Interpretation bleiben Aufgabe der SchülerInnen.

## Lizenz

Die Lizenz sollte vor der öffentlichen Version 1.0.0 ausdrücklich festgelegt werden. Bis dahin sollte das Repository nicht ohne einen klaren Lizenzhinweis als frei nachnutzbar bezeichnet werden.
