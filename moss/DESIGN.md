# Moss Design System

> Fresh growth — A soft green design system for organic, natural interfaces.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Accent         | `#CEE9BD` | Toxic Essence   | Primary actions, links, CTAs  |
| Dark           | `#050504` | Black Metal     | Headers, nav, dark surfaces   |
| Body           | `#5C5E58` | Chicago         | Body text, secondary elements |
| Muted          | `#BCC5AD` | Arbor Vitae     | Borders, muted text, dividers |
| Muted Light    | `#E0D5CF` | Light Weathered Hide | Light backgrounds, cards  |
| Surface        | `#F9F7F6` | Lynx White      | Page background, inputs       |
| Card           | `#FFFFFF` | Pure White      | Card background               |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Dark           | `#050504` | Primary dark, hero sections   |
| Dark-light     | `#151514` | Dark hover state              |
| Accent         | `#CEE9BD` | Primary actions, body text    |
| Accent-lt      | `#D8F0C8` | Hover state                   |
| Body           | `#5C5E58` | Secondary elements            |
| Muted          | `#BCC5AD` | Borders, placeholders         |
| Muted Light    | `#E0D5CF` | Card backgrounds, sections    |
| Surface        | `#F9F7F6` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#6B8A5E` | Positive states     |
| Warning  | `#C49A3E` | Caution states      |
| Error    | `#B85454` | Error states        |
| Info     | `#CEE9BD` | Information (=accent) |

### Semantic Mappings

```css
--bg-primary: #F9F7F6;
--bg-secondary: #E0D5CF;
--bg-tertiary: #BCC5AD;
--bg-card: #FFFFFF;
--bg-input: #F9F7F6;

--text-primary: #050504;
--text-secondary: #5C5E58;
--text-tertiary: #BCC5AD;
--text-muted: #E0D5CF;
--text-inverse: #F9F7F6;

--accent: #CEE9BD;
--accent-hover: #D8F0C8;
--accent-muted: rgba(206,233,189,0.12);

--border: #E0D5CF;
--border-hover: #BCC5AD;
--border-focus: #CEE9BD;
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
| `--shadow-sm`      | `0 2px 8px rgba(5,5,4,0.08)`          | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(5,5,4,0.1)`          | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(5,5,4,0.14)`         | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(5,5,4,0.18)`        | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#CEE9BD`     | `#050504`     | `#CEE9BD`           |
| Secondary   | transparent   | `#050504`     | `#050504`           |
| Ghost       | transparent   | `#5C5E58`     | none                |
| Danger      | `#B85454`     | `#FFFFFF`     | `#B85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

### Input Fields

- Background: `#F9F7F6`
- Border: `1px solid #E0D5CF`
- Focus border: `#CEE9BD` + ring `0 0 0 3px rgba(206,233,189,0.15)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #E0D5CF`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(206,233,189,0.12)`    | `#5C5E58`   |
| Success   | `rgba(107,138,94,0.1)`      | `#6B8A5E`   |
| Warning   | `rgba(196,154,62,0.1)`      | `#C49A3E`   |
| Error     | `rgba(184,84,84,0.1)`       | `#B85454`   |
| Info      | `rgba(206,233,189,0.12)`    | `#5C5E58`   |

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
- `#050504` on `#F9F7F6` = **16.8:1** (AAA)
- `#5C5E58` on `#F9F7F6` = **6.5:1** (AA)
- Never use `#E0D5CF` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  --moss-dark: #050504;
  --moss-dark-light: #151514;
  --moss-accent: #CEE9BD;
  --moss-accent-light: #D8F0C8;
  --moss-body: #5C5E58;
  --moss-muted: #BCC5AD;
  --moss-muted-light: #E0D5CF;
  --moss-surface: #F9F7F6;
  --moss-card: #FFFFFF;

  --bg-primary: #F9F7F6;
  --bg-secondary: #E0D5CF;
  --bg-tertiary: #BCC5AD;
  --bg-card: #FFFFFF;
  --bg-input: #F9F7F6;

  --text-primary: #050504;
  --text-secondary: #5C5E58;
  --text-tertiary: #BCC5AD;
  --text-muted: #E0D5CF;
  --text-inverse: #F9F7F6;

  --accent: #CEE9BD;
  --accent-hover: #D8F0C8;
  --accent-muted: rgba(206,233,189,0.12);

  --border: #E0D5CF;
  --border-hover: #BCC5AD;
  --border-focus: #CEE9BD;

  --success: #6B8A5E;
  --warning: #C49A3E;
  --error: #B85454;
  --info: #CEE9BD;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(5,5,4,0.08);
  --shadow-md: 0 4px 16px rgba(5,5,4,0.1);
  --shadow-lg: 0 8px 32px rgba(5,5,4,0.14);
  --shadow-xl: 0 16px 48px rgba(5,5,4,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Moss Design System v1.0*
