# Robot Forest Design System

This document describes the visual design system used in the Robot Forest theme.

## Color Palette

### Background Colors
```css
--color-bg: #0a0e1a           /* Primary background - very dark blue-black */
--color-bg-secondary: #111827  /* Secondary background - dark blue-gray */
--color-bg-elevated: #1a1f35   /* Elevated surfaces - lighter dark blue */
--color-surface: #1f2937       /* Surface elements - medium dark gray */
```

### Text Colors
```css
--color-text: #e5e7eb          /* Primary text - light gray */
--color-text-secondary: #9ca3af /* Secondary text - medium gray */
--color-text-muted: #6b7280     /* Muted text - darker gray */
```

### Accent Colors
```css
--color-accent: #60a5fa         /* Primary accent - bright blue */
--color-accent-hover: #3b82f6   /* Hover state - deeper blue */
--color-accent-secondary: #8b5cf6 /* Secondary accent - purple */
```

### Utility Colors
```css
--color-border: #374151         /* Borders and dividers */
--color-code-bg: #1e293b        /* Code block background */
```

## Typography

### Font Families
```css
--font-sans: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif
--font-mono: 'JetBrains Mono', 'Courier New', monospace
```

### Type Scale
- **h1**: 2.5rem (40px) - Article titles, hero title
- **h2**: 2rem (32px) - Section headings
- **h3**: 1.5rem (24px) - Subsection headings
- **h4**: 1.25rem (20px) - Minor headings
- **h5**: 1.125rem (18px)
- **h6**: 1rem (16px)
- **Body**: 1rem (16px) - Base text size
- **Small**: 0.875rem (14px) - Meta information

### Font Weights
- **Light**: 300 - Rarely used
- **Regular**: 400 - Body text
- **Medium**: 500 - Nav links, emphasis
- **Semibold**: 600 - Headings
- **Bold**: 700 - Hero title, strong emphasis

### Line Heights
- **Headings**: 1.3 - Tight for impact
- **Body**: 1.6 - Standard readability
- **Article content**: 1.8 - Enhanced readability

## Spacing System

```css
--spacing-xs: 0.5rem   /* 8px - Minimal spacing */
--spacing-sm: 1rem     /* 16px - Small spacing */
--spacing-md: 2rem     /* 32px - Medium spacing */
--spacing-lg: 3rem     /* 48px - Large spacing */
--spacing-xl: 4rem     /* 64px - Extra large spacing */
```

## Layout

### Containers
```css
--max-width: 1200px        /* Standard content width */
--max-width-narrow: 800px  /* Narrow content (articles) */
```

### Border Radius
```css
--border-radius: 8px       /* Standard radius */
--border-radius-lg: 12px   /* Large radius for cards */
```

### Transitions
```css
--transition: 0.2s ease-in-out  /* Standard transition */
```

## Component Patterns

### Cards
- Background: `--color-bg-secondary`
- Border: 1px solid `--color-border`
- Border radius: `--border-radius-lg`
- Padding: `--spacing-md`
- Hover: Translate up 4px, add shadow, accent border

### Buttons
- **Primary**: Gradient from accent to accent-secondary
- **Secondary**: Surface background with border
- Padding: 0.75rem 2rem
- Border radius: `--border-radius`
- Font weight: 600
- Hover: Translate up 2px, add shadow

### Links
- Default: `--color-accent`
- Hover: `--color-accent-hover`
- Transition: color 0.2s
- Nav links include underline animation on hover

### Forms
- Input background: `--color-bg`
- Border: 1px solid `--color-border`
- Focus: Border color changes to `--color-accent`
- Border radius: `--border-radius`
- Padding: 0.75rem 1rem

## Visual Effects

### Gradients
```css
/* Hero background */
background: linear-gradient(135deg, 
    var(--color-bg-secondary) 0%, 
    var(--color-bg-elevated) 100%
);

/* Button background */
background: linear-gradient(135deg, 
    var(--color-accent) 0%, 
    var(--color-accent-secondary) 100%
);

/* Hero title text */
background: linear-gradient(135deg, 
    var(--color-text) 0%, 
    var(--color-accent) 100%
);
```

### Shadows
```css
/* Card hover */
box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);

/* Button hover */
box-shadow: 0 10px 20px rgba(96, 165, 250, 0.3);
```

### Backdrop Effects
```css
/* Header background */
backdrop-filter: blur(10px);
background-color: rgba(17, 24, 39, 0.95);
```

## Iconography

### Social Icons
- Size: 20x20px
- Stroke width: 2px
- Style: Outline (not filled)
- Color: `--color-text-secondary`
- Hover: `--color-accent`

### Icons Used
- GitHub (Octocat)
- LinkedIn (Professional network)
- Twitter (Bird)
- Email (Envelope)
- RSS (Feed)
- YouTube (Play button)

## Responsive Breakpoints

```css
/* Mobile */
@media (max-width: 480px) {
    /* Stack layouts, reduce spacing */
}

/* Tablet */
@media (max-width: 768px) {
    /* Adjust grid, show mobile menu */
}

/* Desktop */
@media (min-width: 769px) {
    /* Full layout, horizontal menu */
}
```

### Mobile Adaptations
- Reduced spacing (xl: 3rem, lg: 2rem)
- Single column post grid
- Hamburger navigation menu
- Stacked newsletter form
- Smaller type scale

## Animation Principles

### Timing
- Fast interactions: 0.2s (hover, focus)
- Transitions: 0.2s ease-in-out
- Longer animations: 0.3s (image scale)

### Transforms
- Translate up on hover: -2px to -4px
- Scale on image hover: 1.05
- Rotation: Used sparingly (hamburger menu)

### Easing
- `ease-in-out`: Most transitions
- Linear: Used for opacity changes only

## Accessibility

### Contrast Ratios
- Body text on background: > 7:1 (AAA)
- Secondary text on background: > 4.5:1 (AA)
- Links maintain sufficient contrast

### Focus States
- All interactive elements have visible focus states
- Focus uses accent color for consistency
- Keyboard navigation fully supported

### Semantic HTML
- Proper heading hierarchy
- ARIA labels on icon-only buttons
- Semantic sectioning elements
- Alt text requirements for images

## Design Philosophy

### Principles
1. **Content First**: Typography and readability are paramount
2. **Subtle Motion**: Animations enhance, don't distract
3. **Consistent Spacing**: Use the spacing scale religiously
4. **Purposeful Color**: Accent colors guide attention
5. **Mobile Responsive**: Mobile is not an afterthought
6. **Performance**: Minimize JavaScript, optimize CSS

### Visual Hierarchy
1. **Hero title**: Largest, gradient effect
2. **Section titles**: Large, high contrast
3. **Post titles**: Medium, accent on hover
4. **Body text**: Readable, comfortable line height
5. **Meta information**: Smaller, muted color

### Whitespace
- Generous spacing between sections
- Comfortable reading width for articles
- Breathing room around interactive elements
- Clear visual separation between content areas

## Implementation Notes

### CSS Organization
1. CSS Variables (design tokens)
2. Reset & base styles
3. Typography
4. Layout utilities
5. Components (ordered by complexity)
6. Responsive overrides

### Browser Support
- Modern browsers (last 2 versions)
- CSS Grid and Flexbox
- CSS Custom Properties
- No IE11 support required

### Performance
- Single CSS file (~10KB gzipped)
- Minimal JavaScript (~2KB)
- System fonts as fallback
- Optimized animations (transform/opacity only)

---

This design system ensures consistency across the Robot Forest theme and makes customization predictable and maintainable.

