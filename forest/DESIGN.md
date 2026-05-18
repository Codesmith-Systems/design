# Forest Design System

> Deep woods — A rich teal-green design system for immersive, natural interfaces.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Accent         | `#D5D016` | Sun Flooded Woods | Primary actions, links, CTAs |
| Dark           | `#141412` | Dark Veil       | Headers, nav, dark surfaces   |
| Body           | `#4F504A` | Subterrain Kingdom | Body text, secondary elements |
| Muted          | `#818B85` | Mummy's Tomb    | Borders, muted text, dividers |
| Muted Light    | `#C3CDCA` | Rediscover      | Light backgrounds, cards      |
| Surface        | `#F0F2F1` | Mist            | Page background, inputs       |
| Card           | `#FFFFFF` | Pure White      | Card background               |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Dark           | `#141412` | Primary dark, hero sections   |
| Dark-light     | `#242422` | Dark hover state              |
| Accent         | `#D5D016` | Primary actions, body text    |
| Accent-lt      | `#E0DB20` | Hover state                   |
| Body           | `#4F504A` | Secondary elements            |
| Muted          | `#818B85` | Borders, placeholders         |
| Muted Light    | `#C3CDCA` | Card backgrounds, sections    |
| Surface        | `#F0F2F1` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#099191` | Positive states     |
| Warning  | `#C49A3E` | Caution states      |
| Error    | `#B85454` | Error states        |
| Info     | `#D5D016` | Information (=accent) |

### Semantic Mappings

```css
--bg-primary: #F0F2F1;
--bg-secondary: #C3CDCA;
--bg-tertiary: #818B85;
--bg-card: #FFFFFF;
--bg-input: #F0F2F1;

--text-primary: #141412;
--text-secondary: #4F504A;
--text-tertiary: #818B85;
--text-muted: #C3CDCA;
--text-inverse: #F0F2F1;

--accent: #D5D016;
--accent-hover: #E0DB20;
--accent-muted: rgba(213,208,22,0.08);

--border: #C3CDCA;
--border-hover: #818B85;
--border-focus: #D5D016;
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
| `--shadow-sm`      | `0 2px 8px rgba(20,20,18,0.08)`       | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(20,20,18,0.1)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(20,20,18,0.14)`      | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(20,20,18,0.18)`     | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#D5D016`     | `#141412`     | `#D5D016`           |
| Secondary   | transparent   | `#141412`     | `#141412`           |
| Ghost       | transparent   | `#4F504A`     | none                |
| Danger      | `#B85454`     | `#FFFFFF`     | `#B85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

### Input Fields

- Background: `#F0F2F1`
- Border: `1px solid #C3CDCA`
- Focus border: `#D5D016` + ring `0 0 0 3px rgba(213,208,22,0.12)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #C3CDCA`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(213,208,22,0.08)`     | `#4F504A`   |
| Success   | `rgba(9,145,145,0.1)`       | `#099191`   |
| Warning   | `rgba(196,154,62,0.1)`      | `#C49A3E`   |
| Error     | `rgba(184,84,84,0.1)`       | `#B85454`   |
| Info      | `rgba(213,208,22,0.08)`     | `#4F504A`   |

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
- `#141412` on `#F0F2F1` = **15.8:1** (AAA)
- `#4F504A` on `#F0F2F1` = **6.8:1** (AA)
- Never use `#C3CDCA` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  --forest-dark: #141412;
  --forest-dark-light: #242422;
  --forest-accent: #D5D016;
  --forest-accent-light: #E0DB20;
  --forest-body: #4F504A;
  --forest-muted: #818B85;
  --forest-muted-light: #C3CDCA;
  --forest-surface: #F0F2F1;
  --forest-card: #FFFFFF;

  --bg-primary: #F0F2F1;
  --bg-secondary: #C3CDCA;
  --bg-tertiary: #818B85;
  --bg-card: #FFFFFF;
  --bg-input: #F0F2F1;

  --text-primary: #141412;
  --text-secondary: #4F504A;
  --text-tertiary: #818B85;
  --text-muted: #C3CDCA;
  --text-inverse: #F0F2F1;

  --accent: #D5D016;
  --accent-hover: #E0DB20;
  --accent-muted: rgba(213,208,22,0.08);

  --border: #C3CDCA;
  --border-hover: #818B85;
  --border-focus: #D5D016;

  --success: #099191;
  --warning: #C49A3E;
  --error: #B85454;
  --info: #D5D016;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(20,20,18,0.08);
  --shadow-md: 0 4px 16px rgba(20,20,18,0.1);
  --shadow-lg: 0 8px 32px rgba(20,20,18,0.14);
  --shadow-xl: 0 16px 48px rgba(20,20,18,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Forest Design System v1.0*
