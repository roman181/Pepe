# ⚔️ Clash of Pepe - Enhanced Edition

Ein episches Tower Defense Strategiespiel mit Meme-Charakteren! Verteidige deinen Tower gegen Wellen von Gegnern mit verschiedenen Einheiten, Power-Ups und strategischen Elementen.

![Version](https://img.shields.io/badge/version-2.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 🎮 Features

### Kern-Gameplay
- **8 einzigartige Einheiten** mit unterschiedlichen Fähigkeiten und Statistiken
- **Endlose Wellen** mit steigender Schwierigkeit
- **Tower Defense Mechanik** mit strategischer Einheitenplatzierung
- **Elixir-System** für Ressourcenmanagement
- **Boss-Wellen** alle 5 Runden mit verstärkten Gegnern

### Power-Up-System
- ⚡ **Rage**: Erhöht Geschwindigkeit und Schaden aller Einheiten (8 Sekunden)
- ❤️ **Heal**: Heilt deinen Tower um 500 HP
- ❄️ **Freeze**: Friert alle Gegner für 5 Sekunden ein
- 30 Sekunden Cooldown pro Power-Up

### Progression
- **Level-System** mit XP und Belohnungen
- **8 Achievements** mit Coin-Belohnungen
- **Einheiten-Upgrades** zur Verbesserung von HP und Schaden
- **Trophäen-System** basierend auf Siege/Niederlagen
- **Daily Rewards** für regelmäßige Spieler

### Combat-Features
- **Combo-System**: Schnelle Kills erhöhen Multiplikator
- **Projektil-basierter Kampf** mit Zielerfassung
- **Spezialfähigkeiten**: Splash-Damage, erhöhte Geschwindigkeit, Schild
- **Intelligente AI** mit Zielpriorisierung

## 🎯 Einheiten-Übersicht

| Einheit | Icon | Kosten | HP | Schaden | Geschwindigkeit | Spezial |
|---------|------|--------|----|---------|--------------------|---------|
| Pepe | 🐸 | 2 | 100 | 15 | 80 | - |
| Doge | 🐕 | 3 | 200 | 25 | 60 | Tank |
| Wojak | 😢 | 4 | 80 | 40 | 50 | Fernkampf |
| Chad | 💪 | 5 | 300 | 35 | 40 | Ultra-Tank |
| Wizard | 🧙 | 6 | 120 | 60 | 45 | Splash Damage |
| Ninja | 🥷 | 3 | 90 | 30 | 120 | Sehr schnell |
| Tank | 🛡️ | 7 | 500 | 20 | 30 | Unzerstörbar |
| Archer | 🏹 | 4 | 100 | 35 | 65 | Präzise |

## 🏆 Achievements

- **Erster Sieg**: Gewinne dein erstes Spiel (+50 Coins)
- **Combo Master**: Erreiche einen 5er Combo (+100 Coins)
- **Survivor**: Überlebe 10 Wellen (+150 Coins)
- **Killer**: Besiege 50 Gegner (+200 Coins)
- **Power-Up Pro**: Nutze 10 Power-Ups (+100 Coins)
- **Perfekt**: Gewinne ohne Schaden (+300 Coins)
- **Millionär**: Sammle 1000 Coins (+250 Coins)
- **Collector**: Kaufe alle Units (+500 Coins)

## 🚀 Installation & Start

### Schnellstart
1. Lade das Repository herunter
2. Öffne `Game202_Enhanced.html` in einem modernen Browser
3. Spiele sofort los!

### Für Entwickler
```bash
# Repository klonen
git clone https://github.com/yourusername/clash-of-pepe.git

# In Verzeichnis wechseln
cd clash-of-pepe

# Mit lokalem Server starten (empfohlen)
python -m http.server 8000
# oder
npx serve

# Im Browser öffnen
http://localhost:8000
```

## 📱 Browser-Kompatibilität

- ✅ Chrome/Edge (empfohlen)
- ✅ Firefox
- ✅ Safari
- ✅ Mobile Browser (iOS/Android)

**Anforderungen:**
- Moderner Browser mit HTML5 Canvas Support
- JavaScript aktiviert
- Mindestens 1024x768 Auflösung empfohlen

## 🎨 Technologie-Stack

- **HTML5 Canvas** für Game Rendering
- **Vanilla JavaScript** (keine Abhängigkeiten!)
- **CSS3** mit Animationen und Effekten
- **LocalStorage** für Spielstand-Speicherung
- **Responsive Design** für Mobile & Desktop

## 🎯 Spielanleitung

### Steuerung
- **Einheiten spawnen**: Klicke auf die Karten unten
- **Power-Ups aktivieren**: Klicke auf die Power-Up-Buttons oben
- **Pause**: Pause-Button oben links

### Strategie-Tipps
1. **Balanciere dein Elixir**: Spare für starke Einheiten oder spawne kontinuierlich
2. **Nutze Power-Ups strategisch**: Freeze bei großen Wellen, Heal bei niedrigem HP
3. **Combo-Aufbau**: Schnelle Kills = höhere Belohnungen
4. **Unit-Synergien**: Kombiniere Tank + Fernkämpfer für optimale Verteidigung
5. **Boss-Wellen**: Spare Power-Ups und Elixir für Welle 5, 10, 15...

### Fortschritt
- Coins durch Siege sammeln
- Neue Einheiten im Shop kaufen
- Einheiten upgraden für bessere Stats
- Level aufsteigen für mehr Rewards
- Achievements freischalten für Bonus-Coins

## 📊 Spielmechaniken

### Ressourcen-System
- **Elixir**: Regeneriert mit 1.2/Sekunde, Max: 10
- **Coins**: Permanente Währung für Upgrades
- **Trophäen**: Rang-System (+25 bei Sieg, -10 bei Niederlage)
- **XP**: Level-Progression (100 XP pro Level)

### Kampf-System
- Einheiten greifen automatisch nächstes Ziel an
- Projektile verfolgen bewegliche Ziele
- Splash-Damage trifft mehrere Gegner (Wizard)
- Combo-Multiplikator: 1.0x + 0.1x pro Combo

### Gegner-Skalierung
```javascript
HP = Base HP × (1 + Wave × 0.15)
Damage = Base Damage × (1 + Wave × 0.10)
Boss: HP × 2, Damage × 1.5
```

## 🔧 Anpassung & Modding

Das Spiel ist vollständig in einer HTML-Datei enthalten und kann leicht angepasst werden:

```javascript
// Konfiguration anpassen (Zeile ~27)
const CONFIG = {
    mapWidth: 2400,        // Spielfeld-Breite
    elixirMax: 10,         // Max Elixir
    elixirRate: 1.2,       // Elixir pro Sekunde
    spawnCooldown: 1000,   // Cooldown zwischen Spawns
    powerUpCooldown: 30000 // Power-Up Cooldown
};

// Neue Einheit hinzufügen (Zeile ~35)
const UNITS = {
    newUnit: {
        name: 'New Unit',
        icon: '🎯',
        cost: 4,
        hp: 150,
        damage: 30,
        speed: 70,
        range: 100,
        attackSpeed: 1.2,
        projectile: '⚡',
        baseCost: 300,
        description: 'Beschreibung'
    }
};
```

## 📝 Changelog

### Version 2.0 (Enhanced Edition)
- ✨ Power-Up-System hinzugefügt (Rage, Heal, Freeze)
- 🎮 4 neue Einheiten (Wizard, Ninja, Tank, Archer)
- 🏆 Achievement-System mit 8 Achievements
- ⚡ Combo-System für Bonus-Rewards
- 🎁 Daily Reward System
- 👾 Boss-Wellen alle 5 Runden
- 💥 Verbesserte visuelle Effekte und Animationen
- 🎨 Achievement-Panel mit Toggle
- 📊 Erweiterte Session-Statistiken
- 🔧 Performance-Optimierungen

### Version 1.0 (Original)
- 🎮 Basis Tower Defense Gameplay
- 🐸 4 Basis-Einheiten (Pepe, Doge, Wojak, Chad)
- 🏰 Tower-System mit HP
- 💧 Elixir-Ressourcen-Management
- 📈 Level und XP System
- 🪙 Coin-basierte Wirtschaft
- 📱 Mobile-optimiertes UI

## 🤝 Contributing

Beiträge sind willkommen! Hier ist wie du helfen kannst:

1. Fork das Repository
2. Erstelle einen Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit deine Änderungen (`git commit -m 'Add some AmazingFeature'`)
4. Push zum Branch (`git push origin feature/AmazingFeature`)
5. Öffne einen Pull Request

### Ideen für Beiträge
- 🎨 Neue Einheiten mit einzigartigen Fähigkeiten
- 🎯 Neue Power-Ups oder Spezialfähigkeiten
- 🏆 Mehr Achievements
- 🎮 Neue Spielmodi (Survival, Endless, Challenge)
- 🌍 Verschiedene Maps oder Themes
- 🔊 Sound-Effekte und Musik
- 🌐 Mehrsprachigkeit
- 📊 Leaderboard-System

## 📄 Lizenz

Dieses Projekt ist unter der MIT License lizenziert - siehe [LICENSE](LICENSE) Datei für Details.

## 👏 Credits

- **Original Konzept**: Tower Defense Genre
- **Meme-Charaktere**: Internet-Kultur
- **Entwicklung**: Community-driven Open Source Project
- **Emojis**: Unicode Standard

## 🐛 Bug Reports & Support

Gefunden einen Bug oder hast Vorschläge?
- Öffne ein [Issue](https://github.com/yourusername/clash-of-pepe/issues)
- Beschreibe das Problem detailliert
- Füge Screenshots hinzu wenn möglich

## 🎮 Viel Spaß!

Viel Erfolg beim Verteidigen deines Towers! 🏰⚔️

---

**Made with ❤️ by the Community**

⭐ Star das Projekt wenn es dir gefällt!
🔔 Watch für Updates!
