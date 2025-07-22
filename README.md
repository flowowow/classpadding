# Classpadding

Sammlung importierbarer Programme für das Casio Classpad II

## 🚀 Installation

1. **Classpad verbinden**
   - Classpad im Modus 'USB-Massenspeicher' mit dem Computer verbinden

2. **Programme übertragen**
   - Gewünschte Programme in den Ordner `AutoImport` auf dem Classpad kopieren

3. **Bilder übertragen** (optional)
   - Gewünschte Bilder (c2p-Format) in den Ordner `Picture/c2p files` auf dem Classpad kopieren
   - Die übertragenen Bilder können z.B. in der App **'Programm'** verwendet werden (Datei → Öffnen)

4. **Programme importieren**
   - Im Taschenrechner: App **'System'** öffnen
   - Zum Reiter **'Storage'** wechseln
   - **'Storage-Ansicht/Imp.'** auswählen
   - Mit **SAVE-F** die übertragenen Programme in `main` oder `library` importieren

5. **Programme nutzen**
   - Die importierten Programme stehen in der App **'Programm'** zur Verfügung

## 📚 Verwendung

Programme werden ausgeführt mit:

<img src="ignore/Play.jpg" alt="Icon" width="50" height="50">

bearbeitet mit:

<img src="ignore/Stift.jpg" alt="Icon" width="50" height="50">

durchsucht mit:

<img src="ignore/Fernglas.jpg" alt="Icon" width="100" height="50">

## 📖 Unterteilung

### GUKR
- `AreaGaus`: Flächenberechnung mit Gauß'scher Flächenformel
- `AreaPola`: Flächenberechnung in Polarkoordinaten
- `DreiPT`: Drei-Parameter-Transformation für n Punkte
- `HelmertT`: Helmert-Transformation
- `KarZuPol` / `PolZuKar`: Koordinatentransformation kartesisch ↔ polar
- `Trans2Pk`: Zwei-Punkte-Transformation / Ähnlichkeitstransformation

### Vermessung
- `ABRISS`: Abriss-Berechnungen
- `Bogensch`: Bogenschnitt
- `Herableg` / `HeraufL`: Herab-/Herauflegung
- `HIndexF`: Horizontalindexfehler
- `Hz_SwRm`: Horizontale, satzweise Richtungsmessung
- `Kippachs` / `Zielachs`: Achsfehlerbestimmung
- `VorwSchn`: Vorwärtsschnitt
- `VW_Mess`: Vertikalwinkel

### Koordinatenreferenzsysteme
- `TRDX`: Funktion zur 7-Parametertransformation
- Parameter: T<sub>x</sub>, T<sub>y</sub>, T<sub>z</sub>, R<sub>x</sub>, R<sub>y</sub>, R<sub>z</sub>, D, X<sub>x</sub>, X<sub>y</sub>, X<sub>z</sub>
- `kTRDX`: Funktion zur 7-Parametertransformation inklusive Konvertierung der Einheiten (R′
[mas] → R′ [rad], D′ [ppm] → D′ [m], T′ [mm] → T′ [m])

## ⚠️ Wichtige Hinweise

### Genauigkeit und Limitierungen
- **Keine Garantie** für Funktionalität oder Korrektheit der Ergebnisse
- Der Taschenrechner unterstützt nur **10-stellige Zahlen** (Vor- und Nachkommastellen zusammen)
- Überschüssige Stellen werden automatisch gerundet

### Beispiel für Rundungsprobleme
```
1000000.001 + 1E-4 = 1000000.001
```
*(Die kleine Zahl 1E-4 = 0.0001 wird nicht addiert, da die Gesamtstellenzahl überschritten würde)*

### Empfehlung für Koordinaten
Bei Koordinateneingaben sollten nur die **relevanten Stellen** eingegeben werden, in denen Änderungen zu erwarten sind. Dies gewährleistet eine hinreichende Rechengenauigkeit.

## 📖 Dokumentation

Viele Programme enthalten eine **Beschreibung im Quellcode**. Bei Fragen zu spezifischen Funktionen sollten die Kommentare im jeweiligen Programmcode konsultiert werden.

---

*Entwickelt für das Casio Classpad II*
