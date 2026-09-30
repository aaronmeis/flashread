# Flashread

A private speed reader that runs in your browser. Paste an article, chapter, or note and read it one word at a time, with your eyes staying in one place.

**Open it:** https://aaronmeis.github.io/flashread/

Nothing is uploaded. Your text, settings, and reading position are stored only in your browser (`localStorage`).

## How to use

1. Paste text, open a `.txt` / `.md` / `.html` file, or drop a file onto the page. You can also pick one of the built-in samples.
2. Press **Play**, press **Space**, or tap the word.
3. Keep your eyes on the red letter. It marks the point where your eye recognizes a word fastest.

Start near 300 words per minute. Slow down when meaning starts to slip.

## Controls

| Key | Action |
|---|---|
| Space, or tap the word | Play / pause |
| ← / → | Back / forward 10 words |
| `[` / `]` | Slower / faster by 20 words per minute |
| F | Focus mode (Esc to exit) |
| R | Restart from the beginning |
| M | Show / hide controls on small screens |

## Settings

- **Speed:** 120–900 words per minute, with presets.
- **Words at a time:** 1, 2, or 3.
- **Pause at punctuation:** longer pauses at sentence ends, commas, and paragraph breaks.
- **Ease in when I press play:** the first few words after you press play run slower.
- **Highlight the focus letter:** the red letter.
- **Show surrounding words:** a line of context under the word.
- **Remember my place:** reopen the page where you stopped.
- Text size, and light or dark theme (follows your system setting until you change it).

## Run it locally

It is a static page with no build step. Open `index.html` in a browser, or serve the folder:

```sh
python -m http.server 8000
# then open http://localhost:8000
```

When the page is opened as a local file, the browser may block the **Paste text** button. Press Ctrl+V (or ⌘V) in the text box instead.

## Files

| File | Purpose |
|---|---|
| `index.html` | The app: markup, styles, and script |
| `packs-data.js` | Built-in samples (original text and public-domain excerpts) |
| `DISCLAIMER.md` | Comprehension, health, privacy, and content notes |

## Samples

- *Welcome: how to use Flashread* (original)
- *RSVP method primer* (original)
- *The Gettysburg Address*, Abraham Lincoln, 1863 (public domain)
- *Alice's Adventures in Wonderland*, opening of chapter 1, Lewis Carroll, 1865 (public domain)

## Disclaimer

Flashread is a reading aid, provided as is. Comprehension usually drops at high speed, so read important material normally. Take a break if rapid text causes discomfort. See [DISCLAIMER.md](DISCLAIMER.md) for the full notes on comprehension, health, privacy, and content.

## License

MIT. See [LICENSE](LICENSE).
