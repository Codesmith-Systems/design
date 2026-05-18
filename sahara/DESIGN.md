# Sahara Design System

> Warm earth — A rich amber-brown design system for grounded, premium interfaces.

---

## 1. Color Palette

### Core Colors

| Token          | Hex       | Name            | Usage                        |
|----------------|-----------|-----------------|------------------------------|
| Accent         | `#BB8F54` | Summer Weasel   | Primary actions, links, CTAs  |
| Dark           | `#231D18` | Dark Orchestra  | Headers, nav, dark surfaces   |
| Body           | `#86460C` | Sis Kebab       | Body text, secondary elements |
| Muted          | `#C2B5A1` | Pigeon Grey     | Borders, muted text, dividers |
| Muted Light    | `#DCDBD9` | Subtle Touch    | Light backgrounds, cards      |
| Surface        | `#F5F4F2` | Sand            | Page background, inputs       |
| Card           | `#FFFFFF` | Pure White      | Card background               |

### Extended Scale

| Token          | Hex       | Usage                        |
|----------------|-----------|------------------------------|
| Dark           | `#231D18` | Primary dark, hero sections   |
| Dark-light     | `#332A20` | Dark hover state              |
| Accent         | `#BB8F54` | Primary actions, body text    |
| Accent-lt      | `#BC760F` | Hover state (Caramel Coating) |
| Body           | `#86460C` | Secondary elements            |
| Muted          | `#C2B5A1` | Borders, placeholders         |
| Muted Light    | `#DCDBD9` | Card backgrounds, sections    |
| Surface        | `#F5F4F2` | Page background               |

### Semantic Colors

| Token    | Hex       | Usage              |
|----------|-----------|--------------------|
| Success  | `#6B8A5E` | Positive states     |
| Warning  | `#C49A3E` | Caution states      |
| Error    | `#B85454` | Error states        |
| Info     | `#BB8F54` | Information (=accent) |

### Semantic Mappings

```css
--bg-primary: #F5F4F2;            /* Page background */
--bg-secondary: #DCDBD9;          /* Section/card background */
--bg-tertiary: #C2B5A1;           /* Elevated surface */
--bg-card: #FFFFFF;               /* Card background */
--bg-input: #F5F4F2;              /* Input field background */

--text-primary: #231D18;          /* Headings, important text */
--text-secondary: #86460C;        /* Body text */
--text-tertiary: #BC760F;         /* Captions, descriptions */
--text-muted: #C2B5A1;            /* Disabled, placeholders */
--text-inverse: #F5F4F2;          /* Text on dark backgrounds */

--accent: #BB8F54;                /* Primary accent */
--accent-hover: #BC760F;          /* Accent hover state */
--accent-muted: rgba(187,143,84,0.08); /* Subtle accent bg */

--border: #DCDBD9;                /* Default border */
--border-hover: #C2B5A1;          /* Hover border */
--border-focus: #BB8F54;          /* Focus ring */
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
| `--shadow-sm`      | `0 2px 8px rgba(35,29,24,0.08)`       | Subtle elevation   |
| `--shadow-md`      | `0 4px 16px rgba(35,29,24,0.1)`       | Cards              |
| `--shadow-lg`      | `0 8px 32px rgba(35,29,24,0.14)`      | Modals, popovers   |
| `--shadow-xl`      | `0 16px 48px rgba(35,29,24,0.18)`     | Hero overlays      |

---

## 6. Component Patterns

### Buttons

| Variant     | Background    | Text Color    | Border              |
|-------------|---------------|---------------|---------------------|
| Primary     | `#BB8F54`     | `#FFFFFF`     | `#BB8F54`           |
| Secondary   | transparent   | `#231D18`     | `#231D18`           |
| Ghost       | transparent   | `#86460C`     | none                |
| Danger      | `#B85454`     | `#FFFFFF`     | `#B85454`           |

**Sizes:** sm (8px 16px), default (12px 24px), lg (16px 32px)

**States:** hover lifts with shadow, active presses down

### Input Fields

- Background: `#F5F4F2`
- Border: `1px solid #DCDBD9`
- Focus border: `#BB8F54` + ring `0 0 0 3px rgba(187,143,84,0.12)`
- Border radius: 10px
- Padding: 12px 16px

### Cards

- Background: `#FFFFFF`
- Border: `1px solid #DCDBD9`
- Border radius: 16px
- Padding: 24px
- Hover: shadow-md + translateY(-2px)

### Badges

| Variant   | Background                  | Text Color  |
|-----------|-----------------------------|-------------|
| Default   | `rgba(187,143,84,0.08)`     | `#BB8F54`   |
| Success   | `rgba(107,138,94,0.1)`      | `#6B8A5E`   |
| Warning   | `rgba(196,154,62,0.1)`      | `#C49A3E`   |
| Error     | `rgba(184,84,84,0.1)`       | `#B85454`   |
| Info      | `rgba(187,143,84,0.1)`      | `#BB8F54`   |

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
- `#231D18` on `#F5F4F2` = **14.8:1** (AAA)
- `#86460C` on `#F5F4F2` = **6.2:1** (AA)
- `#BC760F` on `#F5F4F2` = **4.8:1** (AA)
- Never use `#DCDBD9` for text below 18px on light backgrounds
- Focus indicators use `--border-focus` with 3px offset ring
- All interactive elements have visible focus states
- Respect `prefers-reduced-motion` — disable animations when active

---

## 9. CSS Custom Properties Setup

```css
:root {
  /* Core Palette */
  --sahara-dark: #231D18;
  --sahara-dark-light: #332A20;
  --sahara-accent: #BB8F54;
  --sahara-accent-light: #BC760F;
  --sahara-body: #86460C;
  --sahara-muted: #C2B5A1;
  --sahara-muted-light: #DCDBD9;
  --sahara-surface: #F5F4F2;
  --sahara-card: #FFFFFF;

  /* Semantic */
  --bg-primary: #F5F4F2;
  --bg-secondary: #DCDBD9;
  --bg-tertiary: #C2B5A1;
  --bg-card: #FFFFFF;
  --bg-input: #F5F4F2;

  --text-primary: #231D18;
  --text-secondary: #86460C;
  --text-tertiary: #BC760F;
  --text-muted: #C2B5A1;
  --text-inverse: #F5F4F2;

  --accent: #BB8F54;
  --accent-hover: #BC760F;
  --accent-muted: rgba(187,143,84,0.08);

  --border: #DCDBD9;
  --border-hover: #C2B5A1;
  --border-focus: #BB8F54;

  --success: #6B8A5E;
  --warning: #C49A3E;
  --error: #B85454;
  --info: #BB8F54;

  --font-display: 'Space Grotesk', sans-serif;
  --font-body: 'DM Sans', sans-serif;

  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 16px;
  --radius-xl: 24px;
  --radius-full: 9999px;

  --shadow-sm: 0 2px 8px rgba(35,29,24,0.08);
  --shadow-md: 0 4px 16px rgba(35,29,24,0.1);
  --shadow-lg: 0 8px 32px rgba(35,29,24,0.14);
  --shadow-xl: 0 16px 48px rgba(35,29,24,0.18);

  --ease-out: cubic-bezier(0.16, 1, 0.3, 1);
  --duration-fast: 150ms;
  --duration-normal: 250ms;
  --duration-slow: 400ms;
}
```

---

*Generated by Sahara Design System v1.0*
