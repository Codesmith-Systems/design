# Design Studio — Theme Gallery

A compact, image-led design-system gallery containing 23 polished visual themes. Each theme includes a live HTML preview and a dedicated `DESIGN.md` file with palette tokens, typography, spacing, radius, shadows, and reusable component guidance.

The project is intentionally simple: plain PHP for the gallery index, standalone HTML preview pages, CSS custom properties, and markdown design-system documentation. It is easy to host on Laragon, XAMPP, Apache, Nginx, GitHub Pages with minor conversion, or any PHP-capable static-style environment.

## Project Description

Design Studio is a curated collection of ready-to-use interface moodboards and design-system starters. It pairs strong color palettes with atmospheric Pexels imagery, subdued overlays, and clean editorial preview pages so designers, developers, and coding agents can quickly choose a visual direction for an app, dashboard, landing page, or brand system.

Included themes:

- Arctic
- Blue Eclipse
- Calcite
- Clockwork
- Coral Reef
- Fjord
- Forest
- Frost
- Golden
- Ink Wash
- Iris
- Lavender
- Lemon Drop
- Moonlight
- Moss
- Pine Valley
- Sahara
- Salt & Pepper
- Stone
- Stormy
- Sunset
- Tidal Drift
- Winter Chill

## Features

- 23 theme folders, each with:
  - `preview.html` — visual theme preview
  - `DESIGN.md` — design-system documentation
- Main gallery at `index.php`
- Image-led hero treatment with palette overlays
- Copyable color swatches in previews
- CSS custom property/token-based structure
- No build step required
- Easy for coding agents to inspect and modify

## Folder Structure

```text
/design
  index.php
  README.md
  AGENTS.md
  arctic/
    preview.html
    DESIGN.md
  blue-eclipse/
    preview.html
    DESIGN.md
  ...
```

## How to Run Locally

### Option 1: Laragon / Apache / PHP server

Place the folder in your web root:

```text
C:/laragon/www/design
```

Open:

```text
http://localhost/design/
```

### Option 2: PHP built-in server

From the project directory:

```bash
php -S localhost:8000
```

Open:

```text
http://localhost:8000
```

### Option 3: Open a preview directly

Most theme previews are standalone HTML files and can be opened directly in a browser:

```text
arctic/preview.html
sunset/preview.html
forest/preview.html
```

The main gallery uses `index.php`, so it should be served through PHP.

## How to Use the Themes

1. Open the gallery.
2. Browse the theme cards or use the arrow controls.
3. Open a theme preview.
4. Copy palette values from the swatches.
5. Read the theme’s `DESIGN.md` for implementation details.
6. Reuse the tokens in your own app, dashboard, landing page, or design system.

## Using This Project With Coding Agents

This repo is designed to be friendly to AI coding agents such as Hermes, Claude Code, Codex, Cursor, OpenCode, Aider, and similar tools.

Recommended workflow:

1. Ask the agent to inspect `index.php` first to understand the theme registry.
2. Ask the agent to inspect the target theme folder, especially:
   - `preview.html`
   - `DESIGN.md`
3. Keep edits scoped to the requested theme unless you explicitly want a global update.
4. For global changes, update all `*/preview.html` files consistently.
5. Preserve the theme identity: palette, mood, image treatment, and typography should remain aligned with each theme’s `DESIGN.md`.
6. Verify by opening `index.php` and at least one changed `preview.html` in a browser.

Example prompts:

```text
Inspect this repo and summarize how the gallery works.
```

```text
Update only the Sunset theme preview. Keep the existing palette and image treatment, but make the cards more minimal.
```

```text
Apply the same hero-header layout fix to every */preview.html file. Do not change the DESIGN.md files.
```

```text
Create a new theme folder called ocean-mist with preview.html and DESIGN.md, then add it to index.php.
```

### Agent Editing Rules

- Do not replace all themes when only one theme is requested.
- Do not remove image credits.
- Do not inline large external assets.
- Keep the project build-free unless explicitly requested.
- Maintain accessible contrast where possible.
- After editing, check for broken links and obvious syntax errors.

See `AGENTS.md` for more detailed coding-agent instructions.

## Add a New Theme

1. Create a new folder using a URL-safe slug:

```text
new-theme-name/
```

2. Add:

```text
new-theme-name/preview.html
new-theme-name/DESIGN.md
```

3. Register the theme in `index.php` by adding entries to:

- `$themes`
- `$imageUrls`
- `$imagePositions`
- `$phrases`

4. Test the gallery and preview page.

Please send only USDT on the TRC20 network to this address.

## Image Credits

All images are loaded from Pexels and are marked as free to use under the Pexels License:

https://www.pexels.com/license/

| Theme | Image credit | Photo ID | Source |
|---|---|---:|---|
| Arctic | Pexels / Francesco Ungaro | 30429891 | https://www.pexels.com/photo/30429891/ |
| Blue Eclipse | Pexels / Anton Kudryashov | 9861438 | https://www.pexels.com/photo/9861438/ |
| Calcite | Pexels / Magda Ehlers | 4611326 | https://www.pexels.com/photo/4611326/ |
| Clockwork | Pexels / Melike B | 27818256 | https://www.pexels.com/photo/27818256/ |
| Coral Reef | Pexels / Iryna Ellesionarios | 33445033 | https://www.pexels.com/photo/33445033/ |
| Fjord | Pexels / Raul Ling | 29106462 | https://www.pexels.com/photo/29106462/ |
| Forest | Pexels / Lauri Poldre | 27627366 | https://www.pexels.com/photo/27627366/ |
| Frost | Pexels / Julia Fuchs | 12486644 | https://www.pexels.com/photo/12486644/ |
| Golden | Pexels / Mattia Verga | 5624201 | https://www.pexels.com/photo/5624201/ |
| Ink Wash | Pexels / Kevin Malik | 9016471 | https://www.pexels.com/photo/9016471/ |
| Iris | Pexels / Alban Mehmeti | 37600288 | https://www.pexels.com/photo/37600288/ |
| Lavender | Pexels / Plato Terentev | 9963192 | https://www.pexels.com/photo/9963192/ |
| Lemon Drop | Pexels / Андруша Ананьев | 35560987 | https://www.pexels.com/photo/35560987/ |
| Moonlight | Pexels / Luna Joie | 17302717 | https://www.pexels.com/photo/17302717/ |
| Moss | Pexels / Stanislav Kondratiev | 23232363 | https://www.pexels.com/photo/23232363/ |
| Pine Valley | Pexels / Nedzad | 582833 | https://www.pexels.com/photo/582833/ |
| Sahara | Pexels / Douglas Santos | 6930285 | https://www.pexels.com/photo/6930285/ |
| Salt & Pepper | Pexels / Alex Dos Santos | 33944144 | https://www.pexels.com/photo/33944144/ |
| Stone | Pexels / Polina | 6788504 | https://www.pexels.com/photo/6788504/ |
| Stormy | Pexels / Damir K . | 16533892 | https://www.pexels.com/photo/16533892/ |
| Sunset | Pexels / Anton Kudryashov | 9841932 | https://www.pexels.com/photo/9841932/ |
| Tidal Drift | Pexels / Canary Vista ES | 35579610 | https://www.pexels.com/photo/35579610/ |
| Winter Chill | Pexels / Gundula Vogel | 36052500 | https://www.pexels.com/photo/36052500/ |

Note: If you replace any image, update this table with the new creator, source URL, and license.

## License

Project code and documentation can be released under the MIT License unless you choose a different license before publishing.

Images remain subject to the Pexels License and are credited above.
