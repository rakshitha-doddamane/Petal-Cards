# Petal Cards 🌿

An aesthetic flashcard app inspired by vintage botanical affirmation cards. Add cards by typing, speaking or scanning a picture, then study them with spaced repetition and watch your progress grow.

**Live demo:** `https://<your-username>.github.io/Petal-Cards/`

## Features

**Make cards**
- Type a front and an optional back, with tags and a hint
- **Speak** your text with the browser's voice recognition (English, Kannada, Hindi)
- **Scan a picture** and extract the text with OCR ([Tesseract.js](https://github.com/naptha/tesseract.js)), all in the browser
- **One card per line:** write `question :: answer` per line and create many cards at once
- Edit any card, mark favorites, search by text or `#tag`

**Organise**
- Folders and subjects (for example Security+ › Networking), with rename and delete
- Import and export **CSV** (`folder, subject, front, back, tags, hint`) and a full JSON backup

**Study**
- Study mode with 3D flip, hints, and four ratings (Again, Hard, Good, Easy) that show the next review gap
- **Spaced repetition:** a simplified SM-2 scheduler sets each card's next review date
- Missed cards are collected so you can review them again at the end of a session
- Keyboard shortcuts: `Space` flip, `1-4` rate, `H` hint, `Esc` exit

**Progress**
- Dashboard with cards due, day streak, daily goal, 7-day accuracy, a weekly activity chart and mastered cards
- Day (paper) and Night (garden) themes

Everything is saved in your browser (`localStorage`). Nothing is sent to a server.

## Not included yet
Accounts and cloud sync, AI card generation and payments are not built. They would need a backend and are not in this version.

## Run it
No build step. Host it with GitHub Pages (Settings → Pages → Deploy from branch → `main` / root).

> Voice input works in Chrome, Edge and Safari, and needs `https` or `localhost`. It will not work if you double-click `index.html` (a `file://` address). To test locally, run `python -m http.server` in the project folder and open `http://localhost:8000`.

## Tech
HTML, CSS and vanilla JavaScript in a single file, the Web Speech API, and Tesseract.js.
