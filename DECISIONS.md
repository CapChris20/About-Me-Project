# Architecture Decision Records — About Me Project

This was a first web project (*"CODE ONE — 1st Project"*): a multi-page static site about Chris (socials, favorite movies, shows, sports teams, artists, food, family, education and lyrics), written in plain HTML with one stylesheet.

These records were reconstructed from the HTML/CSS files in this repo.

---

# ADR-001: Plain multi-page HTML + one CSS file

## Context
The goal was to learn HTML structure, links and basic CSS by building a personal page.

## Alternatives Considered
- **Site builder (Wix/Squarespace)**: A faster result, but you learn nothing about code.
- **React or another framework**: Premature before learning HTML and CSS fundamentals.

## Decision
One HTML file per topic (`movies.html`, `shows.html`, `sportsteams.html`, `artists.html`, `food.html`, `fam.html`, `education.html`, `lyrics.html`), linked from `index.html` and sharing `style.css`. There's no JavaScript and no build step.

## Rationale
It's the simplest possible stack, so every line is something being learned.

## Tradeoffs
- **Gained:** a solid grounding in HTML and CSS basics.
- **Cost:** the header and navigation are copied into every page. The layout relies on `<br>` and `<hr>` instead of CSS spacing. There are no media queries, and the README links to `127.0.0.1:5500` (a local Live Server URL), not a deployed site.

## What I'd Change
Use semantic elements (`<nav>`, `<section>`), use CSS flex/grid instead of `<br>` spacing, set a meaningful `<title>`, and deploy to GitHub Pages so the README link works.

## Measurement
- 9 HTML pages and 1 stylesheet, about 363 lines in total.
- `background.jpg` is 480 KB.

---

# ADR-002: No backend, storage, authentication or payments

## Decision
Purely static content.

## Rationale
Nothing to store or protect.

## Tradeoffs
None.

## What I'd Change
Nothing. Later projects (Final CW Portfolio, the 3D portfolio) build on this.

## Measurement
Not applicable.
