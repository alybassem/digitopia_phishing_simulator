# محاكي التصيّد العربي — Arabic Phishing Simulator

A browser-based cybersecurity awareness game that trains users to recognize phishing attempts in Arabic — emails, SMS messages, and phone calls modeled on real-world scenarios relevant to Egypt and the wider Middle East (banks, telecoms, e-commerce, prize scams, etc.).

Built for **Digitopia 2025**, Egypt's national digital innovation competition (Ministry of Communications and Information Technology), where the project advanced past the initial idea-screening stage into the prototype development round.

## What it does

- Presents the player with a series of realistic messages (email / SMS / phone call)
- The player decides whether each one is legitimate or a phishing attempt
- After each answer, a detailed Arabic-language explanation shows exactly what gave it away (a suspicious domain, an urgency tactic, a request for sensitive info, etc.)
- Tracks score, progress, and lets the player review their mistakes at the end
- Fully right-to-left (RTL) layout with Arabic typography (Cairo / Changa fonts)

## Tech stack

Plain **HTML, CSS, and JavaScript** — no frameworks, no build step. Runs entirely in the browser.

## Running it locally

No installation needed — just open `homepage.html` in a browser, or serve the folder with any static file server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000/homepage.html`.

## Project structure

```
index.html     — landing page
learnmore.html     — "learn more" info page
simulation.html    — the quiz/game itself
scenarios.js        — all phishing/legit message scenarios + game logic
styles.css          — shared styles for the simulation screen
```

## Deployment

Includes a GitHub Actions workflow (`.github/workflows/static.yml`) to auto-deploy to GitHub Pages on push to `main`.

## Disclaimer

Built strictly for educational purposes. No real links, credentials, or user data are collected or transmitted.
