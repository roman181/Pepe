# Changelog

All notable changes to Clash of Pepe will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.0.0] - Enhanced Edition - 2024-03-08

### Added
- ⚡ **Power-Up System**: 3 strategische Power-Ups
  - Rage: Erhöht Geschwindigkeit und Schaden (8s Dauer, 30s Cooldown)
  - Heal: Heilt Tower um 500 HP (30s Cooldown)
  - Freeze: Friert alle Gegner (5s Dauer, 30s Cooldown)
- 🎮 **4 Neue Einheiten**:
  - Wizard (🧙): Mächtiger Magier mit Splash-Damage
  - Ninja (🥷): Sehr schneller Assassine
  - Tank (🛡️): Unzerstörbarer Schild
  - Archer (🏹): Präziser Fernkämpfer
- 🏆 **Achievement-System**: 8 verschiedene Achievements
  - Erster Sieg, Combo Master, Survivor, Killer
  - Power-Up Pro, Perfekt, Millionär, Collector
- ⚡ **Combo-System**: 
  - Schnelle Kills erhöhen Combo-Zähler
  - Multiplikator: 1.0x + 0.1x pro Combo
  - 3 Sekunden Timeout zwischen Kills
- 🎁 **Daily Reward System**:
  - 100+ Coins täglich (steigt mit Level)
  - Automatische Benachrichtigung
- 👾 **Boss-Wellen**: Jede 5. Welle
  - 2x HP, 1.5x Damage
  - Längeres Spawn-Intervall
- 🎨 **Achievement-Panel**: 
  - Toggle-Button für Sichtbarkeit
  - Zeigt Fortschritt aller Achievements
- 📊 **Erweiterte Session-Stats**:
  - Kills, Max Combo, Power-Ups verwendet
  - Anzeige im Game-Over Screen

### Changed
- 💥 **Verbesserte visuelle Effekte**:
  - Splash-Damage Visualisierung (Wizard)
  - Freeze-Effekte mit Eis-Icons
  - Power-Up Glow-Animationen
  - Achievement-Benachrichtigungen
- 🎯 **Balancing-Anpassungen**:
  - Gegner-Skalierung pro Welle optimiert
  - Elixir-Regeneration angepasst
  - Unit-Kosten neu balanciert
- 🎨 **UI-Verbesserungen**:
  - Power-Up-Bar mit Cooldown-Anzeige
  - Combo-Display mit Multiplikator
  - Verbesserte Card-Animationen
  - Wave-Indicator prominent platziert
- 📱 **Mobile-Optimierungen**:
  - Responsive Power-Up-Buttons
  - Optimierte Touch-Targets
  - Verbesserte Vibration-Patterns

### Fixed
- 🐛 Projektile treffen jetzt zuverlässiger
- 🎯 Zielerfassung bei mehreren Gegnern verbessert
- 💾 LocalStorage-Speicherung optimiert
- 🎮 Performance bei vielen Einheiten verbessert
- 📊 XP-Berechnung korrigiert

## [1.0.0] - Original Release - 2024-03-01

### Added
- 🎮 **Kern Tower Defense Gameplay**
  - Tower-Verteidigung mit automatischem Combat
  - Elixir-Ressourcen-Management
  - Wellen-basiertes Spawning
- 🐸 **4 Basis-Einheiten**:
  - Pepe: Schneller Nahkämpfer (Standard-Unit)
  - Doge: Starker Tank
  - Wojak: Fernkämpfer
  - Chad: Ultimate Tank
- 🏰 **Tower-System**:
  - Spieler- und Gegner-Türme
  - HP-basierte Zerstörung
  - Visuelle HP-Anzeige
- 💧 **Elixir-System**:
  - Auto-Regeneration (1.2/Sekunde)
  - Maximum: 10 Elixir
  - Visuelle Elixir-Bar
- 📈 **Progression-System**:
  - Level-System mit XP
  - Coin-basierte Währung
  - Trophäen-Ranking
- 🎴 **Sammlung & Upgrades**:
  - Unit-Kaufsystem
  - Upgrade-Mechanik
  - Level-basierte Verbesserungen
- 🎨 **Visuelle Features**:
  - Animierter Sternen-Hintergrund
  - Nebel-Effekte
  - Grid-Floor mit Perspektive
  - Partikel-System
  - Projektil-Animationen
- 📱 **Mobile-Support**:
  - Touch-optimierte Steuerung
  - Responsive Design
  - Vibration-Feedback
  - Safe-Area-Insets
- 💾 **Persistenz**:
  - LocalStorage-Speicherung
  - Automatisches Speichern
  - Fortschritt bleibt erhalten

### Technical Features
- 🎨 HTML5 Canvas Rendering
- ⚡ Vanilla JavaScript (keine Dependencies)
- 🎭 CSS3 Animationen
- 📱 Responsive Design
- 🎮 60 FPS Game Loop
- 🔧 Modular Code-Struktur

---

## Kommende Features (Roadmap)

### Version 2.1 (Geplant)
- 🔊 Sound-Effekte und Musik
- 🌍 Verschiedene Maps/Themes
- 🎯 Neue Spielmodi (Survival, Challenge)
- 📊 Lokales Leaderboard
- 🎨 Mehr visuelle Effekte

### Version 3.0 (Zukunft)
- 🌐 Multiplayer-Support
- 🏪 Erweiterter Shop
- 🎁 Mehr Power-Ups
- 🎖️ Seasons & Events
- 🌍 Internationalisierung

---

## Bekannte Probleme

### Version 2.0
- Keine bekannten kritischen Bugs

### Version 1.0
- Performance-Drops bei vielen Einheiten (>50) - Behoben in 2.0

---

**Legende:**
- ✨ Neue Features
- 🔧 Verbesserungen
- 🐛 Bug Fixes
- 🎨 UI/UX Änderungen
- 📱 Mobile-Optimierungen
- 💾 Daten/Speicherung
- 🎮 Gameplay-Änderungen
- 📊 Statistiken/Analytics
