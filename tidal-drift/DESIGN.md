# Tidal Drift Design System

> Ocean depths meet twilight — A sophisticated blue-gray design system for modern SaaS products.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Tangaroa       | `#1F2E3B` | Deep Ocean      | Headers, nav, dark surfaces   |
| Night Tide     | `#45535F` | Twilight Blue   | Primary text, buttons, CTAs   |
| Forever Denim  | `#7A858E` | Weathered Steel | Secondary text, icons         |
| Silver Lined   | `#BBBFC4` | Sea Foam        | Borders, muted text, dividers |
| December Sky   | `#D5D7DA` | Overcast        | Light backgrounds, cards      |
| White Edgar    | `#EDEDED` | Driftwood       | Page background, inputs       |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Tangaroa       | `#1F2E3B` | Primary dark, hero sections   |
| Tangaroa-light | `#2A3D4D` | Dark hover state              |
| Night Tide     | `#45535F` | Primary actions, body text    |
| Night Tide-lt  | `#556570` | Hover state                   |
| Forever Denim  | `#7A858E` | Secondary elements            |
| Silver Lined   | `#BBBFC4` | Borders, placeholders         |
| December Sky   | `#D5D7DA` | Card backgrounds, sections    |
| White Edgar    | `#EDEDED` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#4A7C6F` | Positive states     |
| Warning  | `#B8943E` | Caution states      |
| Error    | `#A85454` | Error states        |
| Info     | `#45535F` | Information (=primary) |

### Semantic Mappings

```css
--bg-primary: #EDEDED;            /* Page background */
--bg-secondary: #D5D7DA;          /* Section/card background */
--bg-tertiary: #BBBFC4;           /* Elevated surface */
--bg-card: #FFFFFF;               /* Card background */
--bg-input: #EDEDED;              /* Input field background */

--text-primary: #1F2E3B;          /* Headings, important text */
--text-secondary: #45535F;        /* Body text */
--text-tertiary: #7A858E;         /* Captions, descriptions */
--text-muted: #BBBFC4;            /* Disabled, placeholders */
--text-inverse: #EDEDED;          /* Text on dark backgrounds */

--accent: #1F2E3B;                /* Primary accent */
--accent-hover: #2A3D4D;          /* Accent hover state */
--accent-muted: rgba(31,46,59,0.08); /* Subtle accent bg */

--border: #BBBFC4;                /* Default border */
--border-hover: #7A858E;          /* Hover border */
--border-focus: #45535F;          /* Focus ring */
```

---

## 2. Typography

### Font Families

| Token           | Value             | Usage                     |
|-----------------|-------------------|---------------------------|
| `--font-display` | Space Grotesk    | Headings, labels, buttons |
| `--font-body`    | DM Sans          | Body text, descriptions   |

### Type Scale

| Token          | Size      | Weight | Line Height | Usage                |
|----------------|-----------|--------|-------------|----------------------|
| `--text-5xl`   | 3rem      | 700    | 1.1         | Hero headings        |
| `--text-4xl`   | 2.25rem   | 700    | 1.2         | Page titles          |
| `--text-3xl`   | 1.875rem  | 600    | 1.3         | Section headings     |
| `--text-2xl`   | 1.5rem    | 600    | 1.3         | Card titles          |
| `--text-xl`    | 1.25rem   | 600    | 1.4         | Subsection titles    |
| `--text-lg`    | 1.125rem  | 400    | 1.6         | Lead paragraphs      |
| `--text-base`  | 1rem      | 400    | 1.6         | Body text            |
| `--text-sm`    | 0.875rem  | 500    | 1.5         | Labels, captions     |
| `--text-xs`    | 0.75rem   | 500    | 1.5         | Metadata, hints      |

---

## 3. Spacing

Base unit: **4px**

| Token         | Value | Usage                     |
|---------------|-------|---------------------------|
| `--space-1`   | 4px   | Tight gaps                |
| `--space-2`   | 8px   | Inner component padding   |
| `--space-3`   | 12px  | Related element gaps      |
| `--space-4`   | 16px  | Standard padding          |
| `--space-5`   | 20px  | Comfortable padding       |
| `--space-6`   | 24px  | Card padding              |
| `--space-8`   | 32px  | Section gaps              |
| `--space-10`  | 40px  | Large gaps                |
| `--space-12`  | 48px  | Section padding           |
| `--space-16`  | 64px  | Page sections             |
| `--space-20`  | 80px  | Hero spacing              |

