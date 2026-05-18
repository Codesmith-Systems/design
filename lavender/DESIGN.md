# Lavender Haze Design System

> Soft elegance — A muted lavender design system for calm, refined interfaces.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Accent         | `#A79EBE` | Evening Slipper | Primary actions, links, CTAs  |
| Dark           | `#2E3133` | Cod Grey        | Headers, nav, dark surfaces   |
| Body           | `#76757A` | Astrogranite    | Body text, secondary elements |
| Muted          | `#CCC6D2` | Chrome Chalice  | Borders, muted text, dividers |
| Muted Light    | `#DFD8F0` | Japan Blush     | Light backgrounds, cards      |
| Surface        | `#FAFAF7` | Unbleached      | Page background, inputs       |
| Card           | `#FFFFFF` | Pure White      | Card background               |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Dark           | `#2E3133` | Primary dark, hero sections   |
| Dark-light     | `#3E4143` | Dark hover state              |
| Accent         | `#A79EBE` | Primary actions, body text    |
| Accent-lt      | `#B8B0CC` | Hover state                   |
| Body           | `#76757A` | Secondary elements            |
| Muted          | `#CCC6D2` | Borders, placeholders         |
| Muted Light    | `#DFD8F0` | Card backgrounds, sections    |
| Surface        | `#FAFAF7` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#6B8A5E` | Positive states     |
| Warning  | `#C49A3E` | Caution states      |
| Error    | `#B85454` | Error states        |
| Info     | `#A79EBE` | Information (=accent) |

### Semantic Mappings

```css
--bg-primary: #FAFAF7;
--bg-secondary: #DFD8F0;
--bg-tertiary: #CCC6D2;
--bg-card: #FFFFFF;
--bg-input: #FAFAF7;

--text-primary: #2E3133;
--text-secondary: #76757A;
--text-tertiary: #A79EBE;
--text-muted: #CCC6D2;
--text-inverse: #FAFAF7;

--accent: #A79EBE;
--accent-hover: #B8B0CC;
--accent-muted: rgba(167,158,190,0.08);

--border: #CCC6D2;
--border-hover: #A79EBE;
--border-focus: #A79EBE;
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
| `--shadow-sm`      | `0 2px 8px rgba(46,49,51,0.08)`       | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(46,49,51,0.1)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(46,49,51,0.14)`      | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(46,49,51,0.18)`     | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#A79EBE`     | `#FFFFFF`     | `#A79EBE`           |
| Secondary   | transparent   | `#2E3133`     | `#2E3133`           |
| Ghost       | transparent   | `#76757A`     | none                |
| Danger      | `#B85454`     | `#FFFFFF`     | `#B85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

### Input Fields

- Background: `#FAFAF7`
- Border: `1px solid #CCC6D2`
- Focus border: `#A79EBE` + ring `0 0 0 3px rgba(167,158,190,0.12)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #DFD8F0`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(167,158,190,0.08)`    | `#A79EBE`   |
| Success   | `rgba(107,138,94,0.1)`      | `#6B8A5E`   |
| Warning   | `rgba(196,154,62,0.1)`      | `#C49A3E`   |
| Error     | `rgba(184,84,84,0.1)`       | `#B85454`   |
| Info      | `rgba(167,158,190,0.1)`     | `#A79EBE`   |

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
- `#2E3133` on `#FAFAF7` = **14.5:1** (AAA)
- `#76757A` on `#FAFAF7` = **5.5:1** (AA)
- Never use `#DFD8F0` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  --lavender-dark: #2E3133;
  --lavender-dark-light: #3E4143;
  --lavender-accent: #A79EBE;
  --lavender-accent-light: #B8B0CC;
  --lavender-body: #76757A;
  --lavender-muted: #CCC6D2;
  --lavender-muted-light: #DFD8F0;
  --lavender-surface: #FAFAF7;
  --lavender-card: #FFFFFF;

  --bg-primary: #FAFAF7;
  --bg-secondary: #DFD8F0;
  --bg-tertiary: #CCC6D2;
  --bg-card: #FFFFFF;
  --bg-input: #FAFAF7;

  --text-primary: #2E3133;
  --text-secondary: #76757A;
  --text-tertiary: #A79EBE;
  --text-muted: #CCC6D2;
  --text-inverse: #FAFAF7;

  --accent: #A79EBE;
  --accent-hover: #B8B0CC;
  --accent-muted: rgba(167,158,190,0.08);

  --border: #CCC6D2;
  --border-hover: #A79EBE;
  --border-focus: #A79EBE;

  --success: #6B8A5E;
  --warning: #C49A3E;
  --error: #B85454;
  --info: #A79EBE;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(46,49,51,0.08);
  --shadow-md: 0 4px 16px rgba(46,49,51,0.1);
  --shadow-lg: 0 8px 32px rgba(46,49,51,0.14);
  --shadow-xl: 0 16px 48px rgba(46,49,51,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Lavender Haze Design System v1.0*
