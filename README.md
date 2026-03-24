# task. 

> *"The secret of getting ahead is getting started."*

A personal to-do app that lives in a single HTML file. No installation, no server, no account. Just open it and go.

---

## What it does

Every time you open it you get a time-aware greeting, today's date, and a rotating daily quote to kick off your day. Your grocery and recurring tasks are already waiting for you on first launch — ready to check off as you go.

---

## Features

- **Daily greeting** — Good morning / afternoon / evening based on the time, with today's date
- **Daily quote** — rotates through 10 motivational quotes, one per day
- **Pre-loaded groceries** — 5 recurring grocery tasks seeded on first open
- **Priorities** — tag every task as high, medium, or low
- **Filters** — view All, Active, Done, or High priority tasks
- **Inline editing** — hover any task and click ✏ to edit in place
- **Progress bar** — live tracker of how much you've completed today
- **Persistent** — everything saves to `localStorage`, survives refreshes and restarts

---

## Getting started

No install needed. Just download and open.

```
open tickbox.html
```

Works in Chrome, Firefox, Safari, and Edge.

---

## Customising it

All the personal bits live at the top of the `<script>` tag and are easy to change.

**Change the quotes** — edit the `QUOTES` array. Each entry takes a `text` and an `author`.

**Change the pre-loaded tasks** — edit the `GROCERIES` array. Each entry takes a `text` and a `priority` (`"high"`, `"medium"`, or `"low"`). These only seed once on first open — delete the `tasky_seeded` key in localStorage to re-seed.

**Change the colour scheme** — edit the CSS variables at the top of the `<style>` tag. The gold accent is `--accent: #e8c547`.

---

## Resetting your data

Open the browser console (`F12` → Console) and run:

```javascript
localStorage.clear();
location.reload();
```

This wipes all tasks and re-seeds the grocery defaults on next load.

---

## License

MIT — do whatever you like with it.