---

## 4. Border Radius

| Token          | Value  | Usage                     |
|----------------|--------|---------------------------|
| `--radius-sm`   | 6px    | Small elements, badges    |
| `--radius-md`   | 10px   | Buttons, inputs           |
| `--radius-lg`   | 16px   | Cards, modals             |
| `--radius-xl`   | 24px   | Large panels              |
| `--radius-full` | 9999px | Pills, avatars, toggles   |

---

## 5. Shadows

| Token              | Value                                  | Usage              |
|--------------------|----------------------------------------|--------------------|
| `--shadow-sm`      | `0 2px 8px rgba(31,46,59,0.08)`       | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(31,46,59,0.1)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(31,46,59,0.14)`      | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(31,46,59,0.18)`     | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#1F2E3B`     | `#EDEDED`     | `#1F2E3B`           |
| Secondary   | transparent   | `#1F2E3B`     | `#1F2E3B`           |
| Ghost       | transparent   | `#45535F`     | none                |
| Danger      | `#A85454`     | `#EDEDED`     | `#A85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

**States:** hover lifts with shadow, active presses down

### Input Fields

- Background: `#EDEDED`
- Border: `1px solid #BBBFC4`
- Focus border: `#45535F` + ring `0 0 0 3px rgba(69,83,95,0.12)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #D5D7DA`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(31,46,59,0.08)`       | `#1F2E3B`   |
| Success   | `rgba(74,124,111,0.1)`      | `#4A7C6F`   |
| Warning   | `rgba(184,148,62,0.1)`      | `#B8943E`   |
| Error     | `rgba(168,84,84,0.1)`       | `#A85454`   |
| Info      | `rgba(69,83,95,0.1)`        | `#45535F`   |

---

## 7. Motion

| Token              | Value                         | Usage            |
|--------------------|-------------------------------|------------------|
| `--duration-fast`   | 150ms                        | Hover, focus     |
| `--duration-normal` | 250ms                        | Transitions      |
| `--duration-slow`   | 400ms                        | Enter/exit       |
| `--ease-out`        | `cubic-bezier(0.16, 1, 0.3, 1)` | All transitions  |

---

## 8. Accessibility Notes

- Minimum contrast ratio: **4.5:1** for normal text, **3:1** for large text
- `#1F2E3B` on `#EDEDED` = **11.8:1** (AAA)
- `#45535F` on `#EDEDED` = **7.1:1** (AAA)
- `#7A858E` on `#EDEDED` = **3.8:1** (AA large text only)
- Never use `#BBBFC4` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  /* Core Palette */
  --tangaroa: #1F2E3B;
  --tangaroa-light: #2A3D4D;
  --night-tide: #45535F;
  --night-tide-light: #556570;
  --forever-denim: #7A858E;
  --silver-lined: #BBBFC4;
  --december-sky: #D5D7DA;
  --white-edgar: #EDEDED;

  /* Semantic */
  --bg-primary: #EDEDED;
  --bg-secondary: #D5D7DA;
  --bg-tertiary: #BBBFC4;
  --bg-card: #FFFFFF;
  --bg-input: #EDEDED;

  --text-primary: #1F2E3B;
  --text-secondary: #45535F;
  --text-tertiary: #7A858E;
  --text-muted: #BBBFC4;
  --text-inverse: #EDEDED;

  --accent: #1F2E3B;
  --accent-hover: #2A3D4D;
  --accent-muted: rgba(31,46,59,0.08);

  --border: #BBBFC4;
  --border-hover: #7A858E;
  --border-focus: #45535F;

  --success: #4A7C6F;
  --warning: #B8943E;
  --error: #A85454;
  --info: #45535F;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(31,46,59,0.08);
  --shadow-md: 0 4px 16px rgba(31,46,59,0.1);
  --shadow-lg: 0 8px 32px rgba(31,46,59,0.14);
  --shadow-xl: 0 16px 48px rgba(31,46,59,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Tidal Drift Design System v1.0*
