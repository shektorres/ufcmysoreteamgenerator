# UFC Mysore Matchday Team Generator

A responsive single-page HTML app for organizing UFC Mysore matchday squads, generating balanced teams, tracking scores, recording goalscorers, and reviewing football-style player statistics.

## Live Deployment

GitHub Pages URL:
https://shektorres.github.io/ufcmysoreteamgenerator/

## Project Overview

This project is a static web application built in a single HTML file. It helps a team organizer:

- select which players are available for a matchday,
- generate two balanced teams,
- view a tactical pitch layout,
- manually swap players between teams and the bench,
- record goals and match scores,
- save a match history archive,
- review player career statistics and leaderboard records,
- export a match lineup in WhatsApp-friendly text format.

## Repository Structure

```text
ufcmysoreteamgenerator/
├── index.html
├── WhatsApp Image 2026-09-18 at 16.30.23.jpeg
├── README.md
└── .github/            (if enabled by repo settings)
```

### index.html

This is the main file of the project. It contains:

- the page structure and layout,
- the styling and dark theme,
- the roster and player data,
- the JavaScript logic for generation, scoring, history, and admin controls,
- all modal windows and action handlers.

In other words, the entire application logic is embedded in the HTML file rather than split across separate CSS or JavaScript files.

### WhatsApp Image 2026-09-18 at 16.30.23.jpeg

This image is used as the UFC Mysore logo/header brand in the interface.

### README.md

This file documents the app's purpose, its internal structure, and the deployed project link.

## How the HTML App Works

The app is organized into two main sections:

1. Matchday Setup
2. Scoreboard & History

### 1. Matchday Setup

This section lets the user:

- view the squad attendance list,
- search for players,
- filter by position,
- quickly select players,
- generate balanced Red and Yellow teams,
- inspect the pitch layout,
- swap players manually,
- export the lineup for WhatsApp.

The layout includes:

- a left panel for the attendance checklist,
- a right panel for the tactical pitch and team cards,
- quick team generation controls,
- bench/substitute handling,
- fairness and position balance indicators.

### 2. Scoreboard & History

This section manages match results:

- live score for Red vs Yellow,
- goalscorer tracking,
- match date selection,
- admin score controls,
- a saved match history archive,
- player statistics leaderboard.

This section allows the app to act like a mini team-management and match-recording dashboard.

## Key Functional Features

- Team balancing logic based on selected players and their tiers
- Search and filter for attendance list entries
- Tactical pitch presentation for each team
- Bench pool and player swap functionality
- Match score and goalscorer tracking
- Local browser storage for saved roster and history
- Admin-only controls for roster editing and statistics updates
- WhatsApp export formatting for team lineups
- Player leaderboard with match and goal records

## Internal HTML Structure Summary

The page is built with reusable sections such as:

- Header navigation with app branding and navigation buttons
- Matchday generator section
- Attendance checklist and filters
- Tactical pitch visualization
- Squad cards list view
- Scoreboard panel
- Goalscorer selectors
- Match history archive
- Leaderboard modal
- Admin login modal
- Roster editor modal
- Player stats editor modal
- Export modal
- Confirmation dialog

## JavaScript Logic Included in the HTML

The script embedded at the end of `index.html` contains all app behavior. It handles:

- roster data definitions,
- tier and skill calculation,
- team generation,
- player selection toggling,
- swapping logic,
- match score updates,
- saved results history,
- admin authentication state,
- localStorage persistence,
- modal display controls,
- export-to-clipboard functionality.

## How to Run It

Because this is a static site, you can run it locally in either of these ways:

### Option 1: Open directly

Open `index.html` in a browser.

### Option 2: Serve locally

From the project folder, run:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Deployment

The project is designed for GitHub Pages deployment and can be published directly from the repository root because the main entry file is `index.html`.

Deployed site:
https://shektorres.github.io/ufcmysoreteamgenerator/

## Notes

- The project is currently a static front-end app.
- Data storage is browser-local and not synced across multiple users/devices.
- Admin password logic exists in the client-side code for local demo purposes.
- This is best suited for personal or team-use local management rather than a large multi-user system.

## Summary

This repository is a complete matchday squad generator and team-management HTML app. It combines team generation, score tracking, player records, roster management, and game-history storage in a single-page interface that is easy to run and deploy.
