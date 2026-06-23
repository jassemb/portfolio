---
name: Cyber-Terminal Matrix
colors:
  surface: '#051424'
  surface-dim: '#051424'
  surface-bright: '#2c3a4c'
  surface-container-lowest: '#010f1f'
  surface-container-low: '#0e1c2d'
  surface-container: '#122131'
  surface-container-high: '#1d2b3c'
  surface-container-highest: '#283647'
  on-surface: '#d5e4fa'
  on-surface-variant: '#bac9cc'
  inverse-surface: '#d5e4fa'
  inverse-on-surface: '#233143'
  outline: '#849396'
  outline-variant: '#3b494c'
  surface-tint: '#00daf3'
  primary: '#c3f5ff'
  on-primary: '#00363d'
  primary-container: '#00e5ff'
  on-primary-container: '#00626e'
  inverse-primary: '#006875'
  secondary: '#b9c8dd'
  on-secondary: '#233142'
  secondary-container: '#39485a'
  on-secondary-container: '#a7b6cb'
  tertiary: '#e8ecf8'
  on-tertiary: '#2c3139'
  tertiary-container: '#ccd0db'
  on-tertiary-container: '#545962'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#9cf0ff'
  primary-fixed-dim: '#00daf3'
  on-primary-fixed: '#001f24'
  on-primary-fixed-variant: '#004f58'
  secondary-fixed: '#d4e4fa'
  secondary-fixed-dim: '#b9c8dd'
  on-secondary-fixed: '#0d1d2c'
  on-secondary-fixed-variant: '#39485a'
  tertiary-fixed: '#dee2ee'
  tertiary-fixed-dim: '#c2c6d1'
  on-tertiary-fixed: '#171c24'
  on-tertiary-fixed-variant: '#424750'
  background: '#051424'
  on-background: '#d5e4fa'
  surface-variant: '#283647'
  surface-glass: rgba(18, 33, 49, 0.7)
  scanline-cyan: rgba(0, 229, 255, 0.2)
  grid-line: rgba(30, 41, 59, 0.1)
  terminal-black: '#000000'
  critical-red: '#93000a'
typography:
  display-lg:
    fontFamily: JetBrains Mono
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: JetBrains Mono
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: JetBrains Mono
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  code-sm:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  stack-sm: 8px
  gutter: 24px
  stack-md: 24px
  stack-lg: 48px
  container-max: 1200px
  margin-mobile: 16px
---

## Brand & Style
The brand personality is **highly technical, secure, and futuristic**, drawing heavily from **Cyberpunk and DevSecOps aesthetics**. It evokes the feeling of a high-security terminal or an "Operations Center" dashboard. 

The design style is a hybrid of **Glassmorphism** and **Technical Minimalism**. It utilizes deep dark backgrounds, vibrant cyan accents for "data-driven" focus, and subtle grid overlays. The interface prioritizes information density and structural integrity, using monospaced typography to reinforce a coder-centric, professional identity. The emotional response should be one of "controlled power" and "absolute security."

## Colors
The palette is dominated by a deep "Midnight Blue" (`#051424`) background, providing a high-contrast base for the "Electric Cyan" (`#00e5ff`) primary action color. 

- **Primary:** Cyan is used exclusively for interactive elements, status indicators, and critical technical labels.
- **Secondary:** Dark muted blues are used for container backgrounds and glass panels to provide depth without breaking the dark mode immersion.
- **Surface Detail:** A subtle grid pattern and animated scanlines provide a "CRT" or "Heads-Up Display" (HUD) texture.
- **Accents:** Tertiary greys and secondary fixed colors are reserved for metadata and less critical logs.

## Typography
The system uses a **Dual-Font strategy** to balance technical precision with readability.

- **JetBrains Mono** is the core brand font, used for all headlines, buttons, and "log-style" data points. It should be used in uppercase for labels to enhance the "system" feel.
- **Inter** is used for long-form body copy to ensure legibility and a modern, professional touch.

**Scaling:** Large displays use tight tracking and heavy weights. On mobile, headlines scale down significantly to fit the viewport, while body text remains consistent for accessibility.

## Layout & Spacing
The layout follows a **Fixed-Grid philosophy** for desktop, centering content within a 1200px container, while transitioning to a **Fluid model** on mobile with 16px side margins.

- **Vertical Rhythm:** Content is organized into distinct sections separated by `stack-lg` (48px). Internal card spacing relies on `stack-md` (24px).
- **Alignment:** A strong vertical axis is created by left-aligned titles and a custom "Timeline" vertical rule for experience logs.
- **Sectioning:** Heavy use of vertical spacing and semantic icons ensures that technical data is parsable.

## Elevation & Depth
Depth is achieved through **Glassmorphism and Tonal Layering** rather than traditional drop shadows.

- **Glass Panels:** Primary containers use a semi-transparent background (`rgba(18, 33, 49, 0.7)`) with a 12px backdrop blur.
- **Outlines:** Instead of shadows, surfaces are defined by `1px` borders using `outline-variant` colors at low opacity.
- **Glow Effects:** High-importance elements (like active timeline nodes or primary buttons) use a "Cyan Glow" (`box-shadow: 0 0 15px rgba(0, 229, 255, 0.15)`) to simulate light emission from a screen.
- **Layers:** Background (Grid) -> Glass Panels (Content) -> Floating Nav (Top/Bottom bars).

## Shapes
The shape language is **angular and structural**. 

- **Base Radius:** A default "Soft" radius of `0.125rem` (2px) is used for small elements like tags and status badges.
- **Container Radius:** Standard cards and glass panels use `0.25rem` (lg) or `0.5rem` (xl) to slightly soften the technical aesthetic without becoming "bubbly."
- **Interactive Elements:** Buttons and interactive cards maintain sharp, precise corners to reinforce the "terminal" metaphor.

## Components

- **Buttons:**
  - *Primary:* Filled with Cyan (`primary-container`), text in dark navy.
  - *Outline:* Border in Cyan, text in Cyan, no fill.
  - *Terminal:* Rectangular, monospace text, hover effect involves a slight scale reduction (`scale-95`).
- **Cards (Glass):** Feature a top-to-bottom scanline animation and a subtle border. Used for hero sections and project summaries.
- **Timeline:** A vertical line (`outline-variant`) with glowing circular nodes. Active nodes use the `glow-cyan` effect.
- **Tech Chips:** Small, rectangular badges with `0.2em` letter spacing, a low-opacity cyan background, and a 1px border.
- **Terminal Detail:** A specific component for code blocks or status logs featuring a black background, Mac-style window controls (red/yellow/green dots), and animated cursors.
- **Navigation:**
  - *Desktop:* Fixed top bar with a heavy blur and bottom border.
  - *Mobile:* Fixed bottom tab bar using large icons and `label-caps` for quick thumb access.