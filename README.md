# Paradrop

A standalone build of the **HOT Drop Rush Mini-Game** (Paradrop internally), originally published as a
limited-time promotional event on the PUBG website
(`https://pubg.com/en/events/hotsummerdrop`).

## What this is

- The game client (`paradrop-game.js`) and its assets were pulled from the PUBG event site.
- The event was time-limited, so the original backend (round start/link/submit/revoke,
  leaderboards, etc.) will be (or is) no longer available.
- To keep the game playable, this thing:
  - Loads all art, audio, and fonts from local files (`./assets`, `./fonts`) instead
    of the CDN(`pubgwebgame-sdk-test.sisyphusbot.com`).
  - Stubs the game-data API in `index.html` so that game can start and run a round without a server.

> Note: Scores are not submitted anywhere and there is no leaderboard.

## Files

| Path                | Description                                           |
| ------------------- | ----------------------------------------------------- |
| `index.html`        | Entry point. Contains the API stub and boots the game |
| `paradrop-game.js`  | The game                                              |
| `assets/`           | Images, spritesheets, audio.                          |
| `fonts/`            | Fonts                                                 |

## Running in a browser

Open [remtrik.github.io/paradrop](https://remtrik.github.io/paradrop/).

## Running as a desktop app (Electron)

A standalone Windows executable is provided in releases - just
double-click to play. No installation required.

## Disclaimer

This project is an unofficial, extracted copy kept for preservation/education.

All game assets and code belong to their respective owners (PUBG / KRAFTON and the event
operator). The original event was a limited-time promotional event and will be (or is) no longer officially
served.
