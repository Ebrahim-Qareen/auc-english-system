# AUC English System

Interactive self-study site for the AUC continuing-education English course
*English for Effective Communication*.

**Live site:** enable GitHub Pages on this repository (Settings → Pages → Branch: `main`, folder: `/root`)

## Structure

```
index.html            home page — choose A2A or A2B
a2b/
  index.html          A2B level page — all 12 sessions
  session-1..5.html   study pages
  kahoot-session1..5.html
  media/session-1/    audio, video, slide images
a2a/                  (coming next)
```

## Each session page contains

Recap · Listening · Vocabulary flashcards · Idioms · Grammar · Reading ·
Speaking · Roleplay · Email · Writing · 20-question quiz · Cheat sheet ·
Notes · Progress tracker

Progress, notes, and quiz scores are saved in the browser using `localStorage`
(prefix `s1_`–`s12_`, and `kahoot_sN_lb` for the Kahoot leaderboards).

## Media

Slide decks, deep-dive audio, and overview videos are generated from the course
material and stored under `a2b/media/session-N/`.

Third-party videos are embedded from YouTube rather than hosted here.

To move media to a CDN later, change the single `MEDIA_BASE` constant near the
bottom of each session page — no other paths need editing.
