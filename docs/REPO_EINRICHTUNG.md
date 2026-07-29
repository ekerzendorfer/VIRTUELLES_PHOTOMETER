# Einrichtung des Repositories `VIRTUELLES_PHOTOMETER`

## 1. Neues Repository anlegen

Auf GitHub:

1. **New repository** wählen.
2. Repository-Name: `VIRTUELLES_PHOTOMETER`
3. Sichtbarkeit: `Public`
4. README, `.gitignore` und Lizenz beim Anlegen zunächst nicht automatisch erzeugen.
5. Repository erstellen.

Der technische Repository-Name bleibt eindeutig. Die App selbst trägt den Titel:

> **SpektralLab – Virtuelles Photometer**

## 2. Dateien hochladen

Den Inhalt des bereitgestellten Ordners in die oberste Ebene des Repositories hochladen:

```text
index.html
README.md
CHANGELOG.md
.nojekyll
docs/REPO_EINRICHTUNG.md
docs/physikalische_chemie/README.md
```

Wichtig: `index.html` muss direkt im Hauptverzeichnis liegen.

## 3. GitHub Pages aktivieren

1. Repository öffnen.
2. **Settings** aufrufen.
3. Links **Pages** wählen.
4. Unter **Build and deployment** einstellen:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/ (root)`
5. **Save** wählen.

Die spätere Adresse lautet voraussichtlich:

```text
https://ekerzendorfer.github.io/VIRTUELLES_PHOTOMETER/
```

## 4. Erster Funktionstest

Nach der Veröffentlichung prüfen:

- App startet ohne Fehlermeldung.
- Oberfläche passt sich an kleinere Browserfenster an.
- Teststoff erscheint in der Auswahlliste.
- Testscan zeichnet ein Spektrum.
- Konzentration und Schichtdicke verändern die Absorbanz.
- Moduswechsel funktioniert.
- Nach Neuladen bleiben die letzten Einstellungen erhalten.
- „Zurücksetzen“ stellt den Ausgangszustand wieder her.

## 5. Repository-Metadaten

### Beschreibung

```text
Browserbasiertes virtuelles Photometer für Spektren, Eichkurven, Gleichgewichte und Reaktionskinetik im Chemieunterricht.
```

### Topics

```text
chemistry
chemistry-education
photometry
spectroscopy
virtual-lab
github-pages
single-html
```

## 6. Versionsstrategie

Zunächst genügt:

- `main`: jeweils stabile und vorzeigbare Version
- Entwicklung lokal oder in einem temporären Arbeitszweig
- nach erfolgreichem Test Übernahme in `main`

Für stabile Meilensteine empfiehlt sich ein Tag oder Release:

```text
v0.1.0
v0.2.0
v0.3.0
```

## 7. Arbeitsablauf pro Version

1. Vorherige stabile Version sichern.
2. Kleine, klar definierte Änderung umsetzen.
3. Funktion lokal testen.
4. GitHub-Version aktualisieren.
5. Live-Version über GitHub Pages prüfen.
6. `CHANGELOG.md` ergänzen.
7. Erst danach die nächste Funktion beginnen.

## 8. Dokumentation im Online-Begleitkurs

Die ausführliche fachliche und didaktische Dokumentation bleibt im Online-Begleitkurs. Im Repository reichen zunächst Projektbeschreibung, Versionsstand, technische Hinweise, Live-Link, Kurs-Link und Changelog.

Die begleitenden Markdown-Seiten werden im Onlinekurs unter folgendem Pfad gesammelt:

```text
docs/
└── physikalische_chemie/
    ├── index.md
    ├── virtuelles-photometer.md
    ├── photometrie-spektren.md
    ├── photometrie-eichkurven.md
    ├── photometrie-fehlermodus.md
    ├── photometrie-gleichgewicht.md
    └── photometrie-kinetik.md
```

Die genaue Aufteilung kann mit dem Ausbau der App schrittweise wachsen.

## 9. Noch nicht für v0.1.1 erforderlich

- externe `solutions.json`
- fachlich validierte Spektraldaten
- CSV-Export
- Eichkurven
- Aufgabenmodus
- Fehlermodus
- Bromthymolblau
- Kinetikmodule
- vollständige LehrerInnenansicht
- endgültige Lizenz

## 10. Abnahmekriterien

v0.1.1 gilt als abgeschlossen, wenn:

- GitHub Pages die App korrekt ausliefert,
- keine JavaScript-Fehler auftreten,
- der Testscan sichtbar von niedrigen zu hohen Wellenlängen abläuft,
- der Moduswechsel funktioniert,
- Einstellungen lokal gespeichert werden,
- die Oberfläche auf Desktop und Tablet benutzbar bleibt.
