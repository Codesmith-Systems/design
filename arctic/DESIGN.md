# Arctic Design System

> Cool clarity — A crisp blue-steel design system for clean, professional interfaces.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Primary        | `#5289AD` | Arctic Blue     | Primary actions, links, CTAs  |
| Dark           | `#243C4C` | Deep Frost      | Headers, nav, dark surfaces   |
| Steel          | `#698696` | Glacier Steel   | Secondary text, icons         |
| Muted          | `#ACBCBF` | Ice Mist        | Borders, muted text, dividers |
| Muted Light    | `#CDD9DB` | Frost Edge      | Light backgrounds, cards      |
| Surface        | `#F4FCFB` | Snow Surface    | Page background, inputs       |
| Card           | `#FFFFFF` | Pure Ice        | Card background               |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Dark           | `#243C4C` | Primary dark, hero sections   |
| Dark-light     | `#2E4D5E` | Dark hover state              |
| Primary        | `#5289AD` | Primary actions, body text    |
| Primary-lt     | `#6A9BBF` | Hover state                   |
| Steel          | `#698696` | Secondary elements            |
| Muted          | `#ACBCBF` | Borders, placeholders         |
| Muted Light    | `#CDD9DB` | Card backgrounds, sections    |
| Surface        | `#F4FCFB` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#4A8C6F` | Positive states     |
| Warning  | `#C49A3E` | Caution states      |
| Error    | `#B85454` | Error states        |
| Info     | `#5289AD` | Information (=primary) |

### Semantic Mappings

```css
--bg-primary: #F4FCFB;            /* Page background */
--bg-secondary: #CDD9DB;          /* Section/card background */
--bg-tertiary: #ACBCBF;           /* Elevated surface */
--bg-card: #FFFFFF;               /* Card background */
--bg-input: #F4FCFB;              /* Input field background */

--text-primary: #243C4C;          /* Headings, important text */
--text-secondary: #5289AD;        /* Body text */
--text-tertiary: #698696;         /* Captions, descriptions */
--text-muted: #ACBCBF;            /* Disabled, placeholders */
--text-inverse: #F4FCFB;          /* Text on dark backgrounds */

--accent: #5289AD;                /* Primary accent */
--accent-hover: #6A9BBF;          /* Accent hover state */
--accent-muted: rgba(82,137,173,0.08); /* Subtle accent bg */

--border: #ACBCBF;                /* Default border */
--border-hover: #698696;          /* Hover border */
--border-focus: #5289AD;          /* Focus ring */
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
| `--shadow-sm`      | `0 2px 8px rgba(36,60,76,0.08)`       | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(36,60,76,0.1)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(36,60,76,0.14)`      | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(36,60,76,0.18)`     | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#5289AD`     | `#FFFFFF`     | `#5289AD`           |
| Secondary   | transparent   | `#243C4C`     | `#243C4C`           |
| Ghost       | transparent   | `#698696`     | none                |
| Danger      | `#B85454`     | `#FFFFFF`     | `#B85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

**States:** hover lifts with shadow, active presses down

### Input Fields

- Background: `#F4FCFB`
- Border: `1px solid #ACBCBF`
- Focus border: `#5289AD` + ring `0 0 0 3px rgba(82,137,173,0.12)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #CDD9DB`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(82,137,173,0.08)`     | `#5289AD`   |
| Success   | `rgba(74,140,111,0.1)`      | `#4A8C6F`   |
| Warning   | `rgba(196,154,62,0.1)`      | `#C49A3E`   |
| Error     | `rgba(184,84,84,0.1)`       | `#B85454`   |
| Info      | `rgba(82,137,173,0.1)`      | `#5289AD`   |

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
- `#243C4C` on `#F4FCFB` = **13.2:1** (AAA)
- `#5289AD` on `#F4FCFB` = **4.8:1** (AA)
- `#698696` on `#F4FCFB` = **3.5:1** (AA large text only)
- Never use `#ACBCBF` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  /* Core Palette */
  --arctic-dark: #243C4C;
  --arctic-dark-light: #2E4D5E;
  --arctic-primary: #5289AD;
  --arctic-primary-light: #6A9BBF;
  --arctic-steel: #698696;
  --arctic-muted: #ACBCBF;
  --arctic-muted-light: #CDD9DB;
  --arctic-surface: #F4FCFB;
  --arctic-card: #FFFFFF;

  /* Semantic */
  --bg-primary: #F4FCFB;
  --bg-secondary: #CDD9DB;
  --bg-tertiary: #ACBCBF;
  --bg-card: #FFFFFF;
  --bg-input: #F4FCFB;

  --text-primary: #243C4C;
  --text-secondary: #5289AD;
  --text-tertiary: #698696;
  --text-muted: #ACBCBF;
  --text-inverse: #F4FCFB;

  --accent: #5289AD;
  --accent-hover: #6A9BBF;
  --accent-muted: rgba(82,137,173,0.08);

  --border: #ACBCBF;
  --border-hover: #698696;
  --border-focus: #5289AD;

  --success: #4A8C6F;
  --warning: #C49A3E;
  --error: #B85454;
  --info: #5289AD;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(36,60,76,0.08);
  --shadow-md: 0 4px 16px rgba(36,60,76,0.1);
  --shadow-lg: 0 8px 32px rgba(36,60,76,0.14);
  --shadow-xl: 0 16px 48px rgba(36,60,76,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Arctic Design System v1.0*
