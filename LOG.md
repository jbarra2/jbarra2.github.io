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

## 3. Card text

**Asked:**

> Draft the Artifact 1 card: a one-line description, a link, and a short
> reflection on how building the page went.

> Cards 2 through 5 need my own ideas, but I want to brainstorm first. Give me lists and
> I'll keep the ones I like.

> Replace the session-board idea. One card should be Focusqueue: tasks with a
> title, description, due date, and difficulty, plus an optional group. I want
> a view for one group and a view for every task. Easiest tasks with the
> closest due dates come first.

> Another card should be a resale inventory app. My example is a fragrance
> spreadsheet with brand, model, size, buy price, market price, and sale
> price, but the app should work for any product.

> The last card is a home for project ideas. You save an idea, a chat helps
> you turn it into a plan, and it stays until you have time to build it. Theme
> it as a rocket: the idea starts as the base, the plan adds parts, and
> starting the real project is the launch.

> Build sheet needs two modes. One is for before and during the build: parts,
> cost, and install order. The other is for after the build is done, a page
> that shows the finished car, the mods, and the stats.

> Reorder the placeholder cards. Focusqueue is Artifact 2, Stack is Artifact
> 3, and Build sheet is Artifact 5. Leave Resale inventory as Artifact 4.

**What came back / what changed:**

- Filled the Artifact 1 card and pointed it at `https://jbarra2.github.io`.
- Left cards 2 through 5 as placeholders, with these ideas:
  - Artifact 2, Focusqueue: a task queue with optional groups.
  - Artifact 3, Stack: project ideas assembled like a rocket, then launched
    when it is time to build.
  - Artifact 4, Resale inventory: buy, market, and sale prices for any
    product.
  - Artifact 5, Build sheet: a planning mode while the car is being built,
    and a showcase of the finished car, its mods, and its stats.
- Reflections on cards 2 through 5 still say "Not started yet."

## 4. Artifact 2 card

**Asked:**

> Let's fill in the card for focusqueue in our portfolio site

> (answering which layout to use) Only Artifact 1 full width.

**What came back / what changed:**

- Marked the Artifact 2 card done. The idea text is replaced by a short summary of
  the finished app, and the reflection says how the build went and what I learned.
- The link points to the repository on GitHub, `https://github.com/jbarra2/focusqueue`.
  There is no live site on purpose: the app only listens on `127.0.0.1`, so it runs
  on one computer.
- On wide screens every done card spanned both columns, which would have put
  Artifact 2 on its own row. The full-width rule now names `#artifact-1`, so the
  grid stays one wide card, then two rows of two. A done card still gets the warm
  border and full-color text.
- Cards 3 through 5 are unchanged.

## 5. Rename Artifact 3

**Asked:**

> What are some other good names to replace "Stack" for my third artifact? I
> want to keep the same idea but brainstorm a different name

> Launchpad or liftoff?

> Let's change the name to Launchpad please

**What came back / what changed:**

- Claude pointed out that "Stack" also clashes with the card stack in the
  Focusqueue card, then suggested names grouped by theme.
- Claude recommended Launchpad over Liftoff. The card describes a place where
  ideas are assembled and then launched, and a launchpad is that place.
  Liftoff only names the last step.
- Renamed the Artifact 3 card title from Stack to Launchpad. The summary,
  link, and reflection are unchanged, and the card is still a placeholder.
