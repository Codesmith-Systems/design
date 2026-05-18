# Clockwork Design System

> Precision in motion — A warm, mechanical design system with bold orange energy.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Deep Orange    | `#E56515` | Gear Fire       | Primary actions, links, CTAs  |
| Light Orange   | `#FBA45C` | Copper Glow     | Secondary accents, highlights |
| Gray           | `#919599` | Machine Steel   | Secondary text, icons         |
| Light Gray     | `#CDCDCB` | Polished Metal  | Borders, muted text, dividers |
| White          | `#F8F8F8` | Clean Plate     | Page background, inputs       |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Deep Orange    | `#E56515` | Primary dark, hero sections   |
| Deep Orange-lt | `#F07A2E` | Dark hover state              |
| Light Orange   | `#FBA45C` | Primary actions, accents      |
| Light Orange-lt| `#FCB87A` | Hover state                   |
| Gray           | `#919599` | Secondary elements            |
| Light Gray     | `#CDCDCB` | Borders, placeholders         |
| White          | `#F8F8F8` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#4A8C6F` | Positive states     |
| Warning  | `#FBA45C` | Caution states      |
| Error    | `#C45454` | Error states        |
| Info     | `#E56515` | Information (=accent) |

### Semantic Mappings

```css
--bg-primary: #F8F8F8;            /* Page background */
--bg-secondary: #CDCDCB;          /* Section/card background */
--bg-tertiary: #919599;           /* Elevated surface */
--bg-card: #FFFFFF;               /* Card background */
--bg-input: #F8F8F8;              /* Input field background */

--text-primary: #E56515;          /* Headings, important text */
--text-secondary: #919599;        /* Body text */
--text-tertiary: #919599;         /* Captions, descriptions */
--text-muted: #CDCDCB;            /* Disabled, placeholders */
--text-inverse: #F8F8F8;          /* Text on dark backgrounds */

--accent: #E56515;                /* Primary accent */
--accent-hover: #F07A2E;          /* Accent hover state */
--accent-muted: rgba(229,101,21,0.08); /* Subtle accent bg */

--border: #CDCDCB;                /* Default border */
--border-hover: #919599;          /* Hover border */
--border-focus: #E56515;          /* Focus ring */
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
| `--shadow-sm`      | `0 2px 8px rgba(229,101,21,0.08)`     | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(229,101,21,0.1)`     | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(229,101,21,0.14)`    | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(229,101,21,0.18)`   | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#E56515`     | `#FFFFFF`     | `#E56515`           |
| Secondary   | transparent   | `#E56515`     | `#E56515`           |
| Ghost       | transparent   | `#919599`     | none                |
| Danger      | `#C45454`     | `#FFFFFF`     | `#C45454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

**States:** hover lifts with shadow, active presses down

### Input Fields

- Background: `#F8F8F8`
- Border: `1px solid #CDCDCB`
- Focus border: `#E56515` + ring `0 0 0 3px rgba(229,101,21,0.12)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #CDCDCB`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(229,101,21,0.08)`     | `#E56515`   |
| Success   | `rgba(74,140,111,0.1)`      | `#4A8C6F`   |
| Warning   | `rgba(251,164,92,0.1)`      | `#FBA45C`   |
| Error     | `rgba(196,84,84,0.1)`       | `#C45454`   |
| Info      | `rgba(229,101,21,0.1)`      | `#E56515`   |

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
- `#E56515` on `#F8F8F8` = **4.6:1** (AA)
- `#919599` on `#F8F8F8` = **3.4:1** (AA large text only)
- Never use `#CDCDCB` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  /* Core Palette */
  --clockwork-deep-orange: #E56515;
  --clockwork-deep-orange-light: #F07A2E;
  --clockwork-light-orange: #FBA45C;
  --clockwork-light-orange-light: #FCB87A;
  --clockwork-gray: #919599;
  --clockwork-light-gray: #CDCDCB;
  --clockwork-white: #F8F8F8;
  --clockwork-card: #FFFFFF;

  /* Semantic */
  --bg-primary: #F8F8F8;
  --bg-secondary: #CDCDCB;
  --bg-tertiary: #919599;
  --bg-card: #FFFFFF;
  --bg-input: #F8F8F8;

  --text-primary: #E56515;
  --text-secondary: #919599;
  --text-tertiary: #919599;
  --text-muted: #CDCDCB;
  --text-inverse: #F8F8F8;

  --accent: #E56515;
  --accent-hover: #F07A2E;
  --accent-muted: rgba(229,101,21,0.08);

  --border: #CDCDCB;
  --border-hover: #919599;
  --border-focus: #E56515;

  --success: #4A8C6F;
  --warning: #FBA45C;
  --error: #C45454;
  --info: #E56515;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(229,101,21,0.08);
  --shadow-md: 0 4px 16px rgba(229,101,21,0.1);
  --shadow-lg: 0 8px 32px rgba(229,101,21,0.14);
  --shadow-xl: 0 16px 48px rgba(229,101,21,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Clockwork Design System v1.0*
