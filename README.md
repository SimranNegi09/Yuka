# Yuka 🌷

A small, mood-based comfort app for the moments when you need a little pause. Pick how you feel, get a short, gentle activity, and check out when you're done. No sign-up, no account, no tracking.

**Live demo:** https://YOUR-USERNAME.github.io/Yuka/

> Yuka is a self-care companion, not a replacement for professional mental health support.

## What it does

You choose a mood, and Yuka offers short guided activities for it.

| Mood | Activities |
|---|---|
| **Comfort** | Affirmations and pep talk, flowers, a bunny hug, memories, a note to future me |
| **Calm** | Five senses grounding, thought dump, guided meditation |
| **Distraction** | Doodle, word scramble, word search, memory match, slide puzzle, quiz |
| **Let It Out** | Name the feeling, leave it behind, write a letter |

Other touches:
- **Note to Future Me:** an optional sealed envelope you can write for a harder day and open later.
- **Gentle check-out:** two soft questions when you leave, asking if you feel a bit more settled. There is no score and no streak.
- **Help when it's needed:** Tele-MANAS (14416, India) is shown on the Let It Out screens.

## Privacy

- Nothing you write is sent to a server. There is no backend.
- Notes to your future self are stored only in your own browser (`localStorage`). You can delete them at any time from the app.
- No accounts, analytics, ads or cookies.
- The only external request is Google Fonts, used for typography.
- A "Privacy & about" page inside the app explains this in plain language.

## Design

- Mobile-first, responsive layout.
- Soft butter-yellow and moss-green palette, with Unbounded, Caveat and Montserrat typefaces.
- Short, simple flows with large tap targets (minimum 38px).
- Heading colors checked for readable contrast.

## Tech

- A single `index.html` file with plain HTML, CSS and vanilla JavaScript. There are no frameworks, no build step and no dependencies.
- A hash-based router (`#home`, `#mood-…`, `#do-…`, `#checkout`, `#privacy`).
- The bunny is built from layered images animated with CSS (waving, hugging, ear twitches).
- Tested with headless Chromium (Playwright) across all screens and activities.

## Run it locally

Download `index.html` and open it in a browser. That's all.

## Product notes

- **Problem:** many wellbeing apps ask for sign-ups, streaks and engagement. Someone having a hard moment needs something quiet, quick and private.
- **Approach:** collect nothing, keep every experience short, and end with a gentle check-out instead of a metric.
- **Known limits:** it needs a connection for the first load (fonts), it has no service worker for full offline use yet, and notes live on one device only.
- **Possible next steps:** make it an installable PWA with offline support, self-host the fonts, and add more activities.

## Credits

Designed and built by **Simran Negi**.
The bunny, game stickers and envelope are original illustrations made for this project. Some other imagery is used for portfolio and demonstration purposes only, and this project is not for commercial use.
