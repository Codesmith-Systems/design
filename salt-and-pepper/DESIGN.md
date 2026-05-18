# Salt and Pepper Design System

> Contrast and code — A minimal monochrome design system with typographic precision.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Salt           | `#FFFFFF` | Pure White      | Page background, cards        |
| Pepper Light   | `#D4D4D4` | Light Pepper    | Borders, muted text, dividers |
| Pepper Mid     | `#B3B3B3` | Mid Pepper      | Secondary text, placeholders  |
| Pepper         | `#2B2B2B` | Deep Pepper     | Headers, nav, primary text    |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Pepper 950     | `#1A1A1A` | Deepest dark, hero            |
| Pepper 900     | `#2B2B2B` | Primary dark, text            |
| Pepper 800     | `#3D3D3D` | Dark hover state              |
| Pepper 700     | `#525252` | Dark secondary                |
| Pepper 600     | `#6B6B6B` | Muted dark                    |
| Pepper 500     | `#858585` | Neutral mid                   |
| Pepper 400     | `#A3A3A3` | Light mid                     |
| Pepper 300     | `#B3B3B3` | Pepper mid                    |
| Pepper 200     | `#C4C4C4` | Light border                  |
| Pepper 100     | `#D4D4D4` | Pepper light                  |
| Pepper 50      | `#E8E8E8` | Subtle background             |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#4A7C6F` | Positive states     |
| Warning  | `#B8943E` | Caution states      |
| Error    | `#A85454` | Error states        |
| Info     | `#2B2B2B` | Information (=pepper) |

### Semantic Mappings

```css
--bg-primary: #FFFFFF;            /* Page background */
--bg-secondary: #E8E8E8;          /* Section/card background */
--bg-tertiary: #D4D4D4;           /* Elevated surface */
--bg-card: #FFFFFF;               /* Card background */
--bg-input: #FFFFFF;              /* Input field background */

--text-primary: #2B2B2B;          /* Headings, important text */
--text-secondary: #525252;        /* Body text */
--text-tertiary: #6B6B6B;         /* Captions, descriptions */
--text-muted: #B3B3B3;            /* Disabled, placeholders */
--text-inverse: #FFFFFF;          /* Text on dark backgrounds */

--accent: #2B2B2B;                /* Primary accent */
--accent-hover: #3D3D3D;          /* Accent hover state */
--accent-muted: rgba(43,43,43,0.06); /* Subtle accent bg */

--border: #D4D4D4;                /* Default border */
--border-hover: #B3B3B3;          /* Hover border */
--border-focus: #2B2B2B;          /* Focus ring */
```

---

## 2. Typography

### Font Families

| Token           | Value                | Usage                     |
|-----------------|----------------------|---------------------------|
| `--font-display` | Space Grotesk       | Headings, labels, buttons |
| `--font-body`    | JetBrains Mono      | Body text, descriptions   |

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
| `--shadow-sm`      | `0 2px 8px rgba(43,43,43,0.06)`       | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(43,43,43,0.08)`      | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(43,43,43,0.12)`      | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(43,43,43,0.16)`     | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#2B2B2B`     | `#FFFFFF`     | `#2B2B2B`           |
| Secondary   | transparent   | `#2B2B2B`     | `#2B2B2B`           |
| Ghost       | transparent   | `#525252`     | none                |
| Danger      | `#A85454`     | `#FFFFFF`     | `#A85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

**States:** hover lifts with shadow, active presses down

### Input Fields

- Background: `#FFFFFF`
- Border: `1px solid #D4D4D4`
- Focus border: `#2B2B2B` + ring `0 0 0 3px rgba(43,43,43,0.1)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #E8E8E8`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(43,43,43,0.06)`       | `#2B2B2B`   |
| Success   | `rgba(74,124,111,0.1)`      | `#4A7C6F`   |
| Warning   | `rgba(184,148,62,0.1)`      | `#B8943E`   |
| Error     | `rgba(168,84,84,0.1)`       | `#A85454`   |
| Info      | `rgba(43,43,43,0.08)`       | `#2B2B2B`   |

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
- `#2B2B2B` on `#FFFFFF` = **14.7:1** (AAA)
- `#525252` on `#FFFFFF` = **7.5:1** (AAA)
- `#6B6B6B` on `#FFFFFF` = **5.1:1** (AA)
- Never use `#B3B3B3` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  /* Core Palette */
  --salt: #FFFFFF;
  --pepper-950: #1A1A1A;
  --pepper-900: #2B2B2B;
  --pepper-800: #3D3D3D;
  --pepper-700: #525252;
  --pepper-600: #6B6B6B;
  --pepper-500: #858585;
  --pepper-400: #A3A3A3;
  --pepper-300: #B3B3B3;
  --pepper-200: #C4C4C4;
  --pepper-100: #D4D4D4;
  --pepper-50: #E8E8E8;

  /* Semantic */
  --bg-primary: #FFFFFF;
  --bg-secondary: #E8E8E8;
  --bg-tertiary: #D4D4D4;
  --bg-card: #FFFFFF;
  --bg-input: #FFFFFF;

  --text-primary: #2B2B2B;
  --text-secondary: #525252;
  --text-tertiary: #6B6B6B;
  --text-muted: #B3B3B3;
  --text-inverse: #FFFFFF;

  --accent: #2B2B2B;
  --accent-hover: #3D3D3D;
  --accent-muted: rgba(43,43,43,0.06);

  --border: #D4D4D4;
  --border-hover: #B3B3B3;
  --border-focus: #2B2B2B;

  --success: #4A7C6F;
  --warning: #B8943E;
  --error: #A85454;
  --info: #2B2B2B;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'JetBrains Mono', monospace;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(43,43,43,0.06);
  --shadow-md: 0 4px 16px rgba(43,43,43,0.08);
  --shadow-lg: 0 8px 32px rgba(43,43,43,0.12);
  --shadow-xl: 0 16px 48px rgba(43,43,43,0.16);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Salt and Pepper Design System v1.0*
