# Motion Fabrik

Ein Skill für **Claude Code** (läuft notfalls auch in **Codex**), mit dem du Videos
per Code baust: Erklärvideos, Werbespots, Motion Graphics und Shorts. Er richtet
alles ein und hilft dir danach, einen guten Video-Prompt zu schreiben.

**So startest du:** Gib deinem Agenten den Link zu diesem Repo und sag ihm:
„Ich will das installieren.“

```
https://github.com/Arnie936/motion-fabrik
```

---

> ### Für KI-Agenten
>
> Wenn dir jemand diesen Link gibt und das installieren will:
>
> 1. Installiere den Skill global:
>    `npx skills add Arnie936/motion-fabrik -g -y`
>    Klappt das nicht, klone das Repo und kopiere den Ordner `skills/motion-fabrik`
>    nach `~/.claude/skills/` (Claude Code) bzw. `~/.agents/skills/` (Codex).
> 2. Warte nicht auf einen Neustart. Lies sofort `skills/motion-fabrik/SKILL.md`
>    (aus dem Repo oder dem installierten Ordner) und folge der Anleitung ab Teil 1.
> 3. Sprich in der Sprache der Person und frage vor jeder Installation nach.

---

## Was passiert

1. **Einrichten.** Der Skill prüft, ob Node.js, ffmpeg und git da sind, und fragt
   dann, welches Video-Framework du willst:
   **HyperFrames** (empfohlen), **Remotion**, **Tesseract** oder gar keins.
2. **Higgsfield (optional, empfohlen).** Damit generiert der Agent Bilder,
   Videoclips, Stimmen, Musik und Soundeffekte. Der Skill verbindet die Higgsfield
   CLI oder den MCP-Connector.
3. **Prompt bauen.** Ein kurzes Interview: Worum geht es, was ist das Ziel, wie
   lang, welches Format, welche Farben oder welches Branding, gibt es eine
   Referenz, die dir gefällt, und woran erkennst du, dass das Video gut ist?
   Daraus entsteht ein Prompt, den du abnickst, und dann geht es los.

Deine Antworten aus dem Setup landen in `~/.motion-fabrik.json`. Beim nächsten
Video springt der Skill direkt zum Prompt.

## Voraussetzungen

- Claude Code oder Codex
- Node.js 22 oder neuer, ffmpeg, git (der Skill prüft das und hilft beim Installieren)
- Für Higgsfield: ein Konto mit Credits. Generieren kostet Credits, der Skill
  zeigt die Kosten vorher an.
- Für das Umschneiden fertiger Videos (z. B. Longform → Short): Python

## Aufbau

```
skills/motion-fabrik/
├── SKILL.md                      Ablauf in drei Teilen
└── references/
    ├── setup.md                  Prüfungen, Framework, Higgsfield
    ├── prompt-interview.md       Fragen, Prompt-Vorlage, Beispiele, Tipps
    └── troubleshooting.md        Was tun, wenn's klemmt
```

## Hinweise

- **Affiliate-Link:** Wer noch kein Higgsfield-Konto hat, bekommt im Setup einen
  Anmeldelink. Das ist ein Affiliate-Link: Schließt du darüber ein Abo ab, bekomme
  ich eine Provision, für dich ändert sich am Preis nichts.
- **Remotion** ist kostenlos für Einzelpersonen und Firmen bis 3 Mitarbeitende,
  größere Firmen brauchen eine Lizenz.
- **Claude Motion** (direkt in der Claude-App) braucht keine Installation, ist
  aber zurzeit nur in der Beta für Team- und Enterprise-Pläne verfügbar.

## English

Motion Fabrik is a Claude Code skill (also usable in Codex) that sets up
code-based video creation (HyperFrames, Remotion or Tesseract, plus optional
Higgsfield for images, video clips, voices and music) and then interviews you to
write a strong video prompt. Give your agent this repo link and say
"I want to install this". The skill talks to you in your language.

## Lizenz

MIT, siehe [LICENSE](LICENSE).

---

**Community:** Mehr zu Claude Code, Motion Design mit KI und Austausch mit
anderen gibt es in meiner Community:
[skool.com/ai-mit-arnie-ki-revolution](https://www.skool.com/ai-mit-arnie-ki-revolution)
