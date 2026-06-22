---
name: Night Bordeaux
colors:
  surface: '#191119'
  surface-dim: '#191119'
  surface-bright: '#40363f'
  surface-container-lowest: '#140b14'
  surface-container-low: '#221921'
  surface-container: '#261d25'
  surface-container-high: '#312730'
  surface-container-highest: '#3c323b'
  on-surface: '#eedeea'
  on-surface-variant: '#dbc0c4'
  inverse-surface: '#eedeea'
  inverse-on-surface: '#372d36'
  outline: '#a38b8e'
  outline-variant: '#554245'
  surface-tint: '#ffb1c0'
  primary: '#ffb1c0'
  on-primary: '#63082a'
  primary-container: '#7b1e3b'
  on-primary-container: '#ff8ca6'
  inverse-primary: '#a03b57'
  secondary: '#efbe7b'
  on-secondary: '#452b00'
  secondary-container: '#614006'
  on-secondary-container: '#dcad6b'
  tertiary: '#cec5b9'
  on-tertiary: '#353027'
  tertiary-container: '#474138'
  on-tertiary-container: '#b6ada1'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffd9df'
  primary-fixed-dim: '#ffb1c0'
  on-primary-fixed: '#3f0017'
  on-primary-fixed-variant: '#81233f'
  secondary-fixed: '#ffddb2'
  secondary-fixed-dim: '#efbe7b'
  on-secondary-fixed: '#291800'
  on-secondary-fixed-variant: '#614006'
  tertiary-fixed: '#ebe1d4'
  tertiary-fixed-dim: '#cec5b9'
  on-tertiary-fixed: '#1f1b13'
  on-tertiary-fixed-variant: '#4c463d'
  background: '#191119'
  on-background: '#eedeea'
  surface-variant: '#3c323b'
typography:
  display-lg:
    fontFamily: Playfair Display
    fontSize: 64px
    fontWeight: '700'
    lineHeight: 72px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-sm:
    fontFamily: Playfair Display
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Manrope
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
    letterSpacing: 0.05em
  button:
    fontFamily: Manrope
    fontSize: 15px
    fontWeight: '600'
    lineHeight: 20px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1200px
  gutter: 24px
  margin-mobile: 20px
  margin-desktop: 64px
  section-gap: 120px
---

## Brand & Style
The design system is engineered for a high-end personal portfolio, evoking a sense of "After-Hours Luxury." The personality is sophisticated, exclusive, and commanding, yet retains an inviting warmth through its tonal palette. 

The aesthetic is rooted in **Modern Glassmorphism** and **Minimalism**. It utilizes deep, dark backgrounds to create a boundless canvas where content feels illuminated from within. The emotional response should be one of prestige and professional excellence, achieved through high-contrast accents and expansive whitespace that suggests confidence and room to breathe.

## Colors
The palette is centered on a "Deep Night" foundation. 
- **Primary Background:** Used for the main canvas to provide depth.
- **Secondary Background:** Used for section differentiation and surface grouping.
- **Accent (Rich Bordeaux):** Reserved for primary brand elements and emotive highlights.
- **Secondary Accent (Luxury Gold):** Used for interactive cues, icons, and premium details.
- **Highlight (Warm Ivory):** Specifically for moments of high contrast against the dark base.
- **Action Gradient:** A diagonal transition from Bordeaux to Gold, used exclusively for primary calls to action to create a "shimmer" effect.

## Typography
The typographic hierarchy relies on the tension between the editorial elegance of **Playfair Display** and the technical precision of **Manrope**. 

- **Headlines:** Use Playfair Display with tight letter spacing for a high-fashion, "masthead" feel. Headlines should primarily use the Warm Ivory or White color tokens.
- **Body:** Manrope provides superior legibility at smaller sizes. Use the Secondary Text color (#D8D8D8) for long-form reading to reduce eye strain.
- **Labels:** Always set in Manrope with increased letter spacing and uppercase styling to denote metadata or category tags.

## Layout & Spacing
The layout follows a **Fixed Grid** philosophy on desktop (12 columns) and a fluid model on mobile (4 columns). 

- **Generous Gaps:** Maintain a minimum 120px vertical gap between major sections to preserve the luxury feel.
- **Content Alignment:** Center-aligned layouts are preferred for landing sections; left-aligned for data-heavy or portfolio-detail sections.
- **Safe Zones:** High-end portfolios require significant "negative space." Avoid crowding the edges of glass containers.

## Elevation & Depth
Depth is achieved through **Glassmorphism** rather than traditional drop shadows.
- **Surface 1 (Base):** Deep Night Bordeaux (#120A12).
- **Surface 2 (Glass):** Secondary Background (#1D0F18) at 60% opacity with a 20px backdrop-blur. 
- **Border Treatment:** Glass elements should have a 1px solid stroke at 10% opacity (Warm Ivory) to catch the "light" at the edges.
- **Ambient Glow:** Instead of black shadows, use low-opacity Bordeaux (#7B1E3B) glows (0px 20px 40px) behind primary floating cards to create a sense of luminescence.

## Shapes
This design system utilizes a **Rounded** shape language to soften the high-contrast color palette.
- **Standard Radius:** 0.5rem (8px) for input fields and small cards.
- **Container Radius (Large):** 1.5rem (24px) for portfolio item cards and glass sections.
- **Interactive Radius:** Buttons should use a 100px pill shape to distinguish them from structural elements.

## Components
- **Buttons:** 
  - *Primary:* Gradient background (Bordeaux to Gold), White text, pill-shaped. On hover, apply a subtle scale (1.02x) and increase glow intensity.
  - *Secondary:* 1px Luxury Gold border, transparent background, Gold text.
- **Portfolio Cards:** Glassmorphic background with 24px padding. Image within the card should have a 12px border radius.
- **Chips/Tags:** Small pill-shaped containers with a 10% Bordeaux fill and a solid Bordeaux 1px border. Text in Manrope Label-MD style.
- **Input Fields:** Bottom-border only or fully enclosed glass containers. Focus state should trigger a Luxury Gold border transition.
- **Navigation:** Fixed top bar with a heavy backdrop-blur (30px) and a subtle 1px bottom border in Warm Ivory (5% opacity).
- **Smooth Transitions:** All interactive states must use a `cubic-bezier(0.4, 0, 0.2, 1)` timing function for a "weighty," premium feel.