# 📊 Potenzial-Kalkulator Web-App

![EMUGE FRANKEN](logo.png)

Eine **mobile-optimierte, offline-fähige Web-Anwendung** zur Berechnung von CNC-Bearbeitungspotenzialen direkt auf deinem Handy.

**Entwickelt für EMUGE FRANKEN** – Mit unternehmensweitem Corporate Identity Design.

---

## 🚀 **Quick Start (2 Sekunden)**

### **📱 NEUE Hauptversion (empfohlen):**
```
👉 Öffne: potenzial-calculator-simple.html
```
✅ Saubere UI (Kacheln oben → Ergebnis unten)  
✅ EMUGE Logo & Orange-Design  
✅ Perfekt für Handy  
✅ Minimal scrollen  

### **💻 Alternative (vollständig):**
```
👉 Öffne: potenzial-calculator.html
```
Komplettere Version mit allen Details

---

## ✨ Features

- ✅ **100% Offline** – Keine Internetverbindung erforderlich
- ✅ **Mobil-optimiert** – Perfekt für iPhone, Android, Tablet
- ✅ **Lokale Speicherung** – Alle Daten bleiben auf deinem Gerät
- ✅ **Schnelle Berechnung** – Ergebnisse in Echtzeit
- ✅ **Kachel-Interface** – Intuitives, modernes Design
- ✅ **Automatische Schätzung** – Berechnet Maschinenzahl aus Mitarbeitern
- ✅ **Potenzialklassen** – Automatische A-E Klassifizierung
- ✅ **Farbcodierung** – Grün/Blau/Gelb/Orange/Grau nach Potenzial
- ✅ **Kundenverwaltung** – Speichern, bearbeiten, löschen

---

## 📁 **Dateien im Paket**

### 🟢 **App-Dateien**
- **`potenzial-calculator-simple.html`** ← **✨ NEUE Hauptversion!** (saubere UI, Handy-optimiert)
- **`potenzial-calculator.html`** ← Original-Version (vollständig)
- **`logo.png`** ← EMUGE FRANKEN Logo

### 📚 **Dokumentation**
- **`README.md`** ← Diese Datei
- **`QUICKSTART.md`** ← 30-Sekunden-Guide
- **`ANLEITUNG.md`** ← Detailliertes Handbuch
- **`CORPORATE_IDENTITY.md`** ← Design-Guidelines

### 🛠️ **Entwickler & GitHub**
- **`potenzial-calculator.jsx`** ← React Component
- **`package.json`** ← NPM-Metadaten
- **`LICENSE`** ← MIT License
- **`.gitignore`** ← Git-Config
- **`CONTRIBUTING.md`** ← Contributor Guide
- **`beispiel-daten.json`** ← Test-Daten

---

## 🚀 So geht's los

### Schnellstart (30 Sekunden)
```
1. potenzial-calculator.html öffnen → Fertig!
```

### Auf dem Handy
```
iPhone:  Safari → "Teilen" → "Zum Home-Bildschirm"
Android: Chrome → Menü → "Zum Home-Bildschirm hinzufügen"
```

Siehe **`QUICKSTART.md`** für mehr Details.

---

## 🧮 Die Berechnung

### Formel
```
Jahrespotenzial [€] = Maschinenanzahl 
                    × 5.000 € 
                    × Schichtfaktor (1,0 / 1,7 / 2,4)
                    × Materialfaktor (0,65 / 1,0 / 1,15 / 1,5)
                    × Branchenfaktor (1,0 / 1,05 / 1,1 / 1,3)
                    × Wochendendfaktor (1,0 oder 1,15)
```

### Beispielberechnung
```
Kunde: Präzisionsteile Süd GmbH
- 12 CNC-Maschinen
- 2 Schichten → 1,7×
- Edelstahl → 1,15×
- Lohnfertigung → 1,1×
- Kein Wochenendbe trieb

Potenzial = 12 × 5.000 × 1,7 × 1,15 × 1,1 = 129.030 €
Klasse: B – hohes Potenzial (Blau)
```

---

## 🎯 Potenzialklassen

| Klasse | Jahrespotenzial | Farbe | Bedeutung |
|--------|-----------------|-------|-----------|
| **A** | ≥ 150.000 € | 🟢 Grün | Top-Potenzial |
| **B** | 75.000 – 149.999 € | 🔵 Blau | Hohes Potenzial |
| **C** | 25.000 – 74.999 € | 🟡 Gelb | Mittleres Potenzial |
| **D** | 5.000 – 24.999 € | 🟠 Orange | Kleines Potenzial |
| **E** | < 5.000 € | ⚫ Grau | Geringe Relevanz |

---

## 🔧 Parameter aus der Excel

Alle Werte stammen aus deiner **`Kundenpotenzial.xlsx`**:

### Schichtfaktoren
- 1 Schicht: 1,0×
- 2 Schichten: 1,7×
- 3 Schichten: 2,4×

### Materialfaktoren
- Aluminium: 0,65×
- Stahl: 1,0× (Referenz)
- Edelstahl: 1,15×
- Titan: 1,5×

### Branchenfaktoren & Zerspanungsquoten
- **Maschinenbau**: Faktor 1,0 | Quote 0,25
- **Lohnfertigung**: Faktor 1,1 | Quote 0,60
- **Aerospace**: Faktor 1,3 | Quote 0,50
- **Werkzeug-/Formenbau**: Faktor 1,05 | Quote 0,40

