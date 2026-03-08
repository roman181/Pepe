# Contributing to Clash of Pepe

Vielen Dank für dein Interesse an Clash of Pepe! 🎮⚔️

Wir freuen uns über jeden Beitrag - egal ob Bug Reports, Feature-Vorschläge, Code-Verbesserungen oder Dokumentation.

## 📋 Inhaltsverzeichnis

- [Code of Conduct](#code-of-conduct)
- [Wie kann ich beitragen?](#wie-kann-ich-beitragen)
- [Development Setup](#development-setup)
- [Pull Request Prozess](#pull-request-prozess)
- [Coding Standards](#coding-standards)
- [Commit Messages](#commit-messages)

## 🤝 Code of Conduct

Dieses Projekt folgt einem Code of Conduct. Durch Teilnahme verpflichtest du dich, respektvoll und konstruktiv zu sein.

**Grundregeln:**
- Sei respektvoll und freundlich
- Akzeptiere konstruktive Kritik
- Fokussiere auf das Beste für die Community
- Zeige Empathie gegenüber anderen

## 🎯 Wie kann ich beitragen?

### 🐛 Bug Reports

Gefunden einen Bug? Erstelle ein Issue mit:

```markdown
**Beschreibung:**
Kurze Beschreibung des Problems

**Schritte zum Reproduzieren:**
1. Gehe zu '...'
2. Klicke auf '...'
3. Scrolle nach '...'
4. Siehe Fehler

**Erwartetes Verhalten:**
Was sollte passieren

**Tatsächliches Verhalten:**
Was passiert stattdessen

**Screenshots:**
Falls zutreffend

**Browser/Gerät:**
- Browser: Chrome 120
- OS: Windows 11
- Gerät: Desktop
```

### 💡 Feature-Vorschläge

Hast du eine Idee? Erstelle ein Issue mit:

```markdown
**Feature-Beschreibung:**
Beschreibe das Feature

**Problem, das es löst:**
Welches Problem adressiert es?

**Vorgeschlagene Lösung:**
Wie könnte es implementiert werden?

**Alternativen:**
Andere Lösungsansätze

**Zusätzlicher Kontext:**
Screenshots, Mockups, etc.
```

### 🔧 Code-Beiträge

Beliebte Bereiche für Beiträge:

#### 🎮 Gameplay
- Neue Einheiten mit einzigartigen Fähigkeiten
- Neue Power-Ups oder Spezialfähigkeiten
- Spielmodi (Survival, Endless, Challenge)
- Balancing-Verbesserungen

#### 🎨 Visuals & UI
- Neue Animationen und Effekte
- UI/UX Verbesserungen
- Themes und Skins
- Partikel-Effekte

#### 🔊 Audio
- Sound-Effekte
- Hintergrundmusik
- Audio-System-Integration

#### 🌍 Content
- Neue Maps oder Themes
- Mehr Achievements
- Story-Elemente
- Tutorial-System

#### 🛠️ Technical
- Performance-Optimierungen
- Code-Refactoring
- Testing-Framework
- Build-Tools

## 💻 Development Setup

### Voraussetzungen
- Moderner Browser (Chrome, Firefox, Safari, Edge)
- Code-Editor (VS Code empfohlen)
- Git

### Setup-Schritte

```bash
# 1. Fork das Repository auf GitHub

# 2. Clone dein Fork
git clone https://github.com/DEIN-USERNAME/clash-of-pepe.git
cd clash-of-pepe

# 3. Erstelle einen Branch
git checkout -b feature/mein-neues-feature

# 4. Öffne das Spiel
# Option A: Direkt im Browser
# Öffne Game202_Enhanced.html

# Option B: Mit lokalem Server (empfohlen)
python -m http.server 8000
# oder
npx serve

# 5. Mache deine Änderungen

# 6. Teste gründlich
```

### 🧪 Testing

Bevor du einen PR erstellst, teste bitte:

**Funktionalität:**
- [ ] Startet das Spiel ohne Fehler?
- [ ] Funktionieren alle Features wie erwartet?
- [ ] Keine Console-Errors?

**Verschiedene Szenarien:**
- [ ] Neue Einheiten spawnen korrekt
- [ ] Power-Ups funktionieren
- [ ] Achievements werden freigeschaltet
- [ ] Speichern/Laden funktioniert
- [ ] Game-Over-Screen zeigt korrekte Daten

**Browser-Kompatibilität:**
- [ ] Chrome
- [ ] Firefox
- [ ] Safari
- [ ] Edge
- [ ] Mobile Browser

**Performance:**
- [ ] Keine Lags bei vielen Einheiten
- [ ] Flüssige 60 FPS
- [ ] Speicher-Leaks überprüft

## 📝 Pull Request Prozess

### 1. Branch erstellen
```bash
git checkout -b feature/neue-einheit-dragon
# oder
git checkout -b fix/projectile-targeting-bug
# oder
git checkout -b docs/update-readme
```

**Branch-Naming:**
- `feature/` - Neue Features
- `fix/` - Bug Fixes
- `docs/` - Dokumentation
- `refactor/` - Code-Refactoring
- `perf/` - Performance-Verbesserungen
- `test/` - Tests hinzufügen

### 2. Commits machen
```bash
git add .
git commit -m "feat: add dragon unit with fire breath ability"
```

### 3. Push zum Fork
```bash
git push origin feature/neue-einheit-dragon
```

### 4. Pull Request erstellen

**PR-Template:**
```markdown
## Beschreibung
Kurze Beschreibung der Änderungen

## Art der Änderung
- [ ] Bug Fix
- [ ] Neues Feature
- [ ] Breaking Change
- [ ] Dokumentation

## Änderungen
- Added: ...
- Changed: ...
- Fixed: ...

## Testing
- [ ] Funktioniert in Chrome
- [ ] Funktioniert in Firefox
- [ ] Getestet auf Mobile
- [ ] Keine Console-Errors

## Screenshots
Falls UI-Änderungen

## Checklist
- [ ] Code folgt Coding Standards
- [ ] Selbst-Review durchgeführt
- [ ] Kommentare wo nötig
- [ ] Dokumentation aktualisiert
```

### 5. Review-Prozess

Maintainer werden:
- Code reviewen
- Feedback geben
- Änderungen anfordern oder mergen

Sei geduldig und offen für Feedback! 🙏

## 📐 Coding Standards

### JavaScript

**Style Guide:**
```javascript
// ✅ GOOD
const CONFIG = {
    mapWidth: 2400,
    elixirMax: 10
};

class Entity {
    constructor(config, isPlayer, x, y) {
        this.type = config;
        this.isPlayer = isPlayer;
    }
    
    update(dt) {
        // Clear logic
        if(this.hp <= 0) return;
        // ...
    }
}

// ❌ BAD
var config={mapWidth:2400,elixirMax:10}

class entity{
    constructor(c,p,x,y){
        this.t=c;this.p=p;
    }
    update(d){if(this.h<=0)return;}
}
```

**Konventionen:**
- camelCase für Variablen und Funktionen
- PascalCase für Klassen
- UPPER_CASE für Konstanten
- 4 Spaces Indentation
- Semikolons verwenden
- Sprechende Variablennamen

### Kommentare

```javascript
// ✅ GOOD - Erklärt WARUM
// Scale enemy difficulty based on wave number to increase challenge
unit.hp *= (1 + game.wave * 0.15);

// ✅ GOOD - Komplexe Logik
// Check combo timeout: if more than 3 seconds passed since last kill,
// reset combo counter to maintain fair multiplier system
if(now - lastKill > CONFIG.comboTimeout) {
    game.combo = 0;
}

// ❌ BAD - Erklärt offensichtliches
// Increment i by 1
i++;
```

### CSS

```css
/* ✅ GOOD */
.unit-card {
    background: rgba(255,255,255,0.05);
    backdrop-filter: blur(10px);
    border-radius: 15px;
    transition: all 0.2s;
}

/* ❌ BAD */
.uc{background:rgba(255,255,255,.05);backdrop-filter:blur(10px)}
```

## 📝 Commit Messages

Folge [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <subject>

<body>

<footer>
```

**Types:**
- `feat`: Neues Feature
- `fix`: Bug Fix
- `docs`: Dokumentation
- `style`: Formatierung, keine Code-Änderung
- `refactor`: Code-Refactoring
- `perf`: Performance-Verbesserung
- `test`: Tests hinzufügen
- `chore`: Maintenance

**Beispiele:**
```bash
feat(units): add dragon unit with fire breath ability
fix(combat): correct projectile targeting for moving enemies
docs(readme): update installation instructions
perf(render): optimize canvas drawing for many entities
refactor(powerups): extract powerup logic into separate class
```

## 🎨 Feature-Ideen

Nicht sicher wo du anfangen sollst? Hier sind Ideen:

### Einfach (Good First Issue)
- [ ] Neue Einheit mit bestehenden Mechaniken
- [ ] Neue Achievement-Bedingung
- [ ] UI-Farb-Tweaks
- [ ] Zusätzliche Partikel-Effekte
- [ ] Dokumentations-Verbesserungen

### Mittel
- [ ] Neues Power-Up
- [ ] Sound-System hinzufügen
- [ ] Neuer Spielmodus
- [ ] Upgrade-System erweitern
- [ ] Mobile-Performance verbessern

### Fortgeschritten
- [ ] Map-System mit verschiedenen Themes
- [ ] Online-Leaderboard
- [ ] Replay-System
- [ ] Multiplayer-Mode
- [ ] Custom Unit Builder

## 🆘 Hilfe benötigt?

- 💬 Erstelle ein Issue mit deiner Frage
- 📧 Kontaktiere Maintainer
- 📖 Lies die Dokumentation
- 🔍 Durchsuche existierende Issues

## 📜 Lizenz

Durch Beiträge zu diesem Projekt stimmst du zu, dass deine Beiträge unter der MIT-Lizenz lizenziert werden.

---

**Danke für deinen Beitrag! 🎉**

Jeder Beitrag - egal wie klein - hilft das Projekt zu verbessern! ⚔️🏰
