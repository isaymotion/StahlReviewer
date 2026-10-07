# Psychopharmacology Trainer

A web-based review app for psychiatry residents covering Chapters 1–13 of *Stahl’s Essential Psychopharmacology*, 5th edition. Its content comes from the 13 chapter study-guide slide decks and the cumulative review deck.

This app was created by Isabella Navarro, MD. Latest version October 2026. isaymotion@gmail.com

## Features

- **Flashcards:** 208 self-test cards (16 per chapter) with spaced repetition. Cards move through six boxes; missed cards repeat within the session.
- **Quiz:** 24 board-style questions with explanations, card-based multiple choice, and abbreviation drills. Filter by chapter, choose 10, 20 or 40 questions, and retry the ones you missed.
- **Study notes:** every content slide from the 13 decks (about 620 notes), with clinical links, comparison tables and figure references. Searchable within a chapter or across all chapters.
- **Atlas & drugs:** the neurotransmitter atlas, drug-by-drug quick reference and high-yield review from the cumulative deck.
- **Glossary:** about 300 abbreviations and terms, filterable by chapter and quizzable.
- **Dark mode:** the moon/sun button in the top bar switches between light and dark. The choice is remembered, and by default the app follows the device setting (About & progress also offers Light, Dark or Match device).
- **Back and forward:** arrow buttons in the top bar step through the pages you have visited, return you to where you were scrolled, and are greyed out when there is nowhere to go. The browser’s own back/forward buttons and `Alt`+`←`/`→` work the same way.
- **Progress:** mastery and quiz accuracy by chapter and a study-day streak, with export, import and reset.

Progress is saved in each user’s own browser (localStorage). No accounts, servers or tracking.

## Files to upload

Upload all of these to the root of the repository:

| File | Purpose |
| --- | --- |
| `index.html` | The app |
| `manifest.webmanifest` | Lets phones add the app to the home screen |
| `icon.svg` | Brain icon, vector master and browser tab icon |
| `favicon.ico`, `favicon-32.png` | Browser tab icons for older browsers |
| `apple-touch-icon.png` | iPhone and iPad home-screen icon |
| `icon-192.png`, `icon-512.png` | Standard app icons (`icon-512.png` also works as the repository image) |
| `icon-maskable-512.png` | Android home-screen icon with extra padding for round or squircle masks |
| `README.md` | This file |

## Publish on GitHub Pages

1. Create a new public repository on GitHub.
2. Upload the files listed above to the root of the repository.
3. In the repository’s **Settings → Pages**, set the source to deploy from the `main` branch, root folder.
4. After a minute or two, the app is live at `https://<your-username>.github.io/<repository-name>/`.

The app is a single `index.html` plus the icon files, with no build step. It loads two Google Fonts and falls back to system fonts if they are unavailable. Opening `index.html` directly in a browser also works (the home-screen install needs the published site).

## Keyboard shortcuts

- **Flashcards:** `Space` reveals the answer; `1` marks it missed, `2` marks it known.
- **Anywhere:** `Alt`+`←` goes back and `Alt`+`→` goes forward.
- **Quiz:** `A`–`D` answer the question; `Enter` goes to the next one.

## Source and disclaimer

Content summarizes Stahl SM, *Stahl’s Essential Psychopharmacology*, 5th edition (Chapters 1–13), for educational use. It is a study aid, not a substitute for the book or for clinical judgment. Confirm doses and prescribing details in current references before clinical use.
