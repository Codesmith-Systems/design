# Moonlight Design System

> Midnight glow — A dark-mode design system with deep violet tones and ethereal light.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Moonlight 950  | `#080814` | Absolute Night  | Deepest background            |
| Moonlight 900  | `#0D0D1F` | Dark Sky        | Page background               |
| Moonlight 800  | `#141433` | Midnight        | Cards, elevated surfaces      |
| Moonlight 700  | `#1E1E4D` | Deep Violet     | Inputs, secondary surfaces    |
| Moonlight 600  | `#292966` | Night Bloom     | Borders, dividers             |
| Moonlight 500  | `#404080` | Moon Base       | Secondary text, icons         |
| Moonlight 400  | `#5C5C99` | Twilight Glow   | Tertiary text, muted elements |
| Moonlight 300  | `#7A7AAA` | Silver Moon     | Placeholder text              |
| Moonlight 200  | `#A3A3CC` | Moonbeam        | Subtle borders                |
| Moonlight 100  | `#CCCCFF` | Pale Moon       | Light accents                 |
| Moonlight 50   | `#E8E8F5` | Dawn Light      | Text on dark, highlights      |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Moonlight 900  | `#0D0D1F` | Page background, hero         |
| Moonlight 800  | `#141433` | Card background, nav          |
| Moonlight 700  | `#1E1E4D` | Input background              |
| Moonlight 600  | `#292966` | Borders, hover states         |
| Moonlight 500  | `#404080` | Secondary text                |
| Moonlight 400  | `#5C5C99` | Tertiary elements             |
| Moonlight 300  | `#7A7AAA` | Muted text                    |
| Moonlight 200  | `#A3A3CC` | Subtle borders                |
| Moonlight 100  | `#CCCCFF` | Light accents                 |
| Moonlight 50   | `#E8E8F5` | Primary text, highlights      |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#4ADE80` | Positive states     |
| Warning  | `#FBBF24` | Caution states      |
| Error    | `#F87171` | Error states        |
| Info     | `#5C5C99` | Information         |

### Semantic Mappings

```css
--bg-primary: #0D0D1F;            /* Page background */
--bg-secondary: #141433;          /* Section/card background */
--bg-tertiary: #1E1E4D;           /* Elevated surface */
--bg-card: #141433;               /* Card background */
--bg-input: #1E1E4D;              /* Input field background */

--text-primary: #E8E8F5;          /* Headings, important text */
--text-secondary: #CCCCFF;        /* Body text */
--text-tertiary: #7A7AAA;         /* Captions, descriptions */
--text-muted: #5C5C99;            /* Disabled, placeholders */
--text-inverse: #0D0D1F;          /* Text on light backgrounds */

--accent: #5C5C99;                /* Primary accent */
--accent-hover: #7A7AAA;          /* Accent hover state */
--accent-muted: rgba(92,92,153,0.15); /* Subtle accent bg */

--border: #292966;                /* Default border */
--border-hover: #404080;          /* Hover border */
--border-focus: #5C5C99;          /* Focus ring */
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
| `--shadow-sm`      | `0 2px 8px rgba(8,8,20,0.3)`          | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(8,8,20,0.4)`         | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(8,8,20,0.5)`         | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(8,8,20,0.6)`        | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#5C5C99`     | `#E8E8F5`     | `#5C5C99`           |
| Secondary   | transparent   | `#CCCCFF`     | `#5C5C99`           |
| Ghost       | transparent   | `#7A7AAA`     | none                |
| Danger      | `#F87171`     | `#0D0D1F`     | `#F87171`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

**States:** hover lifts with shadow, active presses down

### Input Fields

- Background: `#1E1E4D`
- Border: `1px solid #292966`
- Focus border: `#5C5C99` + ring `0 0 0 3px rgba(92,92,153,0.2)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#141433`
- Border: `1px solid #292966`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(92,92,153,0.15)`      | `#CCCCFF`   |
| Success   | `rgba(74,222,128,0.15)`     | `#4ADE80`   |
| Warning   | `rgba(251,191,36,0.15)`     | `#FBBF24`   |
| Error     | `rgba(248,113,113,0.15)`    | `#F87171`   |
| Info      | `rgba(92,92,153,0.15)`      | `#5C5C99`   |

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
- `#E8E8F5` on `#0D0D1F` = **15.8:1** (AAA)
- `#CCCCFF` on `#0D0D1F` = **11.2:1** (AAA)
- `#7A7AAA` on `#0D0D1F` = **5.6:1** (AA)
- Never use `#5C5C99` for text below 18px on dark backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  /* Core Palette */
  --moonlight-950: #080814;
  --moonlight-900: #0D0D1F;
  --moonlight-800: #141433;
  --moonlight-700: #1E1E4D;
  --moonlight-600: #292966;
  --moonlight-500: #404080;
  --moonlight-400: #5C5C99;
  --moonlight-300: #7A7AAA;
  --moonlight-200: #A3A3CC;
  --moonlight-100: #CCCCFF;
  --moonlight-50: #E8E8F5;

  /* Semantic */
  --bg-primary: #0D0D1F;
  --bg-secondary: #141433;
  --bg-tertiary: #1E1E4D;
  --bg-card: #141433;
  --bg-input: #1E1E4D;

  --text-primary: #E8E8F5;
  --text-secondary: #CCCCFF;
  --text-tertiary: #7A7AAA;
  --text-muted: #5C5C99;
  --text-inverse: #0D0D1F;

  --accent: #5C5C99;
  --accent-hover: #7A7AAA;
  --accent-muted: rgba(92,92,153,0.15);

  --border: #292966;
  --border-hover: #404080;
  --border-focus: #5C5C99;

  --success: #4ADE80;
  --warning: #FBBF24;
  --error: #F87171;
  --info: #5C5C99;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(8,8,20,0.3);
  --shadow-md: 0 4px 16px rgba(8,8,20,0.4);
  --shadow-lg: 0 8px 32px rgba(8,8,20,0.5);
  --shadow-xl: 0 16px 48px rgba(8,8,20,0.6);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Moonlight Design System v1.0*
