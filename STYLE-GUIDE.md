# Style Guide - Replace Spotify Project

**Purpose**: Visual design guidelines for ethical music streaming research documentation.

**Philosophy**: Clean, minimal, professional design that reflects leftist values through trans pride flag colors and accessible typography.

---

## Color Palette

### Trans Pride Flag Colors (Primary)

Our color scheme is derived from the transgender pride flag to center trans community solidarity and LGBTQI+ inclusive values:

**Source**: [Sexual Diversity Education - Trans Pride Flag](https://www.sexualdiversity.org/edu/flags/1086.php)

| Color | Hex Code | Usage |
|-------|----------|-------|
| **Light Blue** | `#74D7EE` | Primary links, accents, interactive elements, high ethics scores (9-10/10) |
| **Pink** | `#FFAFC8` | Hover states, secondary accents, medium ethics scores (4-6/10) |
| **White** | `#FFFFFF` | Backgrounds, callout boxes, highlights |
| **Slate** | `#5A6C7D` | Low ethics scores (1-3/10), muted states |

### Neutral Colors (Supporting)

| Color | Hex Code | Usage |
|-------|----------|-------|
| **Background** | `#fdfdfd` | Page background, card backgrounds |
| **Text Primary** | `#1a1a1a` | Headings, important text |
| **Text Body** | `#2c2c2c` | Body text, paragraphs |
| **Text Secondary** | `#666` | Subtitles, captions, metadata |
| **Text Muted** | `#999` | Footer text, less important info |
| **Border Light** | `#e8e8e8` | Primary borders, dividers |
| **Border Medium** | `#ddd` | Table headers, stronger dividers |
| **Border Subtle** | `#eee` | Table rows, list items |

### Background Tints

| Color | Hex Code | Usage |
|-------|----------|-------|
| **Blue Tint** | `#E5F7FC` | Success message backgrounds, info panels |
| **Blue Border** | `#B8EBFA` | Success message borders |
| **Pink Tint** | `#FFE9F0` | Warning/attention backgrounds, key findings |
| **Pink Border** | `#FFD6E3` | Warning message borders |
| **White** | `#FFFFFF` | Pure backgrounds, callout boxes |
| **Near White** | `#fdfdfd` | Page backgrounds, subtle variation |

---

## Typography

### Font Families

```css
font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
```

**Rationale**: System fonts for fast loading, native feel, excellent readability.

### Font Weights

- **Headings**: 300-400 (light to regular)
- **Body text**: 400 (regular)
- **Emphasis**: 500 (medium)
- **Strong emphasis**: 600 (semi-bold)
- **Never use**: 700+ (too heavy for minimal aesthetic)

### Font Sizes

| Element | Size | Weight |
|---------|------|--------|
| Page title (h1) | 2rem (32px) | 300 |
| Section heading (h2) | 1.8rem (28.8px) | 400 |
| Subsection (h3) | 1.3rem (20.8px) | 400-500 |
| Small heading (h4) | 1.1rem (17.6px) | 500-600 |
| Body text | 1rem (16px) | 400 |
| Subtitle/intro | 1.1rem (17.6px) | 400 |
| Small text | 0.9-0.95rem | 400 |
| Navigation | 0.95rem | 400 |
| Header title | 1.2rem | 400 |

### Line Height

- **Body text**: 1.6
- **Headings**: 1.2-1.4
- **Tight spacing**: 1.3-1.4 (for UI elements)

---

## Borders & Lines

### Border Rules

**CRITICAL**: All borders must be **1px only** - no exceptions.

```css
/* Correct */
border: 1px solid #e8e8e8;
border-left: 1px solid #74D7EE;
border-bottom: 1px solid #ddd;

/* WRONG - Never use thick borders */
border: 2px solid #74D7EE;  ❌
border-left: 4px solid #74D7EE;  ❌
```

### Border Styles

| Context | Border Style |
|---------|--------------|
| Cards/containers | `1px solid #e8e8e8` |
| Left accents (blue) | `1px solid #74D7EE` |
| Left accents (pink) | `1px solid #FFAFC8` |
| Table headers | `1px solid #ddd` |
| Table rows | `1px solid #eee` |
| Section dividers | `1px solid #e8e8e8` |
| Focused/hover | `1px solid #74D7EE` |

### Border Radius

**Avoid rounded corners** - use sharp edges for minimal aesthetic:

```css
/* Only acceptable uses */
border-radius: 0;  /* Preferred */
border-radius: 3-4px;  /* Maximum for small UI elements if needed */

/* WRONG */
border-radius: 8px;  ❌
```

---

## Spacing & Layout

### Padding Scale

```css
/* Small */
padding: 10px 20px;  /* Buttons, small elements */

/* Medium */
padding: 20px;  /* Cards, sections */
padding: 25px;  /* Containers, tables */

/* Large */
padding: 30px;  /* Hero sections, major containers */
```

### Margin Scale

```css
/* Element spacing */
margin-bottom: 8px;   /* List items */
margin-bottom: 15px;  /* Paragraphs, small sections */
margin-bottom: 20px;  /* Subsections */
margin-bottom: 30px;  /* Sections */
margin-bottom: 40px;  /* Major sections */

/* Page structure */
margin-top: 50px;   /* Footer separation */
```

### Container Widths

```css
max-width: 1200px;  /* Main content container */
margin: 0 auto;     /* Center alignment */
padding: 20px;      /* Side gutters */
```

---

## Components

### Sticky Header Navigation

```css
background: #fdfdfd;
border-bottom: 1px solid #e8e8e8;
padding: 1rem 2rem;
position: sticky;
top: 0;
z-index: 1000;
```

**Header Title**:
- Font size: 1.2rem
- Weight: 400
- Color: #1a1a1a

**Navigation Links**:
- Color: #74D7EE
- Hover: #FFAFC8 with underline
- Font size: 0.95rem
- Weight: 400
- Gap: 1.5rem

### Ethics Score Badges

```css
display: inline-block;
padding: 0.25rem 0.75rem;
font-weight: 500;
font-size: 0.9rem;
```

**Colors**:
- High (9-10/10): `background: #74D7EE; color: white;`
- Medium (4-6/10): `background: #FFAFC8; color: white;`
- Low (1-3/10): `background: #5A6C7D; color: white;`

### Cards

```css
background: #fdfdfd;
border: 1px solid #e8e8e8;
padding: 25px;
```

**No shadows, no rounded corners, no gradients.**

Hover states (optional):
```css
transition: border-color 0.3s;
:hover {
    border-color: #74D7EE;
}
```

### Tables

```css
width: 100%;
border-collapse: collapse;
```

**Headers**:
```css
border-bottom: 1px solid #ddd;
padding: 12px;
font-weight: 500;
text-align: left;
```

**Rows**:
```css
border-bottom: 1px solid #eee;
padding: 12px;
```

### Buttons & Links

**Primary Button**:
```css
background: #74D7EE;
color: white;
padding: 10px 20px;
border: 1px solid #74D7EE;
text-decoration: none;
font-weight: 400;
transition: background 0.3s;

:hover {
    background: #FFAFC8;
    border-color: #FFAFC8;
}
```

**Text Links**:
```css
color: #74D7EE;
text-decoration: none;
transition: color 0.3s;

:hover {
    color: #FFAFC8;
    text-decoration: underline;
}
```

### Callout Boxes

**Success/Recommendation**:
```css
background: #E5F7FC;
border: 1px solid #B8EBFA;
border-left: 1px solid #74D7EE;
padding: 20px;
```

**Warning/Attention**:
```css
background: #FFE9F0;
border: 1px solid #FFD6E3;
border-left: 1px solid #FFAFC8;
padding: 20px;
```

**Highlight/Info**:
```css
background: #FFFFFF;
border: 1px solid #e8e8e8;
border-left: 1px solid #74D7EE;
padding: 20px;
```

**Key Findings**:
```css
background: #FFE9F0;
border: 1px solid #FFD6E3;
border-left: 1px solid #FFAFC8;
padding: 20px;
```

---

## Responsive Design

### Breakpoints

```css
@media (max-width: 768px) {
    /* Mobile adjustments */
}
```

### Mobile Adjustments

- Reduce padding: 25px → 15px
- Reduce header font: 1.2rem → 1.1rem
- Reduce page title: 2rem → 1.5rem
- Stack grid columns: `grid-template-columns: 1fr;`
- Reduce navigation gap: 1.5rem → 1rem
- Reduce table font: 1rem → 0.9rem
- Reduce table padding: 12px → 8px

---

## Design Principles

### 1. Minimal Aesthetic
- Flat design (no shadows, no gradients)
- Thin borders (1px only)
- No rounded corners (or max 3-4px)
- Clean, spacious layouts
- Generous whitespace

### 2. Typography Hierarchy
- Light weights for headings (300-400)
- Never use bold headings (700+)
- Clear size differences between heading levels
- Consistent line heights

### 3. Color Usage
- Pride colors for interactive elements and status indicators
- Neutrals for backgrounds and text
- High contrast for accessibility
- Consistent color meanings across the site

### 4. Accessibility
- Sufficient color contrast (WCAG AA minimum)
- Clear focus states
- Readable font sizes (minimum 0.9rem)
- Semantic HTML structure

### 5. Political Alignment
- Trans pride flag colors center trans community solidarity and LGBTQI+ inclusivity
- Anti-corporate: minimal, anti-flashy design
- Transparency: clear information hierarchy
- Accessibility: inclusive design for all users

---

## What to Avoid

### ❌ Never Use

1. **Thick borders**: 2px, 3px, 4px, or larger
2. **Google Material colors**: #007bff, #28a745, #dc3545, #ffc107
3. **Heavy font weights**: 700, 800, 900 (bold, extra bold, black)
4. **Large rounded corners**: border-radius > 4px
5. **Drop shadows**: box-shadow (except minimal 0 1px 3px rgba(0,0,0,0.05) if needed)
6. **Gradients**: linear-gradient, radial-gradient
7. **Bright backgrounds**: High-saturation colors for large areas
8. **Animation excess**: Flashy transitions, spinning elements

### ✅ Always Do

1. **Use 1px borders** for all dividing lines
2. **Use trans pride colors** (light blue, pink, white) for interactive elements
3. **Use light font weights** (300-500 range)
4. **Maintain generous whitespace** around elements
5. **Keep layouts simple** and predictable
6. **Test on mobile** before committing
7. **Ensure color contrast** meets accessibility standards

---

## File-Specific Guidelines

### HTML Files

All HTML files should include:
- Sticky header navigation with consistent styling
- Trans pride flag color scheme throughout
- 1px borders only
- Minimal, flat design aesthetic
- Responsive meta viewport tag
- System font stack

### Markdown Files

When converting to HTML, maintain:
- Simple table styling (1px borders)
- Code blocks with dark background (#2d3748)
- Consistent heading hierarchy
- Link colors matching trans pride palette (light blue, pink)

---

## Version History

- **v1.1** (October 2025): Trans pride flag colors
  - Updated from general pride flag to trans pride flag colors
  - Light blue (#74D7EE), pink (#FFAFC8), white (#FFFFFF) as primary colors
  - Centered trans community solidarity in design philosophy
  - Updated all component examples with new color palette

- **v1.0** (October 2025): Initial style guide
  - Pride flag color palette established (later updated to trans pride)
  - 1px border rule implemented
  - Minimal flat design aesthetic defined
  - Typography guidelines set

---

## Maintenance

This style guide should be updated when:
- New components are added to the design system
- Color usage evolves
- Accessibility requirements change
- User feedback suggests improvements

Always update this guide BEFORE implementing new design patterns to maintain consistency.

---

*Style guide reflects leftist values: inclusive design, anti-corporate aesthetics, accessible presentation.*
