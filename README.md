# bewusst.ki — Werkzeuge

Drei quelloffene, clientseitige Werkzeuge aus dem Arbeitsalltag von [bewusst.ki](https://bewusstki.de). Jedes ist eine einzelne HTML-Datei: keine Installation, kein Build-Schritt, kein Server. Öffnen und benutzen.

Live gehostet: **https://bewusstki.de/werkzeuge.html**

## Die Werkzeuge

### 🔬 [`alex-fehler-labor.html`](alex-fehler-labor.html) — ALEX Fehler-Labor & Lernkarten
Extrahiert aus Session-Logs, Git-Historie und Genesis-Mustern wiederkehrende Fehler, macht daraus Lernkarten und leitet Regeln, Skills (`SKILL.md`) und Hook-Packs ab. Lokale Heuristiken laufen ohne API; optionale KI-Analyse (DeepSeek) findet subtilere Fehlentscheidungen. Teilen ist immer opt-in und redigiert.

### 🧭 [`alex-prompt-content-studio.html`](alex-prompt-content-studio.html) — ALEX Prompt- & Content-Studio
Baut Aufträge, Projekt-Kontext, `CLAUDE.md`-Regeln und Hooks zusammen, unterstützt beim Planen und bei der Session-Analyse und erzeugt Content-Entwürfe.

### 📜 [`genesis.html`](genesis.html) — Genesis: Entwicklung rekonstruieren
Kein ALEX-Bezug. Du ziehst eigene Dateien hinein (Git-Historie, Notizen, Chat-Exporte); das Werkzeug ordnet sie zu einer Zeitleiste, eine KI schlägt als Archivar Momente für ein Interview vor, du beantwortest sie aus der Erinnerung. Getrennt bleibt sichtbar, was belegt ist, was vermutet wird und was nur du bewerten kannst.

## Eigenschaften, die für alle drei gelten

- **Reine Client-Anwendung.** Eine HTML-Datei mit eingebettetem CSS/JS, läuft vollständig im Browser.
- **Daten bleiben lokal.** Was du einliest, bleibt im Browser-`localStorage` bzw. im Speicher des Tabs. Nichts wird an einen bewusst.ki-Server gesendet.
- **Bring your own key.** Wo ein KI-Anbieter (DeepSeek) genutzt wird, trägst du deinen eigenen API-Key ein. Er wird nur in `localStorage` gehalten und nur direkt an den jeweiligen Anbieter geschickt — nie an bewusst.ki.
- **Kein Tracking.**

## Lizenz

[Apache License 2.0](LICENSE) — wie die übrigen öffentlichen bewusst.ki-Repositories.
