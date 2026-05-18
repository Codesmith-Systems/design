# Iris Design System

> Purple bloom — A rich lavender design system for creative, expressive interfaces.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Accent         | `#8692D2` | Mystic Iris     | Primary actions, links, CTAs  |
| Dark           | `#201D23` | Inkwell Inception| Headers, nav, dark surfaces  |
| Body           | `#905772` | Blackberry Tint | Body text, secondary elements |
| Muted          | `#C0A5D6` | Enchanted Lavender | Borders, muted text, dividers |
| Muted Light    | `#E2DDF6` | Lingering Lilac | Light backgrounds, cards      |
| Surface        | `#F5F3FA` | Mist            | Page background, inputs       |
| Card           | `#FFFFFF` | Pure White      | Card background               |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Dark           | `#201D23` | Primary dark, hero sections   |
| Dark-light     | `#302D33` | Dark hover state              |
| Accent         | `#8692D2` | Primary actions, body text    |
| Accent-lt      | `#96A0DC` | Hover state                   |
| Body           | `#905772` | Secondary elements            |
| Muted          | `#C0A5D6` | Borders, placeholders         |
| Muted Light    | `#E2DDF6` | Card backgrounds, sections    |
| Surface        | `#F5F3FA` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#6B8A5E` | Positive states     |
| Warning  | `#C49A3E` | Caution states      |
| Error    | `#B85454` | Error states        |
| Info     | `#8692D2` | Information (=accent) |

### Semantic Mappings

```css
--bg-primary: #F5F3FA;
--bg-secondary: #E2DDF6;
--bg-tertiary: #C0A5D6;
--bg-card: #FFFFFF;
--bg-input: #F5F3FA;

--text-primary: #201D23;
--text-secondary: #905772;
--text-tertiary: #C0A5D6;
--text-muted: #E2DDF6;
--text-inverse: #F5F3FA;

--accent: #8692D2;
--accent-hover: #96A0DC;
--accent-muted: rgba(134,146,210,0.08);

--border: #E2DDF6;
--border-hover: #C0A5D6;
--border-focus: #8692D2;
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
| `--shadow-sm`      | `0 2px 8px rgba(32,29,35,0.08)`       | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(32,29,35,0.1)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(32,29,35,0.14)`      | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(32,29,35,0.18)`     | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#8692D2`     | `#FFFFFF`     | `#8692D2`           |
| Secondary   | transparent   | `#201D23`     | `#201D23`           |
| Ghost       | transparent   | `#905772`     | none                |
| Danger      | `#B85454`     | `#FFFFFF`     | `#B85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

### Input Fields

- Background: `#F5F3FA`
- Border: `1px solid #E2DDF6`
- Focus border: `#8692D2` + ring `0 0 0 3px rgba(134,146,210,0.12)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #E2DDF6`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(134,146,210,0.08)`    | `#8692D2`   |
| Success   | `rgba(107,138,94,0.1)`      | `#6B8A5E`   |
| Warning   | `rgba(196,154,62,0.1)`      | `#C49A3E`   |
| Error     | `rgba(184,84,84,0.1)`       | `#B85454`   |
| Info      | `rgba(134,146,210,0.1)`     | `#8692D2`   |

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
- `#201D23` on `#F5F3FA` = **15.0:1** (AAA)
- `#905772` on `#F5F3FA` = **5.2:1** (AA)
- Never use `#E2DDF6` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  --iris-dark: #201D23;
  --iris-dark-light: #302D33;
  --iris-accent: #8692D2;
  --iris-accent-light: #96A0DC;
  --iris-body: #905772;
  --iris-muted: #C0A5D6;
  --iris-muted-light: #E2DDF6;
  --iris-surface: #F5F3FA;
  --iris-card: #FFFFFF;

  --bg-primary: #F5F3FA;
  --bg-secondary: #E2DDF6;
  --bg-tertiary: #C0A5D6;
  --bg-card: #FFFFFF;
  --bg-input: #F5F3FA;

  --text-primary: #201D23;
  --text-secondary: #905772;
  --text-tertiary: #C0A5D6;
  --text-muted: #E2DDF6;
  --text-inverse: #F5F3FA;

  --accent: #8692D2;
  --accent-hover: #96A0DC;
  --accent-muted: rgba(134,146,210,0.08);

  --border: #E2DDF6;
  --border-hover: #C0A5D6;
  --border-focus: #8692D2;

  --success: #6B8A5E;
  --warning: #C49A3E;
  --error: #B85454;
  --info: #8692D2;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(32,29,35,0.08);
  --shadow-md: 0 4px 16px rgba(32,29,35,0.1);
  --shadow-lg: 0 8px 32px rgba(32,29,35,0.14);
  --shadow-xl: 0 16px 48px rgba(32,29,35,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Iris Design System v1.0*
