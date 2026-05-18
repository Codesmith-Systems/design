# Fjord Design System

> Deep waters — A moody teal design system for bold, immersive interfaces.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Accent         | `#12768A` | Alpine Landing  | Primary actions, links, CTAs  |
| Dark           | `#030A0A` | Eight Ball      | Headers, nav, dark surfaces   |
| Body           | `#515C5C` | Bovine          | Body text, secondary elements |
| Muted          | `#6DADBE` | Water Music     | Borders, muted text, dividers |
| Muted Light    | `#CEDADB` | Light Detroit   | Light backgrounds, cards      |
| Surface        | `#E8EEEF` | Mist            | Page background, inputs       |
| Card           | `#FFFFFF` | Pure White      | Card background               |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Dark           | `#030A0A` | Primary dark, hero sections   |
| Dark-light     | `#0B3F43` | Dark hover state              |
| Accent         | `#12768A` | Primary actions, body text    |
| Accent-lt      | `#1A8A9E` | Hover state                   |
| Body           | `#515C5C` | Secondary elements            |
| Muted          | `#6DADBE` | Borders, placeholders         |
| Muted Light    | `#CEDADB` | Card backgrounds, sections    |
| Surface        | `#E8EEEF` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#2A8A6A` | Positive states     |
| Warning  | `#C49A3E` | Caution states      |
| Error    | `#B85454` | Error states        |
| Info     | `#12768A` | Information (=accent) |

### Semantic Mappings

```css
--bg-primary: #E8EEEF;            /* Page background */
--bg-secondary: #CEDADB;          /* Section/card background */
--bg-tertiary: #6DADBE;           /* Elevated surface */
--bg-card: #FFFFFF;               /* Card background */
--bg-input: #E8EEEF;              /* Input field background */

--text-primary: #030A0A;          /* Headings, important text */
--text-secondary: #515C5C;        /* Body text */
--text-tertiary: #6DADBE;         /* Captions, descriptions */
--text-muted: #CEDADB;            /* Disabled, placeholders */
--text-inverse: #E8EEEF;          /* Text on dark backgrounds */

--accent: #12768A;                /* Primary accent */
--accent-hover: #1A8A9E;          /* Accent hover state */
--accent-muted: rgba(18,118,138,0.08); /* Subtle accent bg */

--border: #CEDADB;                /* Default border */
--border-hover: #6DADBE;          /* Hover border */
--border-focus: #12768A;          /* Focus ring */
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
| `--shadow-sm`      | `0 2px 8px rgba(3,10,10,0.08)`        | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(3,10,10,0.1)`        | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(3,10,10,0.14)`       | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(3,10,10,0.18)`      | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#12768A`     | `#FFFFFF`     | `#12768A`           |
| Secondary   | transparent   | `#030A0A`     | `#030A0A`           |
| Ghost       | transparent   | `#515C5C`     | none                |
| Danger      | `#B85454`     | `#FFFFFF`     | `#B85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

**States:** hover lifts with shadow, active presses down

### Input Fields

- Background: `#E8EEEF`
- Border: `1px solid #CEDADB`
- Focus border: `#12768A` + ring `0 0 0 3px rgba(18,118,138,0.12)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #CEDADB`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(18,118,138,0.08)`     | `#12768A`   |
| Success   | `rgba(42,138,106,0.1)`      | `#2A8A6A`   |
| Warning   | `rgba(196,154,62,0.1)`      | `#C49A3E`   |
| Error     | `rgba(184,84,84,0.1)`       | `#B85454`   |
| Info      | `rgba(18,118,138,0.1)`      | `#12768A`   |

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
- `#030A0A` on `#E8EEEF` = **16.2:1** (AAA)
- `#12768A` on `#E8EEEF` = **5.1:1** (AA)
- `#515C5C` on `#E8EEEF` = **5.8:1** (AA)
- Never use `#CEDADB` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  /* Core Palette */
  --fjord-dark: #030A0A;
  --fjord-dark-light: #0B3F43;
  --fjord-accent: #12768A;
  --fjord-accent-light: #1A8A9E;
  --fjord-body: #515C5C;
  --fjord-muted: #6DADBE;
  --fjord-muted-light: #CEDADB;
  --fjord-surface: #E8EEEF;
  --fjord-card: #FFFFFF;

  /* Semantic */
  --bg-primary: #E8EEEF;
  --bg-secondary: #CEDADB;
  --bg-tertiary: #6DADBE;
  --bg-card: #FFFFFF;
  --bg-input: #E8EEEF;

  --text-primary: #030A0A;
  --text-secondary: #515C5C;
  --text-tertiary: #6DADBE;
  --text-muted: #CEDADB;
  --text-inverse: #E8EEEF;

  --accent: #12768A;
  --accent-hover: #1A8A9E;
  --accent-muted: rgba(18,118,138,0.08);

  --border: #CEDADB;
  --border-hover: #6DADBE;
  --border-focus: #12768A;

  --success: #2A8A6A;
  --warning: #C49A3E;
  --error: #B85454;
  --info: #12768A;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(3,10,10,0.08);
  --shadow-md: 0 4px 16px rgba(3,10,10,0.1);
  --shadow-lg: 0 8px 32px rgba(3,10,10,0.14);
  --shadow-xl: 0 16px 48px rgba(3,10,10,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Fjord Design System v1.0*
