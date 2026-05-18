# Winter Chill Design System

> Frozen stillness — A dark-mode design system with icy teal tones and crisp clarity.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Winter 50      | `#E8F6F8` | Frost Mist      | Text on dark, highlights      |
| Winter 100     | `#B8E3E9` | Ice Crystal     | Light accents                 |
| Winter 200     | `#93B1B5` | Frozen Lake     | Subtle borders                |
| Winter 300     | `#4F7C82` | Deep Ice        | Primary actions, links, CTAs  |
| Winter 400     | `#0B2E33` | Arctic Night    | Page background, dark surfaces|

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Winter 400     | `#0B2E33` | Page background, hero         |
| Winter 400-lt  | `#0E3A40` | Dark hover state              |
| Winter 300     | `#4F7C82` | Primary actions               |
| Winter 300-lt  | `#6A9499` | Hover state                   |
| Winter 200     | `#93B1B5` | Secondary elements            |
| Winter 100     | `#B8E3E9` | Light accents                 |
| Winter 50      | `#E8F6F8` | Primary text, highlights      |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#4ADE80` | Positive states     |
| Warning  | `#FBBF24` | Caution states      |
| Error    | `#F87171` | Error states        |
| Info     | `#4F7C82` | Information (=winter) |

### Semantic Mappings

```css
--bg-primary: #0B2E33;            /* Page background */
--bg-secondary: #0E3A40;          /* Section/card background */
--bg-tertiary: #13454B;           /* Elevated surface */
--bg-card: #0E3A40;               /* Card background */
--bg-input: #13454B;              /* Input field background */

--text-primary: #E8F6F8;          /* Headings, important text */
--text-secondary: #B8E3E9;        /* Body text */
--text-tertiary: #93B1B5;         /* Captions, descriptions */
--text-muted: #4F7C82;            /* Disabled, placeholders */
--text-inverse: #0B2E33;          /* Text on light backgrounds */

--accent: #4F7C82;                /* Primary accent */
--accent-hover: #6A9499;          /* Accent hover state */
--accent-muted: rgba(79,124,130,0.15); /* Subtle accent bg */

--border: #1A5055;                /* Default border */
--border-hover: #4F7C82;          /* Hover border */
--border-focus: #4F7C82;          /* Focus ring */
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
| `--shadow-sm`      | `0 2px 8px rgba(11,46,51,0.3)`        | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(11,46,51,0.4)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(11,46,51,0.5)`       | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(11,46,51,0.6)`      | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#4F7C82`     | `#E8F6F8`     | `#4F7C82`           |
| Secondary   | transparent   | `#B8E3E9`     | `#4F7C82`           |
| Ghost       | transparent   | `#93B1B5`     | none                |
| Danger      | `#F87171`     | `#0B2E33`     | `#F87171`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

**States:** hover lifts with shadow, active presses down

### Input Fields

- Background: `#13454B`
- Border: `1px solid #1A5055`
- Focus border: `#4F7C82` + ring `0 0 0 3px rgba(79,124,130,0.2)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#0E3A40`
- Border: `1px solid #1A5055`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(79,124,130,0.15)`     | `#B8E3E9`   |
| Success   | `rgba(74,222,128,0.15)`     | `#4ADE80`   |
| Warning   | `rgba(251,191,36,0.15)`     | `#FBBF24`   |
| Error     | `rgba(248,113,113,0.15)`    | `#F87171`   |
| Info      | `rgba(79,124,130,0.15)`     | `#4F7C82`   |

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
- `#E8F6F8` on `#0B2E33` = **14.2:1** (AAA)
- `#B8E3E9` on `#0B2E33` = **9.8:1** (AAA)
- `#93B1B5` on `#0B2E33` = **5.2:1** (AA)
- Never use `#4F7C82` for text below 18px on dark backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  /* Core Palette */
  --winter-50: #E8F6F8;
  --winter-100: #B8E3E9;
  --winter-200: #93B1B5;
  --winter-300: #4F7C82;
  --winter-300-light: #6A9499;
  --winter-400: #0B2E33;
  --winter-400-light: #0E3A40;
  --winter-border: #1A5055;
  --winter-card: #0E3A40;

  /* Semantic */
  --bg-primary: #0B2E33;
  --bg-secondary: #0E3A40;
  --bg-tertiary: #13454B;
  --bg-card: #0E3A40;
  --bg-input: #13454B;

  --text-primary: #E8F6F8;
  --text-secondary: #B8E3E9;
  --text-tertiary: #93B1B5;
  --text-muted: #4F7C82;
  --text-inverse: #0B2E33;

  --accent: #4F7C82;
  --accent-hover: #6A9499;
  --accent-muted: rgba(79,124,130,0.15);

  --border: #1A5055;
  --border-hover: #4F7C82;
  --border-focus: #4F7C82;

  --success: #4ADE80;
  --warning: #FBBF24;
  --error: #F87171;
  --info: #4F7C82;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(11,46,51,0.3);
  --shadow-md: 0 4px 16px rgba(11,46,51,0.4);
  --shadow-lg: 0 8px 32px rgba(11,46,51,0.5);
  --shadow-xl: 0 16px 48px rgba(11,46,51,0.6);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Winter Chill Design System v1.0*
