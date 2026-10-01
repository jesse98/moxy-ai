# Moxy AI

A compact, four-page creator website for Moxy. Static HTML, CSS and JavaScript, hosted with GitHub Pages.

## Pages

- Home: creator portrait and brand introduction.
- How it works: accessible Chat / Remember / Earn tabs, illustrative phone conversation, FAQ.
- Earnings: interactive USD monthly gross fan-spending calculator. Assumptions are illustrative; no creator payout split is implied.
- Get started: accepts an existing creator invitation code or approved dashboard signup URL; creator login and a Moxy invitation request link.

## Editing

`build.py` produces the four HTML pages. Edit the templates then run `python3 build.py`. Shared styling and interactions are in `styles.css` and `app.js`. GitHub Pages serves the repository root from `main`; no build dependencies are required.

## Integration notes

Public creator login is `/creator/moxy/login` on the existing dashboard. Signup requires a valid Moxy agency invitation to preserve attribution. The site does not create accounts itself, issue invitations, store form input, or send emails. The request-invitation link opens the creator's mail app. Invitation validity and agency association are checked by the dashboard.

The calculator uses audience × monthly join rate × payer rate × USD spend per paying fan. It estimates gross fan spending, not creator take-home pay. No earnings guarantees or unverified performance claims.

## Assets

Logo: supplied Moxy AI SVG from the developer pack, used intact with teal AI and city lettering. The hero is an AI-generated fictional adult creator holding a phone, not an existing Moxy creator or testimonial. The entire image is contained so the head and phone remain visible. Satoshi is loaded from Fontshare with a system sans-serif fallback. Demo conversations are scripted and labelled.

Visual direction: centered hero, compact creator and interactive conversation composition, diffuse white glows on black, translucent surfaces, white pill actions. Em dashes are excluded from site copy.
