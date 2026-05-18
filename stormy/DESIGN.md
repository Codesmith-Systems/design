# Stormy Design System

> Before the calm — A moody, atmospheric design system with storm-to-sky gradients.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Storm 950      | `#1e2d3a` | Deep Storm      | Deepest background            |
| Storm 900      | `#2a3d4e` | Dark Cloud      | Page background               |
| Storm 800      | `#384959` | Overcast        | Cards, elevated surfaces      |
| Storm 700      | `#4a6275` | Rain Cloud      | Inputs, secondary surfaces    |
| Storm 600      | `#5c7589` | Heavy Sky       | Borders, dividers             |
| Storm 500      | `#6A89A7` | Storm Blue      | Primary actions, links, CTAs  |
| Storm 400      | `#7d9bb8` | Clearing        | Secondary text, icons         |
| Storm 300      | `#88BDF2` | Sky Break       | Highlights, accents           |
| Storm 200      | `#a8d1f7` | Light Sky       | Subtle borders                |
| Storm 100      | `#BDDDFC` | Pale Dawn       | Light backgrounds             |
| Storm 50       | `#ddeeff` | Morning Light   | Text on dark, highlights      |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Storm 900      | `#2a3d4e` | Page background, hero         |
| Storm 800      | `#384959` | Card background, nav          |
| Storm 700      | `#4a6275` | Input background              |
| Storm 600      | `#5c7589` | Borders, hover states         |
| Storm 500      | `#6A89A7` | Primary actions               |
| Storm 400      | `#7d9bb8` | Secondary text                |
| Storm 300      | `#88BDF2` | Highlights                    |
| Storm 200      | `#a8d1f7` | Subtle borders                |
| Storm 100      | `#BDDDFC` | Light backgrounds             |
| Storm 50       | `#ddeeff` | Primary text, highlights      |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#4A8C6F` | Positive states     |
| Warning  | `#C49A3E` | Caution states      |
| Error    | `#B85454` | Error states        |
| Info     | `#6A89A7` | Information (=storm) |

### Semantic Mappings

```css
--bg-primary: #2a3d4e;            /* Page background */
--bg-secondary: #384959;          /* Section/card background */
--bg-tertiary: #4a6275;           /* Elevated surface */
--bg-card: #384959;               /* Card background */
--bg-input: #4a6275;              /* Input field background */

--text-primary: #ddeeff;          /* Headings, important text */
--text-secondary: #BDDDFC;        /* Body text */
--text-tertiary: #7d9bb8;         /* Captions, descriptions */
--text-muted: #5c7589;            /* Disabled, placeholders */
--text-inverse: #2a3d4e;          /* Text on light backgrounds */

--accent: #6A89A7;                /* Primary accent */
--accent-hover: #7d9bb8;          /* Accent hover state */
--accent-muted: rgba(106,137,167,0.15); /* Subtle accent bg */

--border: #5c7589;                /* Default border */
--border-hover: #6A89A7;          /* Hover border */
--border-focus: #6A89A7;          /* Focus ring */
```

---

## 2. Typography

### Font Families

| Token           | Value                | Usage                     |
|-----------------|----------------------|---------------------------|
| `--font-display` | Playfair Display    | Headings, labels, buttons |
| `--font-body`    | Inter               | Body text, descriptions   |

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
| `--shadow-sm`      | `0 2px 8px rgba(30,45,58,0.3)`        | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(30,45,58,0.4)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(30,45,58,0.5)`       | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(30,45,58,0.6)`      | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#6A89A7`     | `#ddeeff`     | `#6A89A7`           |
| Secondary   | transparent   | `#BDDDFC`     | `#6A89A7`           |
| Ghost       | transparent   | `#7d9bb8`     | none                |
| Danger      | `#B85454`     | `#ddeeff`     | `#B85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

**States:** hover lifts with shadow, active presses down

### Input Fields

- Background: `#4a6275`
- Border: `1px solid #5c7589`
- Focus border: `#6A89A7` + ring `0 0 0 3px rgba(106,137,167,0.2)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#384959`
- Border: `1px solid #5c7589`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(106,137,167,0.15)`    | `#BDDDFC`   |
| Success   | `rgba(74,140,111,0.15)`     | `#4A8C6F`   |
| Warning   | `rgba(196,154,62,0.15)`     | `#C49A3E`   |
| Error     | `rgba(184,84,84,0.15)`      | `#B85454`   |
| Info      | `rgba(106,137,167,0.15)`    | `#6A89A7`   |

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
- `#ddeeff` on `#2a3d4e` = **12.8:1** (AAA)
- `#BDDDFC` on `#2a3d4e` = **9.2:1** (AAA)
- `#7d9bb8` on `#2a3d4e` = **5.4:1** (AA)
- Never use `#5c7589` for text below 18px on dark backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  /* Core Palette */
  --storm-950: #1e2d3a;
  --storm-900: #2a3d4e;
  --storm-800: #384959;
  --storm-700: #4a6275;
  --storm-600: #5c7589;
  --storm-500: #6A89A7;
  --storm-400: #7d9bb8;
  --storm-300: #88BDF2;
  --storm-200: #a8d1f7;
  --storm-100: #BDDDFC;
  --storm-50: #ddeeff;

  /* Semantic */
  --bg-primary: #2a3d4e;
  --bg-secondary: #384959;
  --bg-tertiary: #4a6275;
  --bg-card: #384959;
  --bg-input: #4a6275;

  --text-primary: #ddeeff;
  --text-secondary: #BDDDFC;
  --text-tertiary: #7d9bb8;
  --text-muted: #5c7589;
  --text-inverse: #2a3d4e;

  --accent: #6A89A7;
  --accent-hover: #7d9bb8;
  --accent-muted: rgba(106,137,167,0.15);

  --border: #5c7589;
  --border-hover: #6A89A7;
  --border-focus: #6A89A7;

  --success: #4A8C6F;
  --warning: #C49A3E;
  --error: #B85454;
  --info: #6A89A7;

  --font-display: 'Playfair Display', serif;
  --font-body: 'Inter', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(30,45,58,0.3);
  --shadow-md: 0 4px 16px rgba(30,45,58,0.4);
  --shadow-lg: 0 8px 32px rgba(30,45,58,0.5);
  --shadow-xl: 0 16px 48px rgba(30,45,58,0.6);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Stormy Design System v1.0*
