# Yuna Yoon · K-beauty pop-up

Landing page for the Yuna Yoon Korean skincare pop-up store (17–18 October 2026):
free skin-test registration, a registration countdown, and a preview of the products and brands we're bringing.

Everything is in one file, `index.html`. No build step.

## Edit the event details

At the top of the `<script>` in `index.html`:

- `REG_CLOSES` – registration deadline (countdown target)
- `SLOTS` – skin-test time slots
- `FORM_ENDPOINT` – where registrations are sent (see below)

Dates, address and products are written in the page text and the `products` / `brands` lists.

## Receiving registrations

The page is static, so it needs a form service to collect sign-ups.
Create a free form on [Formspree](https://formspree.io), copy its URL (`https://formspree.io/f/xxxxxxx`)
and paste it into `FORM_ENDPOINT`. Each registration then arrives by email and in the Formspree dashboard.

## Publish with GitHub Pages

Repository **Settings → Pages → Deploy from a branch → `main` / root**. The site goes live at
`https://<your-username>.github.io/<repo-name>/`.
