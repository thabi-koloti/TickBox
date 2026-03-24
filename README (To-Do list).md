# task.

A minimal, persistent to-do app that runs entirely in your browser — no installation, no server, no dependencies.

![screenshot placeholder](screenshot.png)

---

## Features

- **Create** tasks with a priority level (high / medium / low)
- **Edit** tasks inline by hovering and clicking the pencil icon
- **Complete** tasks with a single click — struck through and tracked
- **Delete** tasks individually or clear all completed at once
- **Filter** by All, Active, Done, or High priority
- **Persistent** — tasks are saved to `localStorage` and survive page refreshes
- Live progress bar and stats (total / done / remaining)

---

## Getting Started

No installation required.

1. Download `todos.html`
2. Open it in any modern browser

```
open todos.html
```

That's it.

---

## Usage

**Adding a task**
Select a priority from the dropdown, type your task, then press `Enter` or click `+ Add`.

**Editing a task**
Hover over a task to reveal the edit button (✏). Click it, make your changes, then press `Enter` to save or `Escape` to cancel.

**Completing a task**
Click the checkbox on the left side of any task to toggle it done/undone.

**Deleting a task**
Hover over a task and click the trash icon on the right.

**Filtering**
Use the `All / Active / Done / High` buttons to filter the list.

---

## Data Storage

All tasks are stored in your browser's `localStorage` under the key `tasky_v1`. Data is private to your device and browser — nothing is sent to any server.

To reset all data, open your browser's developer console and run:

```javascript
localStorage.removeItem('tasky_v1');
location.reload();
```

---

## Browser Support

Works in any modern browser (Chrome, Firefox, Safari, Edge). No polyfills needed.

---

## License

MIT — do whatever you like with it.
