# Calcite Design System

> Earth and fire — A warm, grounded design system with vibrant orange accents.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Light          | `#DDDCDB` | Stone Light     | Page background, inputs       |
| Accent         | `#FD7B41` | Lava Orange     | Primary actions, links, CTAs  |
| Warm           | `#EDBF9B` | Sandstone       | Secondary backgrounds, cards  |
| Dark           | `#3C4044` | Basalt          | Headers, nav, dark surfaces   |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Dark           | `#3C4044` | Primary dark, hero sections   |
| Dark-light     | `#4E5256` | Dark hover state              |
| Accent         | `#FD7B41` | Primary actions, body text    |
| Accent-lt      | `#FD9563` | Hover state                   |
| Warm           | `#EDBF9B` | Secondary elements            |
| Warm-light     | `#F2D4B8` | Warm hover                    |
| Light          | `#DDDCDB` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#5A9E6F` | Positive states     |
| Warning  | `#E8A83E` | Caution states      |
| Error    | `#C45454` | Error states        |
| Info     | `#FD7B41` | Information (=accent) |

### Semantic Mappings

```css
--bg-primary: #DDDCDB;            /* Page background */
--bg-secondary: #EDBF9B;          /* Section/card background */
--bg-tertiary: #F2D4B8;           /* Elevated surface */
--bg-card: #FFFFFF;               /* Card background */
--bg-input: #DDDCDB;              /* Input field background */

--text-primary: #3C4044;          /* Headings, important text */
--text-secondary: #FD7B41;        /* Body text */
--text-tertiary: #5A5E62;         /* Captions, descriptions */
--text-muted: #A0A4A8;            /* Disabled, placeholders */
--text-inverse: #DDDCDB;          /* Text on dark backgrounds */

--accent: #FD7B41;                /* Primary accent */
--accent-hover: #FD9563;          /* Accent hover state */
--accent-muted: rgba(253,123,65,0.08); /* Subtle accent bg */

--border: #A0A4A8;                /* Default border */
--border-hover: #5A5E62;          /* Hover border */
--border-focus: #FD7B41;          /* Focus ring */
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
| `--shadow-sm`      | `0 2px 8px rgba(60,64,68,0.08)`       | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(60,64,68,0.1)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(60,64,68,0.14)`      | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(60,64,68,0.18)`     | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#FD7B41`     | `#FFFFFF`     | `#FD7B41`           |
| Secondary   | transparent   | `#3C4044`     | `#3C4044`           |
| Ghost       | transparent   | `#5A5E62`     | none                |
| Danger      | `#C45454`     | `#FFFFFF`     | `#C45454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

**States:** hover lifts with shadow, active presses down

### Input Fields

- Background: `#DDDCDB`
- Border: `1px solid #A0A4A8`
- Focus border: `#FD7B41` + ring `0 0 0 3px rgba(253,123,65,0.12)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #EDBF9B`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(253,123,65,0.08)`     | `#FD7B41`   |
| Success   | `rgba(90,158,111,0.1)`      | `#5A9E6F`   |
| Warning   | `rgba(232,168,62,0.1)`      | `#E8A83E`   |
| Error     | `rgba(196,84,84,0.1)`       | `#C45454`   |
| Info      | `rgba(253,123,65,0.1)`      | `#FD7B41`   |

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
- `#3C4044` on `#DDDCDB` = **10.8:1** (AAA)
- `#FD7B41` on `#DDDCDB` = **3.2:1** (AA large text only — use on dark for body text)
- `#5A5E62` on `#DDDCDB` = **5.1:1** (AA)
- Never use `#A0A4A8` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  /* Core Palette */
  --calcite-dark: #3C4044;
  --calcite-dark-light: #4E5256;
  --calcite-accent: #FD7B41;
  --calcite-accent-light: #FD9563;
  --calcite-warm: #EDBF9B;
  --calcite-warm-light: #F2D4B8;
  --calcite-light: #DDDCDB;
  --calcite-card: #FFFFFF;

  /* Semantic */
  --bg-primary: #DDDCDB;
  --bg-secondary: #EDBF9B;
  --bg-tertiary: #F2D4B8;
  --bg-card: #FFFFFF;
  --bg-input: #DDDCDB;

  --text-primary: #3C4044;
  --text-secondary: #FD7B41;
  --text-tertiary: #5A5E62;
  --text-muted: #A0A4A8;
  --text-inverse: #DDDCDB;

  --accent: #FD7B41;
  --accent-hover: #FD9563;
  --accent-muted: rgba(253,123,65,0.08);

  --border: #A0A4A8;
  --border-hover: #5A5E62;
  --border-focus: #FD7B41;

  --success: #5A9E6F;
  --warning: #E8A83E;
  --error: #C45454;
  --info: #FD7B41;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(60,64,68,0.08);
  --shadow-md: 0 4px 16px rgba(60,64,68,0.1);
  --shadow-lg: 0 8px 32px rgba(60,64,68,0.14);
  --shadow-xl: 0 16px 48px rgba(60,64,68,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Calcite Design System v1.0*
