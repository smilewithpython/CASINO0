# Felt & Bone — Casino

Craps, Blackjack, and Video Poker in one mobile app, with a private **luck console** you control from the settings (⚙) menu.

## What's inside
- `index.html` — the whole game
- `manifest.json` — makes it installable as an app
- `service-worker.js` — lets it run offline
- `icon-192.png`, `icon-512.png` — home-screen icons

## Put it on your phone (GitHub Pages)

1. Create a new repo on GitHub (e.g. `felt-and-bone`).
2. Upload **all the files in this folder** to the repo (drag them into the GitHub web uploader, or push with git).
3. Go to **Settings → Pages**.
4. Under "Build and deployment", set **Source: Deploy from a branch**, branch **main**, folder **/ (root)**. Save.
5. Wait ~1 minute. GitHub shows a URL like `https://yourname.github.io/felt-and-bone/`.
6. Open that URL **on your phone**.
   - **iPhone (Safari):** Share button → *Add to Home Screen*.
   - **Android (Chrome):** menu (⋮) → *Install app* / *Add to Home screen*.
7. Launch it from the home-screen icon — it opens fullscreen, no browser bars, and works offline.

> Note: Pages must be served over **https** (GitHub does this automatically) for the offline/installable features to work. Opening the file directly from your files app won't enable them.

## The luck console (⚙ settings)
- Each game has its own slider, **0–10**. **5 = a fair, true-odds game.**
- Above 5 bends outcomes in your favor; at **10** the table can barely beat you (~99% favorable).
- Below 5 bends them against you.
- A master toggle turns the whole console off for pure fair odds.

## House & dealers
- You play against the **House bankroll** (default $4T) — set it to anything in settings. Your winnings come out of it; your losses feed it.
- In Blackjack you face a named dealer. Beat one enough and the pit swaps in a **tougher** dealer. **Bust a dealer** and they're replaced by a new one with **random luck (25%–65%)**.
- No matter how sharp a dealer is, cranking your Blackjack slider to 10 always lets you overcome them.

## Saving
Everything (bankrolls, luck settings, dealer, stats) saves automatically in your browser and survives closing the app.

## Reset
Settings → **Reset Everything** restores defaults.