### Basiswert
- Pro CNC-Maschine/Jahr: **5.000 €**
- Mitarbeiter je CNC-Maschine: **1,2** (für Schätzung)
- Wochenend-Add-on: **1,15×** (+15%)

---

## 💾 Datenspeicherung

### Wo?
Die App speichert alle Kundendaten **lokal auf deinem Gerät** im Browser-Speicher (LocalStorage).

### Sicherheit
- ✅ Keine Cloud-Verbindung
- ✅ Keine Internet erforderlich
- ✅ Keine Daten-Uploads
- ✅ 100% privat

### Persistenz
Daten bleiben erhalten, auch wenn:
- ✅ Der Browser geschlossen wird
- ✅ Das Handy neu startet
- ✅ Offline gearbeitet wird

Daten gehen verloren, wenn:
- ❌ Browser-Cache geleert wird
- ❌ Browser-Daten gelöscht werden

---

## 📱 Browser-Kompatibilität

| Browser | Desktop | Mobile |
|---------|---------|--------|
| Chrome/Chromium | ✅ | ✅ |
| Firefox | ✅ | ✅ |
| Safari | ✅ | ✅ |
| Edge | ✅ | ✅ |
| Internet Explorer | ❌ | – |

---

## 👥 Kundenverwaltung

### Kunde speichern
1. Kundendaten in die Kacheln eingeben
2. Auf "💾 Speichern" klicken
3. Kunde erscheint in der Liste

### Kunde bearbeiten
1. Auf die Kundenkarte klicken
2. Werte ändern
3. Auf "💾 Aktualisieren" klicken

### Kunde löschen
1. Auf 🗑️ auf der Kundenkarte klicken
2. Bestätigen

---

## 🛠️ Technische Details

### Verwendete Technologien
- **React 18** (UI Framework)
- **Tailwind CSS** (Styling)
- **LocalStorage API** (Datenspeicherung)
- **Babel** (JSX-Transpilation)

### Performance
- Alle Libraries über CDN (schnelle Ladezeit)
- Vollständig optimiert für Mobile
- Ultraschnelle Berechnungen (lokal)
- Keine Backend-Anfragen

### Dateigröße
- HTML-Standalone: ~45 KB
- React Component: ~8 KB (+ Dependencies)

---

## 🎨 Design-Highlights

- **Dunkles Tema** – Angenehm für die Augen, modern
- **Grüner Akzent** – Emerald-Grün für CTAs und Header
- **Farbcodierung** – Potenzialklassen sofort visuell erkennbar
- **Responsive Grid** – Automatische Anpassung an Bildschirmgröße
- **Mobile-First** – Optimiert für kleine Bildschirme

---

## ❓ Häufige Fragen

### Kann ich die App offline nutzen?
**Ja!** Das ist sogar das Hauptfeature. Öffne die HTML-Datei einfach lokal.

### Wie berechnet die App die Maschinenanzahl?
```
Maschinen = (Mitarbeiter × Branchenzerspanungsquote) / 1,2
```
Beispiel: 60 Mitarbeiter, Lohnfertigung (Quote 0,6)
→ (60 × 0,6) / 1,2 = 30 Maschinen

### Kann ich die Parameter ändern?
In der aktuellen HTML-Version sind die Werte fest hinterlegt. Du kannst die Quelle anpassen oder die React-Version verwenden.

### Was ist die AD-Schätzung?
Ein optionales Vergleichsfeld, um deine Systemberechnung gegen externe Schätzungen zu validieren.

### Wie sichere ich meine Daten?
Die App speichert lokal – es gibt keine Backup-Funktion. Tipp: Regelmäßig Browser-LocalStorage exportieren.

---

## 📊 Anwendungsbeispiele

### Vertrieb vor Ort
- Schnelle Potenzial-Rückschätzung beim Kundengespräch
- Hilft beim Priorisieren von Opportunities
- Offline einsatzbereit

### Account Management
- Übersicht aller Kundenp otenziale
- Tracking von Veränderungen (Maschineninvestitionen)
- Basis für Vertriebsgespräche

### Strategische Planung
- Portfolioanalyse nach Potenzialklassen
- Identifikation von Top-Potenziale (Klasse A)
- Ressourcen-Allokation

---

## 🚀 Nächste Schritte

1. **App testen** → Öffne `potenzial-calculator.html`
2. **QUICKSTART lesen** → 30-Sekunden-Anleitung
3. **Auf Handy installieren** → Home-Screen-Shortcut
4. **Erste Kunden eingeben** → Live ausprobieren
5. **Regelmäßig nutzen** → Bei jedem Kundenkontakt

---

## 📞 Support

### Fehler oder Fragen?
- Siehe `ANLEITUNG.md` für detaillierte Dokumentation
- Siehe `QUICKSTART.md` für schnelle Hilfe
- Überprüfe die Formel in dieser README

### Anpassungswünsche?
Die App basiert auf zwei Versionen:
- **HTML-Standalone** (einfach zu tweaken)
- **React Component** (modular, erweiterbar)

Bei Bedarf können Funktionen hinzugefügt werden, z.B.:
- Export zu Excel/PDF
- Mehrsprachigkeit
- Benutzerdefinierte Parameter
- Cloud-Synchronisation

---

## 📜 Version & Lizenz

- **Version**: 1.0
- **Status**: Production Ready
- **Kompatibilität**: Alle modernen Browser
- **Lizenz**: Privat/Unternehmensgebrauch

---

## 🎉 Fertig!

Deine **Potenzial-Kalkulator App** ist bereit. Viel Erfolg! 🚀

**→ Starte jetzt: Öffne `potenzial-calculator.html`**
