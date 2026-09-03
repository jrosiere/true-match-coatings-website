# True Match Coatings — Website

Public site repo only — no business documents, formulas, or trade-secret
content. That stays in the separate private `TrueMatchCoatings` repo.

## Structure

- `index.html` — Home
- `contact.html` — Contact (address + team directory)
- `style.css` — shared styles for the whole site

Built as plain HTML/CSS on purpose: no build step, no framework, so adding
a new page later is just a new `.html` file that links to `style.css` and
copies the `<header>`/`<footer>` markup from an existing page. Add new nav
links to the `<nav class="site">` block in each page as new sections
(Services, Gallery, About, etc.) get built out.

## Updating content

Edit directly, or hand new content/direction to Claude to extend — nothing
here requires a build process, just upload the changed files.

## Known follow-ups

- Chip's last name is still needed — currently listed as "Chip" only on
  the Contact page.
- Steve Schmidt's phone/email are live; confirm his listed title ("Sales")
  is what he wants publicly.
