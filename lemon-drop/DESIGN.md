# Lemon Drop Design System

> Bright energy — A vibrant yellow-accented design system for playful, modern interfaces.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name                | Usage                        |
|----------------|-----------|---------------------|------------------------------|
| Accent         | `#FDF79E` | Spaghetti           | Primary actions, links, CTAs  |
| Dark           | `#29292A` | Chromaphobic Black  | Headers, nav, dark surfaces   |
| Body           | `#666458` | Dusty Olive         | Body text, secondary elements |
| Muted          | `#B3B8CA` | Ethereal Mist       | Borders, muted text, dividers |
| Muted Light    | `#DBDEE4` | Terminator Chrome   | Light backgrounds, cards      |
| Surface        | `#FBFCFD` | Wash Me             | Page background, inputs       |
| Card           | `#FFFFFF` | Pure White          | Card background               |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Dark           | `#29292A` | Primary dark, hero sections   |
| Dark-light     | `#3A3A3C` | Dark hover state              |
| Accent         | `#FDF79E` | Primary actions, body text    |
| Accent-lt      | `#F5EF8A` | Hover state                   |
| Body           | `#666458` | Secondary elements            |
| Muted          | `#B3B8CA` | Borders, placeholders         |
| Muted Light    | `#DBDEE4` | Card backgrounds, sections    |
| Surface        | `#FBFCFD` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#6B8A5E` | Positive states     |
| Warning  | `#E2A84B` | Caution states      |
| Error    | `#B85454` | Error states        |
| Info     | `#FDF79E` | Information (=accent) |

### Semantic Mappings

```css
--bg-primary: #FBFCFD;            /* Page background */
--bg-secondary: #DBDEE4;          /* Section/card background */
--bg-tertiary: #B3B8CA;           /* Elevated surface */
--bg-card: #FFFFFF;               /* Card background */
--bg-input: #FBFCFD;              /* Input field background */

--text-primary: #29292A;          /* Headings, important text */
--text-secondary: #666458;        /* Body text */
--text-tertiary: #B3B8CA;         /* Captions, descriptions */
--text-muted: #DBDEE4;            /* Disabled, placeholders */
--text-inverse: #FBFCFD;          /* Text on dark backgrounds */

--accent: #FDF79E;                /* Primary accent */
--accent-hover: #F5EF8A;          /* Accent hover state */
--accent-muted: rgba(253,247,158,0.15); /* Subtle accent bg */

--border: #DBDEE4;                /* Default border */
--border-hover: #B3B8CA;          /* Hover border */
--border-focus: #FDF79E;          /* Focus ring */
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
| `--shadow-sm`      | `0 2px 8px rgba(41,41,42,0.08)`       | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(41,41,42,0.1)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(41,41,42,0.14)`      | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(41,41,42,0.18)`     | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#FDF79E`     | `#29292A`     | `#FDF79E`           |
| Secondary   | transparent   | `#29292A`     | `#29292A`           |
| Ghost       | transparent   | `#666458`     | none                |
| Danger      | `#B85454`     | `#FFFFFF`     | `#B85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

**States:** hover lifts with shadow, active presses down

### Input Fields

- Background: `#FBFCFD`
- Border: `1px solid #DBDEE4`
- Focus border: `#FDF79E` + ring `0 0 0 3px rgba(253,247,158,0.2)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #DBDEE4`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(253,247,158,0.15)`    | `#666458`   |
| Success   | `rgba(107,138,94,0.1)`      | `#6B8A5E`   |
| Warning   | `rgba(226,168,75,0.1)`      | `#E2A84B`   |
| Error     | `rgba(184,84,84,0.1)`       | `#B85454`   |
| Info      | `rgba(253,247,158,0.15)`    | `#666458`   |

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
- `#29292A` on `#FBFCFD` = **15.2:1** (AAA)
- `#666458` on `#FBFCFD` = **6.8:1** (AA)
- `#FDF79E` on `#FBFCFD` = **1.2:1** (not usable for text — accent only for backgrounds)
- Never use `#DBDEE4` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  /* Core Palette */
  --lemon-dark: #29292A;
  --lemon-dark-light: #3A3A3C;
  --lemon-accent: #FDF79E;
  --lemon-accent-light: #F5EF8A;
  --lemon-body: #666458;
  --lemon-muted: #B3B8CA;
  --lemon-muted-light: #DBDEE4;
  --lemon-surface: #FBFCFD;
  --lemon-card: #FFFFFF;

  /* Semantic */
  --bg-primary: #FBFCFD;
  --bg-secondary: #DBDEE4;
  --bg-tertiary: #B3B8CA;
  --bg-card: #FFFFFF;
  --bg-input: #FBFCFD;

  --text-primary: #29292A;
  --text-secondary: #666458;
  --text-tertiary: #B3B8CA;
  --text-muted: #DBDEE4;
  --text-inverse: #FBFCFD;

  --accent: #FDF79E;
  --accent-hover: #F5EF8A;
  --accent-muted: rgba(253,247,158,0.15);

  --border: #DBDEE4;
  --border-hover: #B3B8CA;
  --border-focus: #FDF79E;

  --success: #6B8A5E;
  --warning: #E2A84B;
  --error: #B85454;
  --info: #FDF79E;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(41,41,42,0.08);
  --shadow-md: 0 4px 16px rgba(41,41,42,0.1);
  --shadow-lg: 0 8px 32px rgba(41,41,42,0.14);
  --shadow-xl: 0 16px 48px rgba(41,41,42,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Lemon Drop Design System v1.0*
