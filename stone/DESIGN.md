# Stone Design System

> Solid foundation — A monochrome grey design system for clean, professional interfaces.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Accent         | `#82827D` | Grey Pepper     | Primary actions, links, CTAs  |
| Dark           | `#0A0C0D` | Black Wash      | Headers, nav, dark surfaces   |
| Body           | `#4E4F4D` | Black Oak       | Body text, secondary elements |
| Muted          | `#ADADA7` | Cool Granite    | Borders, muted text, dividers |
| Muted Light    | `#C3C3BD` | Grey Nickel     | Light backgrounds, cards      |
| Surface        | `#E8E8E6` | Mist            | Page background, inputs       |
| Card           | `#FFFFFF` | Pure White      | Card background               |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Dark           | `#0A0C0D` | Primary dark, hero sections   |
| Dark-light     | `#1A1C1D` | Dark hover state              |
| Accent         | `#82827D` | Primary actions, body text    |
| Accent-lt      | `#92928D` | Hover state                   |
| Body           | `#4E4F4D` | Secondary elements            |
| Muted          | `#ADADA7` | Borders, placeholders         |
| Muted Light    | `#C3C3BD` | Card backgrounds, sections    |
| Surface        | `#E8E8E6` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#6B8A5E` | Positive states     |
| Warning  | `#C49A3E` | Caution states      |
| Error    | `#B85454` | Error states        |
| Info     | `#82827D` | Information (=accent) |

### Semantic Mappings

```css
--bg-primary: #E8E8E6;
--bg-secondary: #C3C3BD;
--bg-tertiary: #ADADA7;
--bg-card: #FFFFFF;
--bg-input: #E8E8E6;

--text-primary: #0A0C0D;
--text-secondary: #4E4F4D;
--text-tertiary: #ADADA7;
--text-muted: #C3C3BD;
--text-inverse: #E8E8E6;

--accent: #82827D;
--accent-hover: #92928D;
--accent-muted: rgba(130,130,125,0.08);

--border: #C3C3BD;
--border-hover: #ADADA7;
--border-focus: #82827D;
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
| `--shadow-sm`      | `0 2px 8px rgba(10,12,13,0.08)`       | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(10,12,13,0.1)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(10,12,13,0.14)`      | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(10,12,13,0.18)`     | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#82827D`     | `#FFFFFF`     | `#82827D`           |
| Secondary   | transparent   | `#0A0C0D`     | `#0A0C0D`           |
| Ghost       | transparent   | `#4E4F4D`     | none                |
| Danger      | `#B85454`     | `#FFFFFF`     | `#B85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

### Input Fields

- Background: `#E8E8E6`
- Border: `1px solid #C3C3BD`
- Focus border: `#82827D` + ring `0 0 0 3px rgba(130,130,125,0.12)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #C3C3BD`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(130,130,125,0.08)`    | `#82827D`   |
| Success   | `rgba(107,138,94,0.1)`      | `#6B8A5E`   |
| Warning   | `rgba(196,154,62,0.1)`      | `#C49A3E`   |
| Error     | `rgba(184,84,84,0.1)`       | `#B85454`   |
| Info      | `rgba(130,130,125,0.1)`     | `#82827D`   |

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
- `#0A0C0D` on `#E8E8E6` = **15.5:1** (AAA)
- `#4E4F4D` on `#E8E8E6` = **6.2:1** (AA)
- Never use `#C3C3BD` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  --stone-dark: #0A0C0D;
  --stone-dark-light: #1A1C1D;
  --stone-accent: #82827D;
  --stone-accent-light: #92928D;
  --stone-body: #4E4F4D;
  --stone-muted: #ADADA7;
  --stone-muted-light: #C3C3BD;
  --stone-surface: #E8E8E6;
  --stone-card: #FFFFFF;

  --bg-primary: #E8E8E6;
  --bg-secondary: #C3C3BD;
  --bg-tertiary: #ADADA7;
  --bg-card: #FFFFFF;
  --bg-input: #E8E8E6;

  --text-primary: #0A0C0D;
  --text-secondary: #4E4F4D;
  --text-tertiary: #ADADA7;
  --text-muted: #C3C3BD;
  --text-inverse: #E8E8E6;

  --accent: #82827D;
  --accent-hover: #92928D;
  --accent-muted: rgba(130,130,125,0.08);

  --border: #C3C3BD;
  --border-hover: #ADADA7;
  --border-focus: #82827D;

  --success: #6B8A5E;
  --warning: #C49A3E;
  --error: #B85454;
  --info: #82827D;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(10,12,13,0.08);
  --shadow-md: 0 4px 16px rgba(10,12,13,0.1);
  --shadow-lg: 0 8px 32px rgba(10,12,13,0.14);
  --shadow-xl: 0 16px 48px rgba(10,12,13,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Stone Design System v1.0*
