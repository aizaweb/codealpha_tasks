---
name: Aurelian Precision
colors:
  surface: '#121414'
  surface-dim: '#121414'
  surface-bright: '#38393a'
  surface-container-lowest: '#0c0f0f'
  surface-container-low: '#1a1c1c'
  surface-container: '#1e2020'
  surface-container-high: '#282a2b'
  surface-container-highest: '#333535'
  on-surface: '#e2e2e2'
  on-surface-variant: '#d1c4be'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#2f3131'
  outline: '#9a8e89'
  outline-variant: '#4e4540'
  surface-tint: '#d5c3ba'
  primary: '#d5c3ba'
  on-primary: '#392e28'
  primary-container: '#1b120d'
  on-primary-container: '#8b7b74'
  inverse-primary: '#695c55'
  secondary: '#e9c349'
  on-secondary: '#3c2f00'
  secondary-container: '#af8d11'
  on-secondary-container: '#342800'
  tertiary: '#e4c469'
  on-tertiary: '#3d2f00'
  tertiary-container: '#c7a851'
  on-tertiary-container: '#4f3d00'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#f2dfd6'
  primary-fixed-dim: '#d5c3ba'
  on-primary-fixed: '#231914'
  on-primary-fixed-variant: '#51443e'
  secondary-fixed: '#ffe088'
  secondary-fixed-dim: '#e9c349'
  on-secondary-fixed: '#241a00'
  on-secondary-fixed-variant: '#574500'
  tertiary-fixed: '#ffe08d'
  tertiary-fixed-dim: '#e4c368'
  on-tertiary-fixed: '#241a00'
  on-tertiary-fixed-variant: '#584400'
  background: '#121414'
  on-background: '#e2e2e2'
  surface-variant: '#333535'
typography:
  display-main:
    fontFamily: Geist
    fontSize: 64px
    fontWeight: '300'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-main-mobile:
    fontFamily: Geist
    fontSize: 48px
    fontWeight: '300'
    lineHeight: '1.1'
  headline-lg:
    fontFamily: Manrope
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.05em
  button-label:
    fontFamily: Space Grotesk
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 24px
    letterSpacing: 0.02em
  sub-label:
    fontFamily: Space Grotesk
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
    letterSpacing: 0.1em
  body-md:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  keypad-gap: 12px
  display-margin: 32px
  container-padding: 24px
  button-height: 64px
---

## Brand & Style

This design system translates the heritage of haute horlogerie and high-end automotive interiors into a digital interface for scientific computation. The personality is authoritative, precise, and unapologetically luxurious, targeting professionals who view their tools as an extension of their personal craft.

The visual style is a fusion of **Glassmorphism** and **Tactile Minimalism**. It utilizes deep, multi-layered depth to simulate "physicality under glass." Surfaces appear as polished obsidian or smoked sapphire, framed by precision-machined metallic accents. The emotional response is one of calm confidence—where every interaction feels weighted, intentional, and high-performance.

## Colors

The palette is anchored in a monochromatic range of deep browns and blacks to simulate high-end materials like Makassar ebony and carbon fiber. 

- **Primary Background**: A subtle vertical gradient from Deep Espresso (#241813) to Rich Dark Chocolate (#1B120D), providing a cavernous sense of depth.
- **Metallic Gold (#D4AF37)**: Used for primary functional triggers, active state glows, and hairline borders. It represents the "internal movement" of the calculator.
- **Champagne Gold (#E6C56A)**: A brighter, more reflective tint used for specular highlights and secondary interactive feedback.
- **Soft White (#F8F8F8)**: Employed for all data-rich text to ensure maximum legibility against the dark void of the background.

## Typography

Typography is treated as a mechanical engraving. **Manrope** provides a balanced, modern structure for headings and titles, while **Geist** is used for its technical precision in the main calculation display and body text. **Space Grotesk** is reserved for labels and function keys to provide a subtle futuristic, geometric edge.

- **The Main Display**: Use `display-main` with a slight outer glow to simulate a high-end OLED panel.
- **Function Keys**: Labels should be centered, utilizing `button-label`.
- **Secondary Actions**: Use `sub-label` with increased letter-spacing for a sophisticated, "stamped" look.

## Layout & Spacing

The layout follows a **Fixed Grid** model inspired by precision instrumentation. The interface is divided into two primary zones: the **Aperture** (Display) and the **Manifold** (Keypad).

- **Aperture**: Takes up the top 30% of the screen. Content is right-aligned with generous internal padding to create an "infinity pool" effect.
- **Manifold**: A rigid 12-column grid for desktop or a 4-column grid for mobile. Elements are separated by consistent `keypad-gap` units to allow the background glows to seep through.
- **Margins**: A safety margin of `display-margin` is maintained around the entire interface to ensure the product feels "framed" like a piece of jewelry.

## Elevation & Depth

Hierarchy is established through transparency and metallic light-play rather than traditional shadows.

- **Base Layer**: The dark espresso gradient.
- **Glass Layer**: Semi-transparent overlays with a 20px backdrop-blur. Use a 1px inner stroke of Champagne Gold at 20% opacity to define the edge of the "glass."
- **Active State (Glow)**: When a key is pressed, it emits an ambient golden glow (`#D4AF37`) with a 40px blur radius, appearing as if a light is being switched on behind a sapphire crystal.
- **Reflections**: Apply a diagonal linear gradient (White at 5% to Transparent) across the top half of the entire interface to simulate the reflection of studio lighting on a polished surface.

## Shapes

The shape language is "Squircle-based"—avoiding the harshness of perfect squares but maintaining the structure of professional hardware.

- **Main Buttons**: Use `rounded-lg` (16px) to create a soft, pebble-like feel that is comfortable for frequent interaction.
- **The Display (Aperture)**: Uses a tighter `rounded-sm` (4px) or even sharp edges to differentiate the digital read-out from the physical keys.
- **Container**: The outer housing of the design system should use `rounded-xl` to mimic the chamfered edges of luxury hardware.

## Components

### Precision Buttons
The primary interaction element. Buttons feature a "sunburst" metallic texture (subtle radial gradient) and a 1px border. On hover, the border brightens. On press, the button "sinks" slightly (scale: 0.98) and triggers a golden ripple effect.

### The Glass Aperture
The main display area. It should feature a slight "fresnel" effect at the edges where the background appears darker and more distorted, emphasizing the thickness of the virtual glass.

### Function Chips
Used for scientific constants. These are smaller, pill-shaped elements with a high-contrast Gold border and no fill, ensuring they don't distract from the primary number pad.

### Input Fields
When entering variables, the text field should glow with a subtle Gold pulse, indicating the system is "waiting" for precision data.

### Sliders (for Precision Adjustment)
Inspired by watch crowns. A horizontal track with a metallic thumb that features knurling (fine vertical lines) and haptic-style snapping during movement.