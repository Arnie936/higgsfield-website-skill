# Higgsfield Website Skill 🎬

Ein Claude-Code-Skill, der aus einer kurzen Beschreibung eine **cinematische Scroll-Website mit KI-generierten Videos** baut — Higgsfield MCP (Seedance 2.0, GPT Image 2, Nano Banana), Scroll-Scrub/Exploded-View-Animationen, automatischer Browser-QA-Test und Hosting in einem Flow. Für Produkte, Portfolios, Restaurants, Immobilien, E-Commerce, SaaS, Gyms und mehr.

## 🤖 Agents first: Setup in einem Prompt

Kopiere diesen Prompt in **Claude Code** (oder einen anderen Coding-Agent) — er installiert alles:

```text
Installiere den Higgsfield-Website-Skill aus https://github.com/Arnie936/higgsfield-website-skill :

1. Hole den Skill und kopiere den Ordner "higgsfield-website" nach
   ".claude/skills/higgsfield-website" im aktuellen Projekt.
   (Frage mich, ob ich ihn stattdessen global unter "~/.claude/skills" haben will.)
   - Wenn git installiert ist: Repo in ein temporäres Verzeichnis klonen.
   - Wenn nicht: KEIN git installieren, sondern das ZIP ohne git laden und entpacken:
     https://github.com/Arnie936/higgsfield-website-skill/archive/refs/heads/main.zip
     (Windows: Invoke-WebRequest + Expand-Archive / macOS+Linux: curl -L + unzip)
   - Lege danach im Projekt-Root eine Datei "AGENTS.md" an (bzw. ergänze eine bestehende),
     damit auch Nicht-Claude-Agents (Codex, Cursor etc.) den Skill finden. Inhalt:
     "Skills und Konfiguration liegen unter .claude/ — siehe
      .claude/skills/higgsfield-website/SKILL.md fuer den Higgsfield-Website-Workflow."
2. Registriere die MCP-Server IMMER projektbasiert (--scope project), niemals global:
   claude mcp add --scope project --transport http higgsfield https://mcp.higgsfield.ai/mcp
   claude mcp add --scope project playwright -- npx @playwright/mcp@latest
3. Prüfe, ob ffmpeg installiert ist (ffmpeg -version). Falls nicht, installiere es passend
   zum Betriebssystem (Windows: winget install Gyan.FFmpeg / macOS: brew install ffmpeg /
   Linux: apt install ffmpeg) — frage mich vorher kurz um Erlaubnis.
4. Falls ich noch keinen Higgsfield-Account habe oder die MCP-Verbindung nicht autorisiert ist:
   Bitte mich, mich über diesen Link anzumelden und die Verbindung freizugeben:
   https://higgsfield.ai/s/mcp-arnold-oberleiter-PGBQCb
5. Sag mir, dass ich Claude Code einmal neu starten soll, damit die MCP-Server verbinden.
6. Bestätige die Installation und erkläre mir in 2 Sätzen, wie ich den Skill benutze
   (einfach beschreiben, welche Website ich will — der Skill übernimmt den Rest).
```

> Hinweis: Der Anmelde-Link ist ein Referral-Link von mir, danke =)

## Was der Skill kann

- **Interview statt Prompt-Bastelei:** Was willst du bauen? Eigenes Input-Bild oder Hero-Bild generieren? HD oder 4K? Zielsprache? Zielgeräte (Desktop/Tablet/Mobile)?
- **10 Templates + 7 Scroll-Konzepte:** Luxury Product, Journey, Portfolio, E-Commerce, Restaurant, Real Estate, Automotive, SaaS, Agency, Gym — kombiniert mit bewusst gewähltem Scroll-Verhalten (Scroll Scrub, **Exploded View**, Push Through, Scrollytelling u.a.).
- **Kosten unter Kontrolle:** Shot-Plan mit Credit-Schätzung und Freigabe, bevor irgendetwas generiert wird; Hero-Bild-Checkpoint, bevor teure Videos entstehen.
- **Handwerk statt KI-Look:** These-Zeile, OKLCH-Palette, Copywriting-Regeln, Anti-AI-Verbotsliste, Video-Gesetze für sauber scrubbare Clips.
- **Echter QA-Pass:** Der Agent testet die fertige Seite selbst im Browser (Playwright): Scroll-Scrub, Konsole, Layout, gewählte Viewports — erst dann kommt die Abnahme-Frage.
- **Hosting:** Auf Wunsch direkt über den Higgsfield MCP.

## Manuelle Installation

1. Ordner `higgsfield-website/` nach `.claude/skills/` deines Projekts kopieren (oder `~/.claude/skills/` für global).
   Für Nicht-Claude-Agents (Codex, Cursor …) zusätzlich eine `AGENTS.md` im Projekt-Root anlegen mit dem Verweis: *"Skills und Konfiguration liegen unter `.claude/` — siehe `.claude/skills/higgsfield-website/SKILL.md`."*
2. Higgsfield MCP hinzufügen: `claude mcp add --scope project --transport http higgsfield https://mcp.higgsfield.ai/mcp`
3. Higgsfield-Account anlegen / MCP autorisieren: https://higgsfield.ai/s/mcp-arnold-oberleiter-PGBQCb
4. Claude Code neu starten und z.B. schreiben: *„Mach mir eine cinematische Website für meine Uhrenmarke, mit Exploded-View-Effekt."*

## Voraussetzungen

- Claude Code und Higgsfield-Credits (Seedance 2.0)
- Higgsfield MCP + Playwright MCP (projektbasiert) und ffmpeg — **fehlt etwas, installiert der Skill es selbst** beim Setup-Check; der Setup-Prompt oben richtet ebenfalls alles ein

## Struktur

```
higgsfield-website/
├── SKILL.md                  # Workflow: Interview → Kostenfreigabe → Hero-Checkpoint →
│                             # Videos → Website → Browser-QA → Abnahme → Hosting
└── references/
    ├── templates.md          # Die 10 Website-Templates (Shots, Sektionen, Design, Copy)
    └── craft.md              # 7 Scroll-Konzepte, Design-DNA, Video-Gesetze, Qualitäts-Gates
```
