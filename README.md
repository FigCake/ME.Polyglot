# Polyglot for Marinara Engine

Language study in your Marinara Engine chats. The same Polyglot as the [SillyTavern extension](https://github.com/FigCake/ST.Polyglot).

### Features

- **Annotation** — vocabulary by CEFR level and grammar, highlighted in a message
- **Translation** — double-click a sentence; a whole message paragraph by paragraph (point at a paragraph, or tap it)
- **Input assistant** — fix or translate what you type
- **Wordbook** — spaced reviews; words you are learning are underlined in chat
- **Dialogue voice** — ▶ after each line, in each character's voice
- **Study modes** — flashcards, quizzes, writing, matching, dictation, shadowing, pronunciation checks
- **Anki** — `.apkg` import and export
- **Furigana** — readings over kanji

Polyglot paints over Marinara's text and never changes it, so other extensions keep working on the same messages.

### Install

1. Install [Fetchy](https://github.com/FigCake/ME.Fetchy) (`ENABLE_EXTERNAL_EXTENSIONS=true` in Marinara's `.env`)
2. Settings → Addons → External Extensions → **Install from GitHub (Fetchy)** → `FigCake/ME.Polyglot` (to update, choose **Update existing extension**: your words stay)
3. **Polyglot** → **Review and Run**
4. The globe in the top bar opens the panel and settings

### AI and voice

Uses Marinara's AI connections and Text to Speech: no key needed. Your own provider and key work too.

### Commands

With [Dispensa](https://github.com/FigCake/ME.Dispensa): `/pg-translate`, `/pg-annotate`, `/pg-check`, `/pg-lookup word`, `/pg-panel`. A quick reply `/pg-translate` translates the last reply in one tap.

### Your data

Saved on the Marinara server in `data/game-assets/polyglot/`, shared by every device and included in Marinara's backups. **Settings → Back up** makes one file that also restores in the SillyTavern extension and the [web app](https://github.com/FigCake/W.Polyglot).

To stop using Polyglot: **Erase all Polyglot data** in its settings, then delete it in Settings → Addons. Deleting it alone keeps your data.

### Requirements

Marinara Engine 2.5.0+. Pronunciation practice: Chrome or Edge, or an Azure or OpenAI key.

### Notices

[PolyForm Strict 1.0.0](LICENSE): free for noncommercial use; no changes or redistribution without permission. [Third-party notices](THIRD_PARTY_NOTICES.md). Not affiliated with Anki, Marinara Engine or SillyTavern.
