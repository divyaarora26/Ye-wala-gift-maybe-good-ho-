# Blocky Heart — Valentine's Day Interactive (HTML/CSS/JS)

A small romantic interactive web project built with only HTML, CSS, and JavaScript. No external libraries.

Overview
- A stylized, blocky / voxel-inspired heart inspired by a human heart silhouette.
- Gentle heartbeat animation.
- Click (or press Enter/Space when focused) the heart to split it — a glow appears and the first message fades in.
- Click "Next" to reveal a love letter typed line-by-line inside a soft, glowing card.
- Many falling flowers animate while the love letter appears.
- Responsive and mobile-friendly.

Files
- `index.html` — main page
- `style.css` — styles and animations
- `script.js` — interactive behavior, heart building, typing, and flower generation
- `README.md` — this file

Usage
- Open `index.html` in a modern browser (Chrome, Firefox, Edge, Safari).
- Click or keyboard-activate the heart to begin the interaction.

Customization
- Edit the following values in `script.js` at the top to change the displayed texts:

  - `FIRST_MESSAGE_TEXT` — the short centered message shown immediately after the heart splits.
  - `LOVE_LETTER_LINES` — an array of strings. Each string becomes a separate line in the love letter and will be typed line-by-line.

- Alternatively, you can change texts at runtime from the console:
  - `Valentine.setFirstMessage("New message")`
  - `Valentine.setLetterLines(["Line 1", "Line 2"])`

Styling
- Colors, sizes, and blockiness are controlled in `style.css`.
- Adjust `--cell-size` in the `:root` selector to change the pixel block size used for the heart.
- The heart pixel map is in `script.js` as `HEART_MAP`. You can edit that array to reshape the block heart (it's an 11x11 matrix; `0` means empty, `1/2/3` control shade).

Notes & Tips
- All assets are generated in the DOM — no images or external fonts are used to keep the project self-contained.
- The project is designed with accessibility in mind: the heart is keyboard-focusable.
- For very slow devices, reduce the number of concurrently spawned flowers by modifying `startFlowers()` in `script.js`.

License & Attribution
- This small project was provided as a code gift. Feel free to adapt and personalize it for your Valentine.
- No external libraries or resources are used.

Enjoy — and Happy Valentine's Day!