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
