# Canva Design Master Class: sales page

Single-page site for The Elevation Citadel's Canva Design Master Class with The Elevated James (9–10 Nov 2026, online on Google Meet).

## What is here

- `index.html`: the whole page (HTML, CSS and a small script). No build step, no dependencies beyond Google Fonts.
- A countdown timer that starts at midnight on 26 Oct 2026 (IST) and runs to the first session on 9 Nov 2026 00:00 IST.

## Changing the countdown

The two dates sit at the top of the `<script>` block in `index.html`:

```js
var START = Date.parse('2026-10-26T00:00:00+05:30');  // timer start
var EVENT = Date.parse('2026-11-09T00:00:00+05:30');  // first session
```

Once the session time is announced, set `EVENT` to the exact start time, for example `2026-11-09T19:00:00+05:30`.

## Before going live

- Point every "Reserve my seat" button (`href="#register"`) at the registration or payment link.
- Confirm the Canva Pro bonus terms, or remove the bonus block.
- Replace the session time placeholder ("To be announced") when it is decided.
