# Build Log

A running record of what I asked the chat AI for and what changed.

**Chat AI used:** Claude

---

## 1. Page structure

**Asked:**

> I need a single-page portfolio for a class assignment. It needs a short
> "about me" section and five cards, one per course artifact. Each card needs a
> title, a link, and a short reflection. What's the simplest HTML structure that
> makes the cards easy for me to edit later?

> Should I use a framework, or plain HTML/CSS/JS?

**What came back / what changed:**

- Claude suggested plain HTML, CSS, and JS since the site is static and small.
  No build step means GitHub Pages can serve it directly.
- Created `index.html` with a header, an about section, and five `<article>`
  cards that share one structure.
- Each card has a `data-status` attribute (`done` or `placeholder`) so I can
  style finished and unfinished cards differently without changing the markup.
- Added an HTML comment above the cards explaining how to edit one.
- Name and bio are marked `TODO` / "Your Name" until I fill in real text.

## 2. Dark theme

**Asked:**

> Can you style this as a minimal dark page? Keep it readable, and make the
> finished card look different from the placeholder cards so I can tell them
> apart at a glance.

> The page is short. Do I still need the About and Artifacts links in the
> header, or can I drop the header entirely?

**What came back / what changed:**

- Added `css/styles.css`: dark background, light text, one warm accent color
  for links, and a two-column card grid on wider screens.
- The Artifact 1 card spans the full width and has a slightly warmer border.
  Placeholder cards use muted text.
- Removed the header. About and Artifacts were only in-page jumps, and the
  whole page fits in a short scroll.

