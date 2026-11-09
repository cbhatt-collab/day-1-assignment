# Comic Deck: Salesforce, or Any Topic You Like

A comic-book style slide deck in a single HTML file. It starts out about Salesforce. Type in any other topic and Google Gemini rewrites every slide about it. There's a built-in chat bot you can ask questions, and a playable Pong game at the end.

There's nothing to install or build. Download the file and open it in a browser.

## Quick start

1. Open `salesforce-deck.html` in a modern browser (Chrome, Edge, Safari or Firefox).
2. Press **→** to move through the slides.
3. Optional, for the AI features: paste a Gemini API key into the **🔑 Gemini API key** box on slide 1. You can get a free key from [Google AI Studio](https://aistudio.google.com/apikey).

## Features

| Feature | What it does |
| --- | --- |
| **AI deck generator** | Enter a topic on slide 1 and click **Generate**. Gemini rewrites every slide about that topic. A progress bar follows the work slide by slide. |
| **Chat bot** | Click 💬 (or press **C**) and ask anything. When the slides are relevant, the answer cites them, and clicking a citation such as "Slide 4" jumps to that slide. |
| **Inline editing** | Click **✏️ Edit**, then click any text to change it. Click **💾 Save** to keep your changes. **↺** puts back the original Salesforce content. |
| **5 themes** | Cloud Comic, Midnight Neon, Retro Pop, Emerald Jungle and Noir & Gold. |
| **Slide sorter** | Move the mouse to the left edge to open it. Drag one card onto another to swap the two slides. Tick **Skip** to leave a slide out of the show. |
| **Cloud Pong** | The last slide is a Pong game against a bot, with three difficulty levels. |

## Keyboard shortcuts

| Key | Action |
| --- | --- |
| `→` `Space` / `←` | Next / previous slide |
| `Home` / `End` | First / last slide |
| `F` | Fullscreen |
| `S` | Slide sorter |
| `T` | Theme picker |
| `E` | Edit mode (`⌘/Ctrl + S` saves) |
| `C` | Chat bot |
| `Esc` | Close a panel or leave edit mode |
| `↑` `↓`, `Space` | Pong: move the paddle, start or pause the game |

## Privacy and your API key

- Your Gemini key, your edits, the generated content, the theme and the slide order are all saved in your browser's local storage. None of it is saved in the HTML file.
- The key is sent only to Google's Gemini API (`generativelanguage.googleapis.com`), directly from your browser. The key is stored as plain text in the browser, so use it on your own devices only.
- The AI features use the `gemini-3.5-flash-lite` model. To switch models, change `GEMINI_MODEL` in the script near the end of the HTML file.

## Files

| File | Contents |
| --- | --- |
| `salesforce-deck.html` | The whole app: HTML, CSS and JavaScript in one file, with no dependencies apart from Google Fonts |
| `salesforce.md` | The Markdown overview of Salesforce that the deck was built from |
| `prompts.md`, `prompts2.md` | The prompts used to build this project with Claude Code |
| `_redirects` | Tells Netlify to serve the deck at the site's root URL |
