# Polyglot for Marinara Engine

Turns your Marinara Engine chats into language study. The same Polyglot as the [SillyTavern extension](https://github.com/FigCake/ST.Polyglot), built for Marinara.

**The new version.** Polyglot no longer hides and redraws your messages: it paints its marks over Marinara's own text and shows translations in boxes floating over the chat, so other extensions' work on a message stays as it is. The version before it is kept at [FigCake/ME.Polyglot.OLD](https://github.com/FigCake/ME.Polyglot.OLD).

### Main features

- **Annotation** — Highlight vocabulary by CEFR level and grammar in any character message
- **Translate & look up** — Double-click a sentence: its translation floats under the paragraph; select a word for its meaning
- **Whole-message translation** — Turn it on for a message (its button, or `/pg-translate`), then point at a paragraph (or tap it on a phone): its translation floats under it
- **Input assistant** — Fix or translate what you type before sending
- **Wordbook & reviews** — Save words, review them on a spaced schedule; words you are learning are underlined in chat
- **Listen to dialogue** — ▶ after each line reads it aloud, in each character's voice; 🎧 reads them all
- **Study modes** — Flashcards, quizzes, writing practice, matching, dictation and shadowing
- **Pronunciation checks** — Optional, with your own key: Azure scores word by word, OpenAI transcription, and AI advice on your recording
- **Anki** — Import and export `.apkg` decks with sounds and pictures
- **Furigana** — Readings over kanji (Japanese)

### Install with Fetchy

1. Install [Fetchy](https://github.com/FigCake/ME.Fetchy) (it needs `ENABLE_EXTERNAL_EXTENSIONS=true` in Marinara's `.env`)
2. Settings → Addons → External Extensions → **Install from GitHub (Fetchy)** → `FigCake/ME.Polyglot` (with Polyglot already installed, choose **Update existing extension**: your words stay)
3. Open **Polyglot** in the list → **Review and Run** to approve it
4. A globe button appears in the top bar: the panel and Polyglot's settings

Polyglot asks for full page access: it draws its highlights and buttons on the chat and opens its own panel.

To update, check the source in Fetchy. Each update stays off until you approve it again.

### AI and voice

- **AI** — Uses Marinara's connections (the open chat's, or one you choose), so no key is needed in Polyglot. Your own provider and key also work.
- **Voice** — **Marinara voice** uses Marinara's Text to Speech service; its sounds can be saved with words. The browser's voice and other services also work. Dialogue is read in your study language (Polyglot's settings): set it to the language of your chats.
- **Look** — The panel follows your Marinara theme (custom themes too), or one of Polyglot's own (Settings → Theme). Everything outside the panel looks like Marinara's own controls.

### Commands (with Dispensa)

With [Dispensa](https://github.com/FigCake/ME.Dispensa), Polyglot's commands run in its scripts and quick replies: `/pg-translate` (whole-message translation of the last character message), `/pg-annotate`, `/pg-check`, `/pg-lookup word`, `/pg-panel`. For example, a Dispensa quick reply `/pg-translate` is one tap on a phone, or set it to auto-run after the AI's reply.

### Your data

Words, sounds and pictures are saved on the Marinara server in `data/game-assets/polyglot/`: every device sees the same wordbook, and Marinara's backups include it. Do not delete that folder (or `sfx/polyglot-upload`, normally empty) in Marinara's Game Assets screen.

**Settings → Back up** saves everything to one file, which restores in the SillyTavern extension and the [web app](https://github.com/FigCake/W.Polyglot) too. API keys are never included.

**To stop using Polyglot**, first press **Erase all Polyglot data** at the bottom of Polyglot's settings (it offers a backup first), then delete Polyglot in Settings → Addons. Deleting the extension alone keeps your data, so a reinstall picks up where you left off.

### Requirements

Marinara Engine 2.5.0 or newer with External Extensions enabled. Pronunciation practice works in Chrome or Edge, or in any browser with an Azure or OpenAI key.

### Notices

License: [PolyForm Strict 1.0.0](LICENSE) — free for noncommercial use; no changes or redistribution without permission. Open-source licenses: [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md). Polyglot is not affiliated with Anki, Marinara Engine or SillyTavern, and includes no Anki code.
