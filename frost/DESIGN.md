# Frost Design System

> Cool clarity — A soft blue-purple design system for calm, professional interfaces.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Accent         | `#634065` | Purple Odyssey  | Primary actions, links, CTAs  |
| Dark           | `#634065` | Purple Odyssey  | Headers, nav, dark surfaces   |
| Body           | `#807389` | Hyacinth Dream  | Body text, secondary elements |
| Muted          | `#9B9FAC` | Adhesion        | Borders, muted text, dividers |
| Muted Light    | `#B1B7C5` | Brother Blue    | Light backgrounds, cards      |
| Surface        | `#E6E8ED` | Cool Frost      | Page background, inputs       |
| Card           | `#FFFFFF` | Pure White      | Card background               |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Dark           | `#634065` | Primary dark, hero sections   |
| Dark-light     | `#735075` | Dark hover state              |
| Accent         | `#634065` | Primary actions, body text    |
| Accent-lt      | `#735075` | Hover state                   |
| Body           | `#807389` | Secondary elements            |
| Muted          | `#9B9FAC` | Borders, placeholders         |
| Muted Light    | `#B1B7C5` | Card backgrounds, sections    |
| Surface        | `#E6E8ED` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#6B8A5E` | Positive states     |
| Warning  | `#C49A3E` | Caution states      |
| Error    | `#B85454` | Error states        |
| Info     | `#634065` | Information (=accent) |

### Semantic Mappings

```css
--bg-primary: #E6E8ED;
--bg-secondary: #B1B7C5;
--bg-tertiary: #9B9FAC;
--bg-card: #FFFFFF;
--bg-input: #E6E8ED;

--text-primary: #634065;
--text-secondary: #807389;
--text-tertiary: #9B9FAC;
--text-muted: #B1B7C5;
--text-inverse: #E6E8ED;

--accent: #634065;
--accent-hover: #735075;
--accent-muted: rgba(99,64,101,0.08);

--border: #B1B7C5;
--border-hover: #9B9FAC;
--border-focus: #634065;
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
| `--shadow-sm`      | `0 2px 8px rgba(99,64,101,0.08)`      | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(99,64,101,0.1)`      | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(99,64,101,0.14)`     | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(99,64,101,0.18)`    | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#634065`     | `#FFFFFF`     | `#634065`           |
| Secondary   | transparent   | `#634065`     | `#634065`           |
| Ghost       | transparent   | `#807389`     | none                |
| Danger      | `#B85454`     | `#FFFFFF`     | `#B85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

### Input Fields

- Background: `#E6E8ED`
- Border: `1px solid #B1B7C5`
- Focus border: `#634065` + ring `0 0 0 3px rgba(99,64,101,0.12)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #B1B7C5`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(99,64,101,0.08)`      | `#634065`   |
| Success   | `rgba(107,138,94,0.1)`      | `#6B8A5E`   |
| Warning   | `rgba(196,154,62,0.1)`      | `#C49A3E`   |
| Error     | `rgba(184,84,84,0.1)`       | `#B85454`   |
| Info      | `rgba(99,64,101,0.1)`       | `#634065`   |

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
- `#634065` on `#E6E8ED` = **7.8:1** (AA)
- `#807389` on `#E6E8ED` = **4.2:1** (AA large text)
- Never use `#B1B7C5` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  --frost-dark: #634065;
  --frost-dark-light: #735075;
  --frost-accent: #634065;
  --frost-accent-light: #735075;
  --frost-body: #807389;
  --frost-muted: #9B9FAC;
  --frost-muted-light: #B1B7C5;
  --frost-surface: #E6E8ED;
  --frost-card: #FFFFFF;

  --bg-primary: #E6E8ED;
  --bg-secondary: #B1B7C5;
  --bg-tertiary: #9B9FAC;
  --bg-card: #FFFFFF;
  --bg-input: #E6E8ED;

  --text-primary: #634065;
  --text-secondary: #807389;
  --text-tertiary: #9B9FAC;
  --text-muted: #B1B7C5;
  --text-inverse: #E6E8ED;

  --accent: #634065;
  --accent-hover: #735075;
  --accent-muted: rgba(99,64,101,0.08);

  --border: #B1B7C5;
  --border-hover: #9B9FAC;
  --border-focus: #634065;

  --success: #6B8A5E;
  --warning: #C49A3E;
  --error: #B85454;
  --info: #634065;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(99,64,101,0.08);
  --shadow-md: 0 4px 16px rgba(99,64,101,0.1);
  --shadow-lg: 0 8px 32px rgba(99,64,101,0.14);
  --shadow-xl: 0 16px 48px rgba(99,64,101,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Frost Design System v1.0*
