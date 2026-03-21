# Lojban Word Trainer

A lightweight, single-file HTML app for learners of Lojban who want to practice vocabulary output — that is, not just recognizing words, but actively using them in sentences.

No installation, no server, no account. Open the file in a browser and it works.

---

## What it does

The core loop is simple: you collect words as you study, the app draws a random one, and you write a sentence with it. The sentence gets saved so you build up a personal corpus of your own Lojban output over time.

---

## Tabs

**Add words** — Enter a word (valsi), its class, a definition, and optional notes. Duplicate words are rejected automatically. Shows the 5 most recently added words as a quick preview.

**Words** — Full word bank with a search bar (searches word, definition, and notes) and class filters. Shows the last 10 added by default; searching returns all matches. Each word can be edited or deleted inline.

**Practice** — Draws a random word from your chosen class (defaults to gismu, which is the most useful for sentence building). You write a sentence using that word and save it. Duplicate sentences are rejected using normalized matching (case and spacing insensitive).

**Sentences** — Log of all saved sentences, newest first. Last 10 shown by default. Search by sentence text or by the word that prompted it. Each sentence can be edited or deleted inline.

**Export / Import** — Copy or download your full data as a `.json` file. Paste JSON back in to import and merge data between devices.

---

## Word classes

Words are organized by Lojban grammatical class:

- **gismu** — root words with a full place structure (x1, x2...). Best class for sentence practice.
- **cmavo** — grammatical particles and structure words.
- **lujvo** — compound words built from gismu.
- **other** — anything else (fu'ivla, names, etc.)

---

## Data persistence

Data is saved in the browser's `localStorage`, tied to the file path on disk. As long as you open the same file from the same location in the same browser, your data will be there.

To move data between computers or browsers, use the Export tab to download a `.json` file and the Import tab to load it on the other machine.

---

## No dependencies

Single `.html` file. No frameworks, no build step, no internet connection required after download.

---

Created by Claude AI.
