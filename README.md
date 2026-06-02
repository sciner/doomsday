# Doomsday Trainer

A lightweight browser trainer for practicing the Doomsday algorithm: given a random date, choose the correct day of the week as quickly as possible.

The project is intentionally simple: a single static `index.html` file with embedded HTML, CSS, and JavaScript. It has no build step, no package manager dependencies, and no backend.

## Features

- Random date generation for day-of-week drills
- Optional fixed-year mode for focused practice
- Text and voice date presentation modes
- Immediate answer validation with the correct weekday highlighted
- Step-by-step Doomsday calculation breakdown
- Reference popup for month anchor dates and century anchors
- Separate 0-27 year-index trainer
- Local attempt history grouped by day and session
- Keyboard shortcuts for faster practice
- Responsive layout for desktop and mobile screens

## Getting Started

Open `index.html` directly in a modern browser.

For local development, you can also serve the folder with any static file server, but it is not required. The app does not need installation or compilation.

## Usage

1. Click **Загадать дату** to generate a new date.
2. Pick the weekday with the buttons or keyboard shortcuts.
3. Review the result and open the calculation details when needed.
4. Use the history section to track recent sessions and daily performance.

Keyboard shortcuts:

- `N` starts a new date
- `1`-`7` answer Monday through Sunday
- `Enter` reveals the answer without selecting a weekday
- `Escape` closes open popups

## Doomsday Method Support

The trainer shows the main parts of the calculation:

- century anchor
- last two digits of the year
- leap-year status
- calculated Doomsday for the year
- month anchor date
- offset from the anchor date
- final weekday

The reference popup includes common anchor dates such as `4/4`, `6/6`, `8/8`, `10/10`, `12/12`, and the mnemonic "I work 9-5 at the 7-11".

## Data Storage

Practice history and user preferences are stored in the browser via `localStorage`.

Stored data stays on the current device and browser profile. Clearing site data or browser storage will remove the history and saved settings.

## Project Structure

```text
.
├── README.md
└── index.html
```

## Browser Requirements

Any current desktop or mobile browser should work. Voice mode depends on the browser's Web Speech API support.

## Notes

The current interface text is in Russian, while this README is written in English for project-level documentation.