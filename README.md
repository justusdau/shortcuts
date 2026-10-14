# Justus Shortcuts

Meine Apple-Kurzbefehle zum Herunterladen.



## Einmalig einrichten

1. Auf github.com einloggen → oben rechts **+** → **New repository**
2. Name: `justus-shortcuts`, auf **Public** stellen → **Create repository**
3. **Add file → Upload files** → `index.html`, `shortcuts.json` und `README.md` hineinziehen → **Commit changes**
4. **Settings → Pages** → bei *Source* „Deploy from a branch“, Branch `main`, Ordner `/ (root)` → **Save**
5. Nach 1–2 Minuten ist die Seite unter `https://DEIN-GITHUB-NAME.github.io/justus-shortcuts/` online

## Neuen Kurzbefehl hinzufügen

1. In der Kurzbefehle-App: Kurzbefehl → **Teilen** → **iCloud-Link kopieren**
2. Auf GitHub `shortcuts.json` öffnen → Stift-Symbol (Bearbeiten)
3. Einen neuen Eintrag ergänzen (Komma zwischen den Einträgen nicht vergessen):

```json
{
  "name": "Mein Kurzbefehl",
  "description": "Was er macht.",
  "emoji": "🚀",
  "color": "#0a84ff",
  "tags": ["Kategorie"],
  "link": "https://www.icloud.com/shortcuts/..."
}
```

4. **Commit changes** – die Seite aktualisiert sich nach etwa einer Minute.

### Alternative: .shortcut-Datei statt Link

Exportierte `.shortcut`-Dateien in einen Ordner `shortcuts/` hochladen und im Eintrag statt `"link"` schreiben:

```json
"file": "shortcuts/MeinKurzbefehl.shortcut"
```

Der iCloud-Link ist aber bequemer: Freunde tippen ihn an und können den Kurzbefehl sofort hinzufügen.
