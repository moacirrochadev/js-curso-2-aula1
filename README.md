# js-curso-2-aula1

Simple demo project for a JavaScript course (aula 1). Contains a small web page and a JS game example.

## Project structure

- `index.html` — main HTML page for the demo
- `app.js` — main JavaScript for the demo
- `style.css` — main stylesheet
- `img/` — images and an extra `JS Game.html` demo inside `img/JS Game.html` with its own `app.js` and `style.css` in `img/JS Game_files/`

## Description

This repository is a lightweight starter for practicing DOM manipulation, styling and small JavaScript games. It appears to be part of a course exercise; the code is intentionally simple so students can read and modify it.

## How to run

The project is static — you can open `index.html` directly in a browser, or serve the folder with a simple HTTP server (recommended to avoid some browser restrictions).

Using Python (if installed):

```powershell
# run from the repository root
python -m http.server 8000
# then open http://localhost:8000 in your browser
```

Or, simply double-click `index.html` in your file explorer to open in your default browser.

## Notes

- If you edit files, refresh the browser to see changes.
- There is an extra game demo in `img/JS Game.html`. Its resources are in `img/JS Game_files/`.
- This repository doesn't have a build step or dependencies.

## What `app.js` does

`app.js` implements a simple "secret number" guessing game used by the demo page. High-level behavior:

- Generates a secret number between 1 and 10 and avoids repeating generated numbers until all values have been used.
- Shows messages by updating the page `h1` and `p` elements and speaks messages using `responsiveVoice.speak` (Brazilian Portuguese).
- Reads the player's guess from an `input` element and checks it with `verificarChute()`; provides hints (higher/lower).
- Tracks attempts and enables a `reiniciar` button when the user guesses correctly.
- Main functions: `exibirTextoNaTela`, `exibirMensagemInicial`, `verificarChute`, `gerarNumeroAleatorio`, `limparCampo`, `reiniciarJogo`.

## Author

Repository owner: `moacirrochadev`.