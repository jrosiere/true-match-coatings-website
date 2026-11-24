# True Match Coatings website

Public site for truematchcoatings.com. This repo is public and GitHub Pages
serves every file in it (there is a `.nojekyll`), so this file and
MEMORY.md are publicly readable too: keep them to how the site works. No
business plans, prices, customer data, formulas or secrets here; those live
in the private `TrueMatchCoatings` repo.

## How it's built
- Plain HTML/CSS, no build step. Pages share `style.css`; copy the header
  and footer from an existing page when adding one.
- Merging to `main` publishes the site within a minute or two. Every change
  goes through a pull request the owner approves before it's merged.

## Contact form
- `contact.html` posts straight to the HubSpot Forms API (v3 integration
  submit) for the form "Contact form 10-13-26" (shown in HubSpot as
  "Website Form"). `marketing_opt_in` is on that form. Field names must match
  HubSpot contact property internal names.
- Fields sent: firstname, lastname, email, phone (if given),
  `what_s_this_about_`, message, and `marketing_opt_in` = true only when the
  "Send me product news and specials" box is ticked.
- If HubSpot rejects a submission (HTTP 400) that included the opt-in, the
  script resends it without the opt-in so the message is never lost.

## After working on this repo
Update this file and MEMORY.md with what changed, and add a line to the
private TrueMatchCoatings repo's MEMORY.md too.
