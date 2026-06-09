# Contribution Guidelines

Danke, dass du an der **Potenzial-Kalkulator** App mitarbeiten möchtest! 🎉

## 🚀 Wie du beitragen kannst

### 1. Bugs melden
Erstelle ein [GitHub Issue](../../issues) mit:
- Beschreibung des Problems
- Schritte zum Reproduzieren
- Browser & OS
- Screenshots (falls relevant)

### 2. Features vorschlagen
Erstelle ein [GitHub Issue](../../issues) mit dem Label `enhancement`:
- Was soll die App können?
- Warum ist das wichtig?
- Beispiel-Use-Case

### 3. Code beitragen
1. **Fork** das Repository
2. Erstelle einen **Feature Branch**: `git checkout -b feature/dein-feature`
3. Mache deine **Änderungen**
4. **Teste** die App gründlich
5. **Commit**: `git commit -m "Add: Beschreibung"`
6. **Push**: `git push origin feature/dein-feature`
7. Erstelle einen **Pull Request**

## 📋 Development Setup

### Voraussetzungen
- Node.js 16+ (nur für React-Version)
- Moderner Browser (Chrome, Firefox, Safari, Edge)

### HTML-Standalone Version (keine Installation nötig)
```bash
# Einfach öffnen:
open potenzial-calculator.html
```

### React Component Version
```bash
# Dependencies installieren
npm install

# Dev-Server starten
npm start

# Build erstellen
npm build
```

## 🎨 Coding Style

- **JavaScript/React**: ES6+
- **CSS**: Tailwind CSS (keine Custom-Styles außer wenn nötig)
- **Naming**: camelCase für Variablen/Funktionen, PascalCase für Components
- **Comments**: Deutsch für Geschäftslogik, Englisch für technische Details

### Beispiel:
```jsx
// Berechne das Potenzial basierend auf Maschinen
const calculatePotential = (machineCount, factors) => {
  return machineCount * baseValue * factors.shift * factors.material;
};
```

## ✅ Vor dem Pull Request

- [ ] Code läuft ohne Fehler
- [ ] Auf mobilen Geräten getestet (iPhone, Android)
- [ ] Keine Browser-Konsolen-Fehler
- [ ] README aktualisiert (wenn neue Features)
- [ ] Neue Funktionen dokumentiert

## 📝 Commit Messages

Nutze das Format:
```
[Type]: Kurze Beschreibung (max 50 Zeichen)

Längere Erklärung hier (max 72 Zeichen pro Zeile)
- Punkt 1
- Punkt 2
```

Typen:
- `feat:` Neues Feature
- `fix:` Bugfix
- `docs:` Dokumentation
- `style:` Code-Style (keine Funktionsänderung)
- `refactor:` Code-Umstrukturierung
- `test:` Tests

### Beispiele:
```
feat: Add export to PDF functionality
fix: Mobile layout breaks on small screens
docs: Update README with new parameters
```

## 🧪 Testing

### Manuelles Testen
1. Öffne die App im Browser
2. Teste auf Desktop & Mobile
3. Teste im Offline-Modus (DevTools → Network → Offline)
4. Teste Dateneingabe & -speicherung
5. Teste alle Berechnungsszenarien

### Browser-Kompatibilität
Teste mindestens:
- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile Safari (iOS)
- ✅ Chrome Mobile (Android)

## 📚 Dokumentation

Wenn du Features hinzufügst:
1. Update `README.md` (Übersicht)
2. Update `ANLEITUNG.md` (Detailierte Beschreibung)
3. Update `QUICKSTART.md` (Falls quick Reference)
4. Inline-Kommentare im Code

## 🐛 Bekannte Probleme

Siehe [GitHub Issues](../../issues) für:
- Offene Bugs
- Geplante Features
- Diskussionen

## 🎯 Roadmap

Geplante Verbesserungen:
- [ ] PDF-Export
- [ ] Excel-Import
- [ ] Dark/Light Mode Toggle
- [ ] Mehrsprachigkeit (English)
- [ ] Datenbank-Anbindung (optional)
- [ ] Vergleichs-Funktionen zwischen Kunden

## ❓ Fragen?

- **Issues**: Für Bugs & Features
- **Discussions**: Für Fragen & Ideen
- **README**: Für Dokumentation

---

**Danke für deine Unterstützung!** 🚀
