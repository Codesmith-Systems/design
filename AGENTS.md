# Coding Agent Instructions

This project is a simple PHP + standalone HTML design-theme gallery.

## Project Overview

- `index.php` is the main gallery and theme registry.
- Each theme lives in its own folder.
- Each theme folder contains:
  - `preview.html` — the visual preview page
  - `DESIGN.md` — the design-system documentation for that theme

## Important Rules

1. Keep changes scoped.
   - If the user asks for one theme, edit only that theme folder.
   - If the user asks for a global change, update every `*/preview.html` consistently.

2. Preserve theme identity.
   - Do not randomly change palettes, image URLs, typography, or mood language.
   - Use each theme’s `DESIGN.md` as the source of truth for colors and component style.

3. Keep the project build-free.
   - Do not add Node, npm, bundlers, frameworks, or package managers unless explicitly requested.
   - Prefer plain HTML, CSS, JavaScript, PHP, and Markdown.

4. Maintain image credits.
   - Do not remove the `README.md` image-credit table.
   - If an image is changed, update the credit table with the new Pexels/photo source and license.

5. Do not inline large assets.
   - Current images are externally loaded from Pexels.
   - Keep external image URLs unless the user specifically asks to download/localize assets.

6. Preserve donation information.
   - Keep the USDT TRC20 support section in `README.md` unless the project owner asks to remove it.

## Recommended Inspection Steps

Before editing:

1. Read `index.php` to understand the registered themes.
2. Read the relevant theme’s `DESIGN.md`.
3. Read the relevant theme’s `preview.html`.
4. Identify whether the requested change is single-theme or global.

## Common Tasks

### Add a New Theme

1. Create a new slug folder, for example:

```text
ocean-mist/
```

2. Add:

```text
ocean-mist/preview.html
ocean-mist/DESIGN.md
```

3. Add the theme to `index.php` in these arrays:

- `$themes`
- `$imageUrls`
- `$imagePositions`
- `$phrases`

4. Test `index.php` and the new preview page.

### Update All Theme Previews

1. Search all `*/preview.html` files.
2. Apply the same structural/CSS change to every preview.
3. Verify the count of changed files matches the number of theme folders.
4. Open at least one representative preview in a browser.

### Update the Gallery

1. Edit `index.php`.
2. Keep `$themes`, `$imageUrls`, `$imagePositions`, and `$phrases` synchronized.
3. Make sure all gallery links resolve to existing `preview.html` files.

## Verification Checklist

After editing:

- `index.php` still loads.
- Theme links point to valid folders.
- Edited preview pages open without obvious layout breakage.
- No image-credit rows were removed accidentally.
- Donation address remains unchanged unless explicitly requested.

USDT TRC20 address:

```text
TSgwbA11ZexsM2jhw6LvzfaKd2x8xkJWC3
```
