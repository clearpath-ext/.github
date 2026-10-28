# ClearPath brand assets

The **C-path mark** is the official ClearPath logo: a C that starts at a dot and opens onto a forward chevron, a path from where you are to where you're going. It's used for the extension icon, the website ([clearpathext.com](https://clearpathext.com)), and the GitHub org. Use these files rather than redrawing it.

<p align="center"><img src="clearpath-icon.svg" width="110" alt="ClearPath logo"></p>

## Logo

| File | What it's for |
| --- | --- |
| `clearpath-mark.svg` | **Master.** The mark on its own, transparent, sharp at any size. Works on navy and on white. Edit this file (and `clearpath-icon.svg`), then regenerate everything else. |
| `clearpath-icon.svg` | **Icon master.** The mark centred on the navy rounded tile. Favicons, the extension icon, avatars. |
| `clearpath-mark.png` | Transparent PNG (465×512) for places that can't take SVG. |
| `clearpath-icon-1024.png`, `clearpath-icon-512.png` | Large icon renders (store listings, app launchers). |
| `clearpath-avatar-500.png` | Full-bleed square on navy for avatars that apply their own rounding (GitHub org, LinkedIn, Discord). |
| `clearpath-icon-400.png` | Rounded tile on transparent, for places that show the image as-is (Gmail signature, docs). |

On navy backgrounds the mark can take a soft blue/mint glow (see the social template). It doesn't need one on white.

## Extension icons

`extension/icon-16.png`, `icon-32.png`, `icon-48.png`, `icon-128.png`, rendered from `clearpath-icon.svg`. These are copied into `clearpath-extension/public/icons/` and referenced from `manifest.json` (`icons` and `action.default_icon`). The 128 px one is also the Chrome Web Store icon.

## Social images

| File | Size | Use |
| --- | --- | --- |
| `social/og-image-1200x630.png` | 1200×630 (rendered at 2×) | Link previews for clearpathext.com (the site's `og.png`) |

Its HTML source is in `social/templates/`. To change it, edit the HTML and re-render it at the listed size with a headless browser (Chromium/Playwright screenshot of the page, opened from the file so the relative SVG path resolves). The template loads DM Serif Display and DM Sans from Google Fonts.

## Colours

These match the website's Tailwind tokens.

| Token | Hex | Use |
| --- | --- | --- |
| `navy-900` | `#0D1F3C` | Primary background, icon tile |
| `navy-800` | `#112240` | Raised surfaces |
| `brand-blue` | `#5B9BF8` | Start of the gradient, links, the mark's dot |
| `brand-green` | `#6DD9A8` | End of the gradient, the chevron |
| Gradient | `#5B9BF8 → #6DD9A8` | The mark, headline accents (`bg-brand-gradient`) |

## Typography

- **DM Serif Display** for headings and the wordmark
- **DM Sans** (300–600) for body text and UI
- **JetBrains Mono** for code
