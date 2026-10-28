# Canva Design Master Class: sales page

Single-page site for The Elevation Citadel's Canva Design Master Class with The Elevated James (16–17 Nov 2026, online on Google Meet).

## What is here

- `index.html`: the whole page (HTML, CSS and a small script). No build step, no dependencies beyond Google Fonts.
- A countdown timer that starts at midnight on 26 Oct 2026 (IST) and runs to the first session on 16 Nov 2026 at 21:00 IST.

## Changing the countdown

The two dates sit at the top of the `<script>` block in `index.html`:

```js
var START = Date.parse('2026-10-26T00:00:00+05:30');  // timer start
var EVENT = Date.parse('2026-11-16T21:00:00+05:30');  // first session, 9:00 PM IST
```

If the session time changes, update `EVENT` and the "9:00 PM IST" wording on the page.

## Before going live

- Point every "Reserve my seat" button (`href="#register"`) at the registration or payment link.
- Confirm the Canva Pro bonus terms, or remove the bonus block.
- Replace the session time placeholder ("To be announced") when it is decided.
