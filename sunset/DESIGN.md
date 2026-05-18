# Sunset Design System

> Warm glow — A vibrant orange design system for bold, energetic interfaces.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Accent         | `#F6A242` | Osage Orange    | Primary actions, links, CTAs  |
| Dark           | `#3C3D48` | Indian Ink      | Headers, nav, dark surfaces   |
| Body           | `#BAC0BE` | Maiden Mist     | Body text, secondary elements |
| Muted          | `#F1C183` | Sunset in Italy | Borders, muted text, dividers |
| Muted Light    | `#E8E8E7` | Polish White    | Light backgrounds, cards      |
| Surface        | `#FDFDFD` | Brilliance      | Page background, inputs       |
| Card           | `#FFFFFF` | Pure White      | Card background               |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Dark           | `#3C3D48` | Primary dark, hero sections   |
| Dark-light     | `#4C4D58` | Dark hover state              |
| Accent         | `#F6A242` | Primary actions, body text    |
| Accent-lt      | `#F8B058` | Hover state                   |
| Body           | `#BAC0BE` | Secondary elements            |
| Muted          | `#F1C183` | Borders, placeholders         |
| Muted Light    | `#E8E8E7` | Card backgrounds, sections    |
| Surface        | `#FDFDFD` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#6B8A5E` | Positive states     |
| Warning  | `#E2A84B` | Caution states      |
| Error    | `#B85454` | Error states        |
| Info     | `#F6A242` | Information (=accent) |

### Semantic Mappings

```css
--bg-primary: #FDFDFD;
--bg-secondary: #E8E8E7;
--bg-tertiary: #F1C183;
--bg-card: #FFFFFF;
--bg-input: #FDFDFD;

--text-primary: #3C3D48;
--text-secondary: #BAC0BE;
--text-tertiary: #F1C183;
--text-muted: #E8E8E7;
--text-inverse: #FDFDFD;

--accent: #F6A242;
--accent-hover: #F8B058;
--accent-muted: rgba(246,162,66,0.08);

--border: #E8E8E7;
--border-hover: #BAC0BE;
--border-focus: #F6A242;
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
| `--shadow-sm`      | `0 2px 8px rgba(60,61,72,0.08)`       | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(60,61,72,0.1)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(60,61,72,0.14)`      | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(60,61,72,0.18)`     | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#F6A242`     | `#FFFFFF`     | `#F6A242`           |
| Secondary   | transparent   | `#3C3D48`     | `#3C3D48`           |
| Ghost       | transparent   | `#BAC0BE`     | none                |
| Danger      | `#B85454`     | `#FFFFFF`     | `#B85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

### Input Fields

- Background: `#FDFDFD`
- Border: `1px solid #E8E8E7`
- Focus border: `#F6A242` + ring `0 0 0 3px rgba(246,162,66,0.12)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #E8E8E7`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(246,162,66,0.08)`     | `#F6A242`   |
| Success   | `rgba(107,138,94,0.1)`      | `#6B8A5E`   |
| Warning   | `rgba(226,168,75,0.1)`      | `#E2A84B`   |
| Error     | `rgba(184,84,84,0.1)`       | `#B85454`   |
| Info      | `rgba(246,162,66,0.1)`      | `#F6A242`   |

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
- `#3C3D48` on `#FDFDFD` = **12.8:1** (AAA)
- `#BAC0BE` on `#FDFDFD` = **2.8:1** (AA large text only)
- Never use `#E8E8E7` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  --sunset-dark: #3C3D48;
  --sunset-dark-light: #4C4D58;
  --sunset-accent: #F6A242;
  --sunset-accent-light: #F8B058;
  --sunset-body: #BAC0BE;
  --sunset-muted: #F1C183;
  --sunset-muted-light: #E8E8E7;
  --sunset-surface: #FDFDFD;
  --sunset-card: #FFFFFF;

  --bg-primary: #FDFDFD;
  --bg-secondary: #E8E8E7;
  --bg-tertiary: #F1C183;
  --bg-card: #FFFFFF;
  --bg-input: #FDFDFD;

  --text-primary: #3C3D48;
  --text-secondary: #BAC0BE;
  --text-tertiary: #F1C183;
  --text-muted: #E8E8E7;
  --text-inverse: #FDFDFD;

  --accent: #F6A242;
  --accent-hover: #F8B058;
  --accent-muted: rgba(246,162,66,0.08);

  --border: #E8E8E7;
  --border-hover: #BAC0BE;
  --border-focus: #F6A242;

  --success: #6B8A5E;
  --warning: #E2A84B;
  --error: #B85454;
  --info: #F6A242;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(60,61,72,0.08);
  --shadow-md: 0 4px 16px rgba(60,61,72,0.1);
  --shadow-lg: 0 8px 32px rgba(60,61,72,0.14);
  --shadow-xl: 0 16px 48px rgba(60,61,72,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Sunset Design System v1.0*
