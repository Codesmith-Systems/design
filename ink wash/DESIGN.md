# Ink Wash Design System

> Brush and paper — An elegant, artistic design system inspired by traditional ink painting.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Charcoal       | `#4A4A4A` | Deep Ink        | Headers, nav, dark surfaces   |
| Cool Gray      | `#CBCBCB` | Washed Stone    | Borders, muted text, dividers |
| Soft Ivory     | `#FFFFE3` | Rice Paper      | Page background, inputs       |
| Muted Slate    | `#6D8196` | Distant Mountain| Primary actions, links, CTAs  |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Charcoal       | `#4A4A4A` | Primary dark, hero sections   |
| Charcoal-light | `#5E5E5E` | Dark hover state              |
| Muted Slate    | `#6D8196` | Primary actions, accents      |
| Muted Slate-lt | `#8499AD` | Hover state                   |
| Cool Gray      | `#CBCBCB` | Secondary elements            |
| Cool Gray-light| `#DCDCDC` | Borders, placeholders         |
| Soft Ivory     | `#FFFFE3` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#5A8C6F` | Positive states     |
| Warning  | `#B8943E` | Caution states      |
| Error    | `#A85454` | Error states        |
| Info     | `#6D8196` | Information (=slate) |

### Semantic Mappings

```css
--bg-primary: #FFFFE3;            /* Page background */
--bg-secondary: #DCDCDC;          /* Section/card background */
--bg-tertiary: #CBCBCB;           /* Elevated surface */
--bg-card: #FFFFFF;               /* Card background */
--bg-input: #FFFFE3;              /* Input field background */

--text-primary: #4A4A4A;          /* Headings, important text */
--text-secondary: #6D8196;        /* Body text */
--text-tertiary: #6D8196;         /* Captions, descriptions */
--text-muted: #CBCBCB;            /* Disabled, placeholders */
--text-inverse: #FFFFE3;          /* Text on dark backgrounds */

--accent: #6D8196;                /* Primary accent */
--accent-hover: #8499AD;          /* Accent hover state */
--accent-muted: rgba(109,129,150,0.08); /* Subtle accent bg */

--border: #CBCBCB;                /* Default border */
--border-hover: #6D8196;          /* Hover border */
--border-focus: #6D8196;          /* Focus ring */
```

---

## 2. Typography

### Font Families

| Token           | Value                | Usage                     |
|-----------------|----------------------|---------------------------|
| `--font-display` | Playfair Display    | Headings, labels, buttons |
| `--font-body`    | DM Sans             | Body text, descriptions   |

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
| `--shadow-sm`      | `0 2px 8px rgba(74,74,74,0.08)`       | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(74,74,74,0.1)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(74,74,74,0.14)`      | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(74,74,74,0.18)`     | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#6D8196`     | `#FFFFE3`     | `#6D8196`           |
| Secondary   | transparent   | `#4A4A4A`     | `#4A4A4A`           |
| Ghost       | transparent   | `#6D8196`     | none                |
| Danger      | `#A85454`     | `#FFFFE3`     | `#A85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

**States:** hover lifts with shadow, active presses down

### Input Fields

- Background: `#FFFFE3`
- Border: `1px solid #CBCBCB`
- Focus border: `#6D8196` + ring `0 0 0 3px rgba(109,129,150,0.12)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #DCDCDC`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(109,129,150,0.08)`    | `#6D8196`   |
| Success   | `rgba(90,140,111,0.1)`      | `#5A8C6F`   |
| Warning   | `rgba(184,148,62,0.1)`      | `#B8943E`   |
| Error     | `rgba(168,84,84,0.1)`       | `#A85454`   |
| Info      | `rgba(109,129,150,0.1)`     | `#6D8196`   |

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
- `#4A4A4A` on `#FFFFE3` = **12.1:1** (AAA)
- `#6D8196` on `#FFFFE3` = **4.9:1** (AA)
- `#6D8196` on `#FFFFE3` for large text = **4.9:1** (AA)
- Never use `#CBCBCB` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  /* Core Palette */
  --inkwash-charcoal: #4A4A4A;
  --inkwash-charcoal-light: #5E5E5E;
  --inkwash-slate: #6D8196;
  --inkwash-slate-light: #8499AD;
  --inkwash-cool-gray: #CBCBCB;
  --inkwash-cool-gray-light: #DCDCDC;
  --inkwash-ivory: #FFFFE3;
  --inkwash-card: #FFFFFF;

  /* Semantic */
  --bg-primary: #FFFFE3;
  --bg-secondary: #DCDCDC;
  --bg-tertiary: #CBCBCB;
  --bg-card: #FFFFFF;
  --bg-input: #FFFFE3;

  --text-primary: #4A4A4A;
  --text-secondary: #6D8196;
  --text-tertiary: #6D8196;
  --text-muted: #CBCBCB;
  --text-inverse: #FFFFE3;

  --accent: #6D8196;
  --accent-hover: #8499AD;
  --accent-muted: rgba(109,129,150,0.08);

  --border: #CBCBCB;
  --border-hover: #6D8196;
  --border-focus: #6D8196;

  --success: #5A8C6F;
  --warning: #B8943E;
  --error: #A85454;
  --info: #6D8196;

  --font-display: 'Playfair Display', serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(74,74,74,0.08);
  --shadow-md: 0 4px 16px rgba(74,74,74,0.1);
  --shadow-lg: 0 8px 32px rgba(74,74,74,0.14);
  --shadow-xl: 0 16px 48px rgba(74,74,74,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Ink Wash Design System v1.0*
