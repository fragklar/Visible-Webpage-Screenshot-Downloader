# Visible Webpage Screenshot Downloader

Ein leichtgewichtiges Browser-Extension-Tool, um den sichtbaren Bereich einer Webseite mit nur einem Klick zu erfassen und direkt als WebP-Datei zu speichern.

---

## 🚀 Features

* **Schnelle Erfassung:** Nimmt sofort den aktuell sichtbaren Bereich des aktiven Tabs auf.
* **WebP-Optimierung:** Konvertiert Screenshots direkt in das moderne WebP-Format für eine optimale Balance zwischen Bildqualität und geringer Dateigröße.
* **Minimalistisches Design:** Ein einfacher Klick genügt, um den Download auszulösen.
* **Manifest V3:** Entwickelt nach den neuesten Sicherheits- und Performance-Standards für Browser-Erweiterungen.

## 🛠️ Installation (Entwicklermodus)

Da dieses Plugin aktuell als Quellcode vorliegt, kannst du es wie folgt in deinem Browser (Chrome, Edge, Brave) installieren:

1. Lade dieses Repository herunter oder entpacke die `Visible Webpage Screenshot Downloader.zip`.
2. Öffne deinen Browser und navigiere zu `chrome://extensions/`.
3. Aktiviere oben rechts den **Entwicklermodus** (Developer Mode).
4. Klicke auf **Entpackte Erweiterung laden** (Load unpacked).
5. Wähle den Ordner aus, der die `manifest.json` enthält.

## 📖 Funktionsweise

Die Erweiterung nutzt die `chrome.tabs.captureVisibleTab`-API, um das aktuelle Fenster zu erfassen:

1. **Erfassung:** Das Bild wird technisch als PNG im Hintergrund aufgenommen.
2. **Verarbeitung:** Ein injiziertes Skript zeichnet das Bild auf ein unsichtbares Canvas-Element.
3. **Konvertierung & Download:** Das Bild wird in einen WebP-Blob umgewandelt und automatisch als `screenshot.webp` heruntergeladen.

## 📄 Technische Details

* **Version:** 1.1
* **Berechtigungen:** `activeTab`, `scripting`, `tabs`
* **Autor:** [fragklar.de](https://fragklar.de)

## ⚖️ Lizenz

Dieses Projekt steht unter der **MIT-Lizenz**.

> Copyright (c) 2026 [Fragklar.de](https://fragklar.de)
>
> Die Software wird "wie besehen" (as is) zur Verfügung gestellt, ohne jegliche Gewährleistung. In keinem Fall sind die Autoren oder Urheberrechtsinhaber für Ansprüche, Schäden oder sonstige Haftung haftbar.
