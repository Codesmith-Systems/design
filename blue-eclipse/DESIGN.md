# Blue Eclipse Design System

> Into the void — A deep indigo design system built for dark-mode-first interfaces.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Eclipse 900    | `#0F0E47` | Deep Void       | Background, darkest surfaces  |
| Eclipse 800    | `#1A1A52` | Night Sky       | Cards, elevated surfaces      |
| Eclipse 700    | `#272757` | Dark Nebula     | Inputs, secondary surfaces    |
| Eclipse 600    | `#3B3B6E` | Twilight        | Borders, dividers             |
| Eclipse 500    | `#505081` | Mid Eclipse     | Secondary text, icons         |
| Eclipse 400    | `#6B6B97` | Starlight       | Tertiary text, muted elements |
| Eclipse 300    | `#8686AC` | Soft Glow       | Placeholder text              |
| Eclipse 200    | `#A5A5C4` | Moonbeam        | Subtle borders                |
| Eclipse 100    | `#C4C4DC` | Pale Light      | Light accents                 |
| Eclipse 50     | `#EDEDF6` | Dawn            | Text on dark, highlights      |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Eclipse 900    | `#0F0E47` | Page background, hero         |
| Eclipse 800    | `#1A1A52` | Card background, nav          |
| Eclipse 700    | `#272757` | Input background              |
| Eclipse 600    | `#3B3B6E` | Borders, hover states         |
| Eclipse 500    | `#505081` | Secondary text                |
| Eclipse 400    | `#6B6B97` | Tertiary elements             |
| Eclipse 300    | `#8686AC` | Muted text                    |
| Eclipse 200    | `#A5A5C4` | Subtle borders                |
| Eclipse 100    | `#C4C4DC` | Light accents                 |
| Eclipse 50     | `#EDEDF6` | Primary text, highlights      |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#4ADE80` | Positive states     |
| Warning  | `#FBBF24` | Caution states      |
| Error    | `#F87171` | Error states        |
| Info     | `#6B6B97` | Information         |

### Semantic Mappings

```css
--bg-primary: #0F0E47;            /* Page background */
--bg-secondary: #1A1A52;          /* Section/card background */
--bg-tertiary: #272757;           /* Elevated surface */
--bg-card: #1A1A52;               /* Card background */
--bg-input: #272757;              /* Input field background */

--text-primary: #EDEDF6;          /* Headings, important text */
--text-secondary: #C4C4DC;        /* Body text */
--text-tertiary: #8686AC;         /* Captions, descriptions */
--text-muted: #6B6B97;            /* Disabled, placeholders */
--text-inverse: #0F0E47;          /* Text on light backgrounds */

--accent: #6B6B97;                /* Primary accent */
--accent-hover: #8686AC;          /* Accent hover state */
--accent-muted: rgba(107,107,151,0.15); /* Subtle accent bg */

--border: #3B3B6E;                /* Default border */
--border-hover: #505081;          /* Hover border */
--border-focus: #6B6B97;          /* Focus ring */
```

---

## 2. Typography

### Font Families

| Token           | Value             | Usage                     |
|-----------------|-------------------|---------------------------|
| `--font-display` | Inter            | Headings, labels, buttons |
| `--font-body`    | Inter            | Body text, descriptions   |

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
| `--shadow-sm`      | `0 2px 8px rgba(15,14,71,0.3)`        | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(15,14,71,0.4)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(15,14,71,0.5)`       | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(15,14,71,0.6)`      | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#6B6B97`     | `#EDEDF6`     | `#6B6B97`           |
| Secondary   | transparent   | `#C4C4DC`     | `#6B6B97`           |
| Ghost       | transparent   | `#8686AC`     | none                |
| Danger      | `#F87171`     | `#0F0E47`     | `#F87171`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

**States:** hover lifts with shadow, active presses down

### Input Fields

- Background: `#272757`
- Border: `1px solid #3B3B6E`
- Focus border: `#6B6B97` + ring `0 0 0 3px rgba(107,107,151,0.2)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#1A1A52`
- Border: `1px solid #3B3B6E`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(107,107,151,0.15)`    | `#C4C4DC`   |
| Success   | `rgba(74,222,128,0.15)`     | `#4ADE80`   |
| Warning   | `rgba(251,191,36,0.15)`     | `#FBBF24`   |
| Error     | `rgba(248,113,113,0.15)`    | `#F87171`   |
| Info      | `rgba(107,107,151,0.15)`    | `#6B6B97`   |

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
- `#EDEDF6` on `#0F0E47` = **15.2:1** (AAA)
- `#C4C4DC` on `#0F0E47` = **10.1:1** (AAA)
- `#8686AC` on `#0F0E47` = **5.8:1** (AA)
- Never use `#6B6B97` for text below 18px on dark backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  /* Core Palette */
  --eclipse-900: #0F0E47;
  --eclipse-800: #1A1A52;
  --eclipse-700: #272757;
  --eclipse-600: #3B3B6E;
  --eclipse-500: #505081;
  --eclipse-400: #6B6B97;
  --eclipse-300: #8686AC;
  --eclipse-200: #A5A5C4;
  --eclipse-100: #C4C4DC;
  --eclipse-50: #EDEDF6;

  /* Semantic */
  --bg-primary: #0F0E47;
  --bg-secondary: #1A1A52;
  --bg-tertiary: #272757;
  --bg-card: #1A1A52;
  --bg-input: #272757;

  --text-primary: #EDEDF6;
  --text-secondary: #C4C4DC;
  --text-tertiary: #8686AC;
  --text-muted: #6B6B97;
  --text-inverse: #0F0E47;

  --accent: #6B6B97;
  --accent-hover: #8686AC;
  --accent-muted: rgba(107,107,151,0.15);

  --border: #3B3B6E;
  --border-hover: #505081;
  --border-focus: #6B6B97;

  --success: #4ADE80;
  --warning: #FBBF24;
  --error: #F87171;
  --info: #6B6B97;

  --font-display: 'Inter', sans-serif;
  --font-body: 'Inter', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(15,14,71,0.3);
  --shadow-md: 0 4px 16px rgba(15,14,71,0.4);
  --shadow-lg: 0 8px 32px rgba(15,14,71,0.5);
  --shadow-xl: 0 16px 48px rgba(15,14,71,0.6);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Blue Eclipse Design System v1.0*
