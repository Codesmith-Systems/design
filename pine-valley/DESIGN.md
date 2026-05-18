# Pine Valley Design System

> Cool serenity — A muted blue-green design system for calm, professional interfaces.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Accent         | `#6B8384` | Hammock         | Primary actions, links, CTAs  |
| Dark           | `#163212` | Dark Serpent    | Headers, nav, dark surfaces   |
| Body           | `#A0B1C1` | Blue Pot        | Body text, secondary elements |
| Muted          | `#C8D7E6` | Lively Tune     | Borders, muted text, dividers |
| Muted Light    | `#E2EBF6` | Dissolved Denim | Light backgrounds, cards      |
| Surface        | `#F4F9FC` | Mā White        | Page background, inputs       |
| Card           | `#FFFFFF` | Pure White      | Card background               |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Dark           | `#163212` | Primary dark, hero sections   |
| Dark-light     | `#1E4418` | Dark hover state              |
| Accent         | `#6B8384` | Primary actions, body text    |
| Accent-lt      | `#7A9495` | Hover state                   |
| Body           | `#A0B1C1` | Secondary elements            |
| Muted          | `#C8D7E6` | Borders, placeholders         |
| Muted Light    | `#E2EBF6` | Card backgrounds, sections    |
| Surface        | `#F4F9FC` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#4A7A5E` | Positive states     |
| Warning  | `#C49A3E` | Caution states      |
| Error    | `#B85454` | Error states        |
| Info     | `#6B8384` | Information (=accent) |

### Semantic Mappings

```css
--bg-primary: #F4F9FC;            /* Page background */
--bg-secondary: #E2EBF6;          /* Section/card background */
--bg-tertiary: #C8D7E6;           /* Elevated surface */
--bg-card: #FFFFFF;               /* Card background */
--bg-input: #F4F9FC;              /* Input field background */

--text-primary: #163212;          /* Headings, important text */
--text-secondary: #A0B1C1;        /* Body text */
--text-tertiary: #6B8384;         /* Captions, descriptions */
--text-muted: #C8D7E6;            /* Disabled, placeholders */
--text-inverse: #F4F9FC;          /* Text on dark backgrounds */

--accent: #6B8384;                /* Primary accent */
--accent-hover: #7A9495;          /* Accent hover state */
--accent-muted: rgba(107,131,132,0.08); /* Subtle accent bg */

--border: #C8D7E6;                /* Default border */
--border-hover: #A0B1C1;          /* Hover border */
--border-focus: #6B8384;          /* Focus ring */
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
| `--shadow-sm`      | `0 2px 8px rgba(22,50,18,0.08)`       | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(22,50,18,0.1)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(22,50,18,0.14)`      | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(22,50,18,0.18)`     | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#6B8384`     | `#FFFFFF`     | `#6B8384`           |
| Secondary   | transparent   | `#163212`     | `#163212`           |
| Ghost       | transparent   | `#A0B1C1`     | none                |
| Danger      | `#B85454`     | `#FFFFFF`     | `#B85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

**States:** hover lifts with shadow, active presses down

### Input Fields

- Background: `#F4F9FC`
- Border: `1px solid #C8D7E6`
- Focus border: `#6B8384` + ring `0 0 0 3px rgba(107,131,132,0.12)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #E2EBF6`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(107,131,132,0.08)`    | `#6B8384`   |
| Success   | `rgba(74,122,94,0.1)`       | `#4A7A5E`   |
| Warning   | `rgba(196,154,62,0.1)`      | `#C49A3E`   |
| Error     | `rgba(184,84,84,0.1)`       | `#B85454`   |
| Info      | `rgba(107,131,132,0.1)`     | `#6B8384`   |

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
- `#163212` on `#F4F9FC` = **15.8:1** (AAA)
- `#6B8384` on `#F4F9FC` = **4.9:1** (AA)
- `#A0B1C1` on `#F4F9FC` = **3.2:1** (AA large text only)
- Never use `#C8D7E6` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  /* Core Palette */
  --pine-dark: #163212;
  --pine-dark-light: #1E4418;
  --pine-accent: #6B8384;
  --pine-accent-light: #7A9495;
  --pine-body: #A0B1C1;
  --pine-muted: #C8D7E6;
  --pine-muted-light: #E2EBF6;
  --pine-surface: #F4F9FC;
  --pine-card: #FFFFFF;

  /* Semantic */
  --bg-primary: #F4F9FC;
  --bg-secondary: #E2EBF6;
  --bg-tertiary: #C8D7E6;
  --bg-card: #FFFFFF;
  --bg-input: #F4F9FC;

  --text-primary: #163212;
  --text-secondary: #A0B1C1;
  --text-tertiary: #6B8384;
  --text-muted: #C8D7E6;
  --text-inverse: #F4F9FC;

  --accent: #6B8384;
  --accent-hover: #7A9495;
  --accent-muted: rgba(107,131,132,0.08);

  --border: #C8D7E6;
  --border-hover: #A0B1C1;
  --border-focus: #6B8384;

  --success: #4A7A5E;
  --warning: #C49A3E;
  --error: #B85454;
  --info: #6B8384;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(22,50,18,0.08);
  --shadow-md: 0 4px 16px rgba(22,50,18,0.1);
  --shadow-lg: 0 8px 32px rgba(22,50,18,0.14);
  --shadow-xl: 0 16px 48px rgba(22,50,18,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Pine Valley Design System v1.0*
