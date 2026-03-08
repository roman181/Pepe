# 🚀 Installation & Deployment

## 📦 Schnellstart - Lokal spielen

Die einfachste Methode - keine Installation nötig!

### Option 1: Direkt im Browser öffnen
1. Entpacke die ZIP-Datei
2. Doppelklick auf `index.html`
3. Spiel läuft sofort! 🎮

### Option 2: Mit lokalem Webserver (empfohlen)

**Python (meist vorinstalliert):**
```bash
cd clash-of-pepe
python -m http.server 8000
```
Dann öffne: `http://localhost:8000`

**Node.js:**
```bash
npx serve
```

**PHP:**
```bash
php -S localhost:8000
```

## 🌐 GitHub Pages Deployment

Hoste das Spiel kostenlos auf GitHub Pages!

### Schritt 1: Repository erstellen
```bash
# Auf GitHub.com: Erstelle neues Repository "clash-of-pepe"

# Dann lokal:
cd clash-of-pepe
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/DEIN-USERNAME/clash-of-pepe.git
git push -u origin main
```

### Schritt 2: GitHub Pages aktivieren

1. Gehe zu deinem Repository auf GitHub
2. Klicke auf **Settings** (Einstellungen)
3. In der linken Sidebar: **Pages**
4. Bei **Source**: Wähle **GitHub Actions**
5. Der Workflow wird automatisch ausgeführt
6. Nach ~1 Minute ist dein Spiel online! 🎉

**Deine URL:**
`https://DEIN-USERNAME.github.io/clash-of-pepe/`

## 🔄 Updates veröffentlichen

Nach Änderungen einfach pushen:
```bash
git add .
git commit -m "feat: add new unit"
git push
```

GitHub Actions deployed automatisch! ⚡

## 🖥️ Andere Hosting-Optionen

### Netlify
1. Gehe zu [netlify.com](https://netlify.com)
2. Drag & Drop den Ordner
3. Fertig! 🚀

### Vercel
```bash
npx vercel
```

### Cloudflare Pages
1. GitHub Repository verbinden
2. Build Command: (leer lassen)
3. Publish directory: `/`

### Eigener Server
Einfach alle Dateien in das Webserver-Verzeichnis kopieren:
```bash
# Apache
cp -r clash-of-pepe/* /var/www/html/

# Nginx
cp -r clash-of-pepe/* /usr/share/nginx/html/
```

## 📱 Mobile App (PWA)

Das Spiel ist bereits PWA-ready! Benutzer können es zum Home-Screen hinzufügen.

### Optional: App Icons hinzufügen

Erstelle `manifest.json`:
```json
{
  "name": "Clash of Pepe",
  "short_name": "Clash of Pepe",
  "description": "Epic Tower Defense Game",
  "start_url": "/",
  "display": "fullscreen",
  "orientation": "landscape",
  "background_color": "#0a0a0a",
  "theme_color": "#ffd700",
  "icons": [
    {
      "src": "icon-192.png",
      "sizes": "192x192",
      "type": "image/png"
    },
    {
      "src": "icon-512.png",
      "sizes": "512x512",
      "type": "image/png"
    }
  ]
}
```

Füge in `index.html` im `<head>` hinzu:
```html
<link rel="manifest" href="manifest.json">
<link rel="apple-touch-icon" href="icon-192.png">
```

## 🐳 Docker (Optional)

Für fortgeschrittene Benutzer:

**Dockerfile:**
```dockerfile
FROM nginx:alpine
COPY . /usr/share/nginx/html
EXPOSE 80
```

**Build & Run:**
```bash
docker build -t clash-of-pepe .
docker run -d -p 8080:80 clash-of-pepe
```

## 🔧 Entwicklungs-Setup

### VS Code Extensions (empfohlen)
- Live Server
- Prettier - Code formatter
- ESLint
- HTMLHint

### Live Reload Setup
```bash
# Mit Live Server Extension:
# Rechtsklick auf index.html → "Open with Live Server"

# Oder mit npm:
npm install -g live-server
live-server
```

## ⚠️ Troubleshooting

### "File not found" Fehler
- Stelle sicher, dass `index.html` im Root-Verzeichnis ist
- Überprüfe Dateipfade (case-sensitive auf Linux!)

### LocalStorage funktioniert nicht
- Benutze einen Webserver statt `file://` Protokoll
- Überprüfe Browser-Einstellungen (Cookies erlaubt?)

### Spiel lädt nicht
- Öffne Browser Console (F12)
- Suche nach JavaScript-Fehlern
- Stelle sicher, dass JavaScript aktiviert ist

### Performance-Probleme
- Schließe andere Tabs/Programme
- Aktualisiere deinen Browser
- Reduziere Anzahl der Einheiten im Code

## 📞 Support

Probleme? Erstelle ein Issue auf GitHub oder kontaktiere die Community!

---

**Viel Spaß beim Spielen! 🎮⚔️**
