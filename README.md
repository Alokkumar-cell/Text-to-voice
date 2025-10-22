# Text-to-voice

A minimal browser-based Text-to-Speech demo that uses the Web Speech API.

- Open [index.html](index.html) in your browser to run it.
- Styling is in [index.css](index.css).
- Logic is in [index.js](index.js) (creates the [`speech`](index.js) utterance and calls the Web Speech API).

## Usage

1. Open [index.html](index.html) in a modern browser (Chrome, Edge, Firefox).
   - From the dev container you can run a simple server and open it, e.g.:
     - Python 3: python -m http.server 8000
     - Then open http://localhost:8000 in your browser.
2. Type some text into the textarea.
3. Click the "Listen" button to have the browser speak the text.

## How it works

- The page creates a SpeechSynthesisUtterance (`[`speech`](index.js)`) and on button click sets `speech.text` from the textarea value, then calls `window.speechSynthesis.speak(speech)` to play the audio.

## Notes

- Requires a browser with the Web Speech API enabled.
- No server-side code; purely client-side static files.

## Files

- [index.html](index.html) — markup and controls.
- [index.css](index.css) — styling.
- [index.js](index.js) — speech logic.

## License

Unlicensed — feel free to adapt for your needs.