# Datengrundlage – Spektren, Gleichgewicht und Kinetik

## Primäre fachliche Orientierung

1. Shimada, T.; Hasegawa, T. Determination of equilibrium structures of bromothymol blue revealed by using quantum chemistry with an aid of multivariate analysis of electronic absorption spectra. *Spectrochimica Acta Part A* **2017**, 185, 104–110. DOI: 10.1016/j.saa.2017.05.040.

   Relevanz: Zwei Spezies reichen zur Beschreibung der pH-abhängigen Spektren aus; thermodynamischer pKa-Wert unter Berücksichtigung der Ionenstärke.

2. Ionochromism, solvatochromism and effect of dissolved gases on the spectral properties of bromothymol blue. *Journal of Molecular Liquids* **2023**.

   Relevanz: Maximum der blauen Form bei etwa 615,5 nm und spektrale Einflüsse der Messbedingungen.

3. Ergänzende spektrophotometrische Untersuchungen und Lehrversuche beschreiben die gelbe Form mit einem Maximum um 430–433 nm und verwenden häufig einen apparenten pKa-Wert nahe 7,1.

## Modellentscheidung

Die App übernimmt keine vollständigen experimentellen Spektraldatensätze. Sie verwendet Gauß-Peaks mit folgenden didaktischen Parametern:

- HIn: 433 nm, εmax 18 000 L mol⁻¹ cm⁻¹
- In⁻: 615,5 nm, εmax 24 000 L mol⁻¹ cm⁻¹
- apparentes pKa: 7,1

Diese Werte erzeugen gut lesbare Spektren mit einem gemeinsamen Schnittbereich. Sie sind als transparentes Unterrichtsmodell zu verstehen.


## Kristallviolett-Kinetik

Für Version 0.7.0 wurden folgende fachliche Eckpunkte verwendet:

- Kristallviolett reagiert mit Hydroxid zu einem nahezu farblosen Produkt.
- Bei großem Hydroxidüberschuss wird der Verlauf häufig als pseudo-erste Ordnung behandelt.
- Lehrversuche messen die Absorbanz typischerweise im grünen Spektralbereich, häufig ungefähr zwischen 565 und 590 nm.
- Für reale Geräte wird ein mittlerer Absorbanzbereich bevorzugt; publizierte didaktische Arbeiten nennen beispielsweise ungefähr A = 0,7 bis 0,1 als günstigen Auswertungsbereich.

Die in der App verwendeten Geschwindigkeitskonstanten sind didaktisch parametrisiert und nicht als Reproduktion eines einzelnen Versuchsprotokolls zu verstehen.


## Fast Green FCF in v0.7.1

### Fachliche Orientierung

Für Fast Green FCF werden in wässrigen Systemen mehrere Absorptionsbanden beschrieben. Zwei Quellen stützen insbesondere die für den sichtbaren Unterrichtsbereich verwendeten Banden:

1. Koli, P. *UV–visible spectroscopic exploratory insight into the long term photo-stability of the Fast Green FCF dye–fructose–sodium lauryl sulphate–NaOH electrolyte based photogalvanic cell.* Results in Materials **2024**, 23, 100573. DOI: 10.1016/j.rinma.2024.100573.

   Relevanz: intensives langwelliges Band bei ungefähr 622 nm und weiteres sichtbares Band um etwa 425 nm.

2. Sürme, Y.; Kahve Yıldırım, G. *Ultrasound-assisted d-SPE of Fast Green FCF on chitin bio-adsorbent prior to spectrophotometric determination.* Eurasian Journal of Science Engineering and Technology **2025**, 6(2), 89–94. DOI: 10.55696/ejset.1732523.

   Relevanz: für die wässrige Lösung werden Banden bei etwa 300, 420 und 620 nm beschrieben; 620 nm wird als Hauptmaximum verwendet.

### Modellentscheidung

Die App verwendet keine digitalisierte Originalkurve, sondern zwei Gauß-Peaks:

- Nebenband: 423 nm, didaktisch gesetztes εmax 22 000 L mol⁻¹ cm⁻¹
- Hauptband: 622 nm, didaktisch gesetztes εmax 85 000 L mol⁻¹ cm⁻¹

Die beiden Banden lassen zwischen ihnen einen vergleichsweise gut durchlässigen grünen Spektralbereich. Dadurch wird anschaulich, warum die Lösung grün erscheint, obwohl ihr Hauptabsorptionsmaximum im orange-roten Bereich liegt. Peakbreiten und Extinktionskoeffizienten sind für gut lesbare schulische Spektren parametrisiert und nicht als Referenzmesswerte zu verstehen.


## Brillantblau FCF und Hypochlorit

- Thermo Fisher Scientific: *Kinetics of Blue Dye with Hypochlorite Bleach*. Unterrichtsversuch zur photometrischen Verfolgung der Entfärbung und zum Vergleich von A, ln(A) und 1/A gegen die Zeit.
  https://documents.thermofisher.com/TFS-Assets/MSD/Flyers/FL53103-kinetics-blue-dye-hypochlorite-bleach.pdf
- Makedonas, C.: *Taking School Instrumentation One Step Forward: A Do-It-Yourself Type Spectrophotometer and a Jupyter Notebook That Enable Real Time Spectroscopy during School Lessons*. Journal of Chemical Education 2023. Enthält die Degradation von Brilliant Blue mit Bleichlösung als schulisches Echtzeit-Spektroskopiebeispiel.
  https://doi.org/10.1021/acs.jchemed.3c00248
- Gosetti et al.: *Oxidative degradation of food dye E133 Brilliant Blue FCF*. Journal of Chromatography A 2004. Die Arbeit zeigt, dass Entfärbung nicht mit vollständiger Mineralisierung gleichzusetzen ist.
  https://pubmed.ncbi.nlm.nih.gov/15553166/

Die in der App verwendeten Geschwindigkeitskonstanten sind didaktisch parametrisierte Modellwerte und keine Übernahme eines konkreten Versuchsprotokolls.
