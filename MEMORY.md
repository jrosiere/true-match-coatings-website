# MEMORY (website)

Public file: site decisions only, nothing confidential.

## Decisions
- Email opt-in (Nov 24, 2026): unchecked checkbox on the contact form,
  stored in a plain HubSpot contact property `marketing_opt_in` (single
  checkbox) rather than HubSpot's consent block, which needs subscription
  types set up first. Sent only when ticked, so a returning contact who
  opted in before is never switched off. Privacy policy mentions these
  emails.
- Retry without the opt-in on a 400 from HubSpot, because a lost customer
  message costs more than a missed opt-in.

## Log
- Nov 24, 2026: opt-in checkbox merged and live (PR #1). HubSpot property
  `marketing_opt_in` created the same day, and added to the HubSpot form
  (shown in HubSpot as "Website Form") and published that afternoon.

## Open
- Planned pages: before-and-after gallery, a how-to page or two.
- Chip's last name still needed on the Contact page.
