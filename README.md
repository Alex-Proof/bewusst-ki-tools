# bewusst.ki — Werkzeuge

Vier quelloffene, clientseitige Werkzeuge aus dem Arbeitsalltag von [bewusst.ki](https://bewusstki.de). Jedes ist eine einzelne HTML-Datei: keine Installation, kein Build-Schritt, kein Server. Öffnen und benutzen.

Live gehostet: **https://bewusstki.de/werkzeuge.html**

## Die Werkzeuge

### 🔬 [`alex-fehler-labor.html`](alex-fehler-labor.html) — ALEX Fehler-Labor & Lernkarten
Damit du denselben Agenten-Fehler nicht zum dritten Mal machst: Session-Log oder Git-Historie rein, wiederkehrende Fehler raus — als Lernkarten und fertige Regeln (`SKILL.md`, Hook-Packs) für den nächsten Lauf. Lokale Heuristiken laufen ohne API; optionale KI-Analyse findet subtilere Fehlentscheidungen. Teilen ist immer opt-in und redigiert.

### 🧭 [`alex-prompt-content-studio.html`](alex-prompt-content-studio.html) — ALEX Prompt- & Content-Studio
Aus einer vagen Idee in Minuten einen klaren Auftrag für deinen Coding-Agenten — inklusive Leitplanken, die er tatsächlich einhält. Baut Aufträge, Projekt-Kontext, `CLAUDE.md`-Regeln und Hooks zusammen, unterstützt beim Planen und bei der Session-Analyse und erzeugt Content-Entwürfe.

### 📜 [`genesis.html`](genesis.html) — Genesis: Entwicklung rekonstruieren
Kein ALEX-Bezug. Deine eigene Entwicklung nachvollziehbar rekonstruiert — aus echten Belegen (Git, Notizen, Chats), nicht aus Erinnerung allein. Du ziehst eigene Dateien hinein; das Werkzeug ordnet sie zu einer Zeitleiste, eine KI schlägt als Archivar Momente für ein Interview vor, du beantwortest sie aus der Erinnerung. Getrennt bleibt sichtbar, was belegt ist, was vermutet wird und was nur du bewerten kannst.

### 🔬 [`researcho.html`](researcho.html) — Researcho: Forschungs-Persona-Generator & Wissens-Scout
Kein ALEX-Bezug. Erschafft eine hochspezialisierte Wissenschaftler-Persona mit echter Live-Internet-Recherche: Gemini durchsucht per [Search Grounding](https://ai.google.dev/gemini-api/docs/google-search) das Web nach aktuellen Papers, Instituten und Toolstacks und belegt jede Angabe mit echten Quellen. Feld, Fachwissen und Methoden eingeben (oder eine von 5 Fach-Vorlagen wählen) — heraus kommen 6-7 downloadbare Textdateien, ein vollständiges Dossier (inkl. ZIP-Export, eingebauter Zip-Writer ohne externe Abhängigkeit) und ein Chat mit der generierten Persona. Einziges der vier Werkzeuge, das zwingend Gemini braucht (Search Grounding ist Gemini-exklusiv, kein DeepSeek/OpenAI/Anthropic-Äquivalent).

## Eigenschaften, die für alle vier gelten

- **Reine Client-Anwendung.** Eine HTML-Datei mit eingebettetem CSS/JS, läuft vollständig im Browser.
- **Daten bleiben lokal.** Was du einliest, bleibt im Browser-`localStorage` bzw. im Speicher des Tabs. Nichts wird an einen bewusst.ki-Server gesendet.
- **Bring your own key.** Fehler-Labor/Studio/Genesis: freie Wahl zwischen DeepSeek, OpenAI, Anthropic oder einem eigenen OpenAI-kompatiblen Endpunkt (teilen sich dieselbe Einstellung im selben Browser). Researcho: eigener Gemini-Key (separates Schema, da Search Grounding ein Gemini-Feature ist). Kein Key verlässt je den Browser in Richtung bewusst.ki.
- **Kein Tracking.**

## Lizenz

[Apache License 2.0](LICENSE) — wie die übrigen öffentlichen bewusst.ki-Repositories.
