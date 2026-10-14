# GTK Cyber Teleprompter

A single-file browser teleprompter for recording videos. It loads a Markdown script and scrolls it at a steady speed.

## Usage

1. Open `index.html` in a browser. No server or install is needed.
2. Click the file picker or drag a `.md` / `.txt` file onto the page.
3. Press Space to start scrolling.

Keep `logo.svg` next to the HTML file so the logo and favicon load. An internet connection is needed on first load to fetch the Markdown parser (`marked`) from jsDelivr.

## Controls

| Key | Action |
|---|---|
| Space / PgDn / → | Play or pause |
| PgUp / ← | Back up a little |
| ↑ / ↓ | Faster / slower (10 px/sec steps) |
| + / - | Bigger / smaller text |
| M | Mirror the text (for beam-splitter glass) |
| H | Hide or show the top bar |
| Home | Jump back to the start |

Speed, text size, and mirror setting are remembered between sessions in the browser's local storage.

A presentation clicker works as a remote, since most clickers send PgDn/PgUp or the arrow keys.

## Writing scripts

Scripts are plain Markdown. Headings, bold, and lists render as usual, which makes them handy for section markers and emphasis cues. The gold line across the screen marks the reading position.

## License

Apache License 2.0. See [LICENSE](LICENSE).
