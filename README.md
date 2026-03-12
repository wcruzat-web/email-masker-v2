# MaskMail ✉️

A clean, premium SaaS-style **email masking UI** built with pure HTML and Tailwind CSS — zero JavaScript, zero dependencies beyond a CDN.

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)
![No JS](https://img.shields.io/badge/JavaScript-none-lightgrey?style=flat)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat)

---

## Preview

> A warm grid-paper background, frosted-glass input card, and a dark terminal-style output panel — all in a single `.html` file.

```
┌────────────────────────────────────────┐
│  ✉  MaskMail   Email Privacy Tool     │
│                                        │
│  Hide your email,                      │
│  keep your privacy.                    │
│                                        │
│  ┌──────────────────────────────────┐  │
│  │  yourname@example.com            │  │
│  └──────────────────────────────────┘  │
│  [       Mask Email       ]            │
│                                        │
│  ┌── masked_output.txt ───────────┐   │
│  │ input  │ yourname@example.com  │   │
│  │        │ ──── masked ───────── │   │
│  │ output │ y*******e@e******.com │   │
│  └────────────────────────────────┘   │
└────────────────────────────────────────┘
```

---

## Features

- **Single file** — everything lives in `email-masking.html`, no build step needed
- **Pure HTML + Tailwind CSS** — loaded via CDN, no JavaScript whatsoever
- **Responsive** — works seamlessly on mobile, tablet, and desktop
- **CSS-only animations** — staggered page load, button hover wipe, blinking caret, scan-line effect on the output panel
- **Premium feel** — Instrument Serif + DM Sans + DM Mono type stack, dark terminal output, dot-grid background, soft blue glow blob

---

## Tech Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 |
| Styling | [Tailwind CSS](https://tailwindcss.com/) (CDN) |
| Fonts | [Instrument Serif](https://fonts.google.com/specimen/Instrument+Serif), [DM Sans](https://fonts.google.com/specimen/DM+Sans), [DM Mono](https://fonts.google.com/specimen/DM+Mono) via Google Fonts |
| JavaScript | **None** |

---

## Getting Started

No install, no build tool, no package manager.


## Design Tokens

| Token | Value | Usage |
|---|---|---|
| Ink | `#1a1a1a` | Primary text, button background |
| Accent | `#2563eb` | Hover fill, output highlights |
| Surface | `#f6f5f1` | Page background |
| Card | `#ffffff` | Input card |
| Terminal | `#0d1117` | Output panel background |
| Border | `#e2e0da` | Input borders |

---

## CSS Animations

All effects are CSS-only using `@keyframes` and Tailwind utility classes:

| Effect | Trigger | Description |
|---|---|---|
| `fadeUp` | Page load | Staggered entrance for each section |
| `btn::after` slide | `:hover` | Blue fill wipes up over the dark button |
| `blink` | Always | Blinking `\|` caret on the masked output |
| `scan` | Always | Subtle scan-line sweeps over the terminal panel |
| `field:focus` | Input focus | Border darkens + soft shadow ring |

---

## Customisation

**Change the accent color** — find and replace `#2563eb` with any hex value.

**Change fonts** — swap the Google Fonts `<link>` and update the three font-family declarations at the top of the `<style>` block.

**Make it functional** — wrap the form in a `<form action="...">` pointing at your backend or add a small JS listener to the button to perform the masking logic client-side.

---

## Future Updates

- [ ] JavaScript masking logic (partial / full modes)
- [ ] Clipboard copy button wired up
- [ ] Dark mode toggle

---

## License

[MIT](LICENSE) — free to use, modify, and ship.

---

<p align="center">Note : Frontend was vibe coded.</code></p>
