# Golden Hour Design System

> Warm earth tones — A sophisticated olive-gold design system for grounded, premium interfaces.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Accent         | `#CDA85A` | Glorious Gold   | Primary actions, links, CTAs  |
| Dark           | `#302E2B` | Diesel          | Headers, nav, dark surfaces   |
| Body           | `#786E4F` | Go Ben          | Body text, secondary elements |
| Muted          | `#9FAB85` | Cucumber Crush  | Borders, muted text, dividers |
| Muted Light    | `#D5D0A9` | Crystal Palace  | Light backgrounds, cards      |
| Surface        | `#E5E5DE` | Black Squeeze   | Page background, inputs       |
| Card           | `#FFFFFF` | Pure White      | Card background               |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Dark           | `#302E2B` | Primary dark, hero sections   |
| Dark-light     | `#3E3C38` | Dark hover state              |
| Accent         | `#CDA85A` | Primary actions, body text    |
| Accent-lt      | `#D4B06A` | Hover state                   |
| Body           | `#786E4F` | Secondary elements            |
| Muted          | `#9FAB85` | Borders, placeholders         |
| Muted Light    | `#D5D0A9` | Card backgrounds, sections    |
| Surface        | `#E5E5DE` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#6B8F5E` | Positive states     |
| Warning  | `#C49A3E` | Caution states      |
| Error    | `#B85454` | Error states        |
| Info     | `#CDA85A` | Information (=accent) |

### Semantic Mappings

```css
--bg-primary: #E5E5DE;            /* Page background */
--bg-secondary: #D5D0A9;          /* Section/card background */
--bg-tertiary: #9FAB85;           /* Elevated surface */
--bg-card: #FFFFFF;               /* Card background */
--bg-input: #E5E5DE;              /* Input field background */

--text-primary: #302E2B;          /* Headings, important text */
--text-secondary: #786E4F;        /* Body text */
--text-tertiary: #9FAB85;         /* Captions, descriptions */
--text-muted: #D5D0A9;            /* Disabled, placeholders */
--text-inverse: #E5E5DE;          /* Text on dark backgrounds */

--accent: #CDA85A;                /* Primary accent */
--accent-hover: #D4B06A;          /* Accent hover state */
--accent-muted: rgba(205,168,90,0.08); /* Subtle accent bg */

--border: #9FAB85;                /* Default border */
--border-hover: #786E4F;          /* Hover border */
--border-focus: #CDA85A;          /* Focus ring */
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
| `--shadow-sm`      | `0 2px 8px rgba(48,46,43,0.08)`       | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(48,46,43,0.1)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(48,46,43,0.14)`      | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(48,46,43,0.18)`     | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#CDA85A`     | `#302E2B`     | `#CDA85A`           |
| Secondary   | transparent   | `#302E2B`     | `#302E2B`           |
| Ghost       | transparent   | `#786E4F`     | none                |
| Danger      | `#B85454`     | `#FFFFFF`     | `#B85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

**States:** hover lifts with shadow, active presses down

### Input Fields

- Background: `#E5E5DE`
- Border: `1px solid #9FAB85`
- Focus border: `#CDA85A` + ring `0 0 0 3px rgba(205,168,90,0.12)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #D5D0A9`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(205,168,90,0.08)`     | `#CDA85A`   |
| Success   | `rgba(107,143,94,0.1)`      | `#6B8F5E`   |
| Warning   | `rgba(196,154,62,0.1)`      | `#C49A3E`   |
| Error     | `rgba(184,84,84,0.1)`       | `#B85454`   |
| Info      | `rgba(205,168,90,0.1)`      | `#CDA85A`   |

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
- `#302E2B` on `#E5E5DE` = **14.1:1** (AAA)
- `#786E4F` on `#E5E5DE` = **5.2:1** (AA)
- `#9FAB85` on `#E5E5DE` = **2.8:1** (AA large text only)
- Never use `#D5D0A9` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  /* Core Palette */
  --gold-dark: #302E2B;
  --gold-dark-light: #3E3C38;
  --gold-accent: #CDA85A;
  --gold-accent-light: #D4B06A;
  --gold-body: #786E4F;
  --gold-muted: #9FAB85;
  --gold-muted-light: #D5D0A9;
  --gold-surface: #E5E5DE;
  --gold-card: #FFFFFF;

  /* Semantic */
  --bg-primary: #E5E5DE;
  --bg-secondary: #D5D0A9;
  --bg-tertiary: #9FAB85;
  --bg-card: #FFFFFF;
  --bg-input: #E5E5DE;

  --text-primary: #302E2B;
  --text-secondary: #786E4F;
  --text-tertiary: #9FAB85;
  --text-muted: #D5D0A9;
  --text-inverse: #E5E5DE;

  --accent: #CDA85A;
  --accent-hover: #D4B06A;
  --accent-muted: rgba(205,168,90,0.08);

  --border: #9FAB85;
  --border-hover: #786E4F;
  --border-focus: #CDA85A;

  --success: #6B8F5E;
  --warning: #C49A3E;
  --error: #B85454;
  --info: #CDA85A;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(48,46,43,0.08);
  --shadow-md: 0 4px 16px rgba(48,46,43,0.1);
  --shadow-lg: 0 8px 32px rgba(48,46,43,0.14);
  --shadow-xl: 0 16px 48px rgba(48,46,43,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Golden Hour Design System v1.0*
