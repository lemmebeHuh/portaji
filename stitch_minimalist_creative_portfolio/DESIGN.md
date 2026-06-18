---
name: Obsidian & Parchment
colors:
  surface: '#fbf9f8'
  surface-dim: '#dbdad9'
  surface-bright: '#fbf9f8'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f5f3f3'
  surface-container: '#efeded'
  surface-container-high: '#eae8e7'
  surface-container-highest: '#e4e2e2'
  on-surface: '#1b1c1c'
  on-surface-variant: '#444748'
  inverse-surface: '#303030'
  inverse-on-surface: '#f2f0f0'
  outline: '#747878'
  outline-variant: '#c4c7c7'
  surface-tint: '#5f5e5e'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#1c1b1b'
  on-primary-container: '#858383'
  inverse-primary: '#c8c6c5'
  secondary: '#13677b'
  on-secondary: '#ffffff'
  secondary-container: '#a1e7ff'
  on-secondary-container: '#18697e'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#1a1c1c'
  on-tertiary-container: '#838484'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e5e2e1'
  primary-fixed-dim: '#c8c6c5'
  on-primary-fixed: '#1c1b1b'
  on-primary-fixed-variant: '#474746'
  secondary-fixed: '#b2ebff'
  secondary-fixed-dim: '#8bd1e8'
  on-secondary-fixed: '#001f27'
  on-secondary-fixed-variant: '#004e5f'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c7'
  on-tertiary-fixed: '#1a1c1c'
  on-tertiary-fixed-variant: '#454747'
  background: '#fbf9f8'
  on-background: '#1b1c1c'
  surface-variant: '#e4e2e2'
  parchment-bg: '#F9F9F9'
  ink-text: '#1A1A1A'
  deep-teal: '#005F73'
  canvas-gray: '#EEEEEE'
typography:
  display-lg:
    fontFamily: Playfair Display
    fontSize: 72px
    fontWeight: '700'
    lineHeight: 84px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Playfair Display
    fontSize: 48px
    fontWeight: '600'
    lineHeight: 56px
  headline-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-md:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '500'
    lineHeight: 42px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 32px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 28px
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.1em
  label-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
spacing:
  unit: 8px
  margin-mobile: 24px
  margin-desktop: 80px
  gutter: 32px
  section-gap: 160px
---

## Brand & Style

This design system is built for the elite creative professional, embodying a "Sophisticated Minimalist" aesthetic. It draws heavily from the **Minimalism** movement, prioritizing negative space as a functional element rather than a void. The emotional response is one of calm authority, intellectual rigor, and quiet luxury. 

The visual language follows an "Ink & Paper" philosophy: high-contrast legibility paired with tactile-inspired surfaces. The goal is to create a museum-gallery atmosphere where the UI recedes, allowing the creative work (photography, case studies, art) to command full attention. Interactions should be buttery and understated, avoiding aggressive animations in favor of subtle opacity shifts and smooth layout transitions.

## Colors

The palette is strictly curated to evoke the sensation of high-end editorial print. 

- **Primary (Ink):** Used for headlines, iconography, and high-impact borders. It provides the grounding weight of the design.
- **Secondary (Teal):** Used sparingly as a "focus" color for active states, text links, or subtle highlights. It adds a modern, digital edge to an otherwise classic palette.
- **Background (Parchment):** An off-white `#F9F9F9` is the primary canvas, reducing eye strain and feeling more premium than pure white.
- **Neutral (Slate):** Used for secondary metadata, body text, and decorative rules to maintain a hierarchy that doesn't compete with the primary headlines.

## Typography

The typographic system relies on the tension between the classic, high-contrast serifs of **Playfair Display** and the utilitarian precision of **Inter**.

- **Headlines:** Use Playfair Display for all major headings. Large display sizes should utilize tighter letter-spacing to feel more like a bespoke masthead.
- **Body:** Use Inter for all long-form reading. A generous line height (1.6x to 1.8x) is mandatory to maintain the "airy" feel of the brand.
- **Labels:** Small caps with increased tracking (0.1em) should be used for categories, eyebrows, and navigational links to provide a structured, architectural contrast to the fluid serif headlines.

## Layout & Spacing

The layout follows a **Fixed Grid** philosophy for desktop to maintain editorial control over line lengths and image compositions.

- **Desktop:** A 12-column grid with a maximum container width of 1440px. Gutters are wide (32px) to prevent visual clutter.
- **Whitespace:** Use "The Rule of Oversized Margins." Section gaps should be aggressive (160px+) to force the user to focus on one piece of content at a time.
- **Mobile:** Transition to a 4-column fluid grid. Margins remain generous (24px) to frame the content like a mobile magazine.
- **Alignment:** Mix centered headlines for introductory sections with asymmetrical, left-aligned body text for a modern, rhythmic feel.

## Elevation & Depth

This system avoids traditional shadows to maintain a flat, print-like aesthetic. Depth is achieved through **Tonal Layers** and scale:

- **Surface Tiers:** Use the #EEEEEE (Canvas Gray) for subtle background containers or image cards to separate them from the Parchment background without using borders.
- **Z-Index Strategy:** Only the navigation bar uses a backdrop blur (Glassmorphism) when scrolling, allowing content to pass underneath it with a soft 10px blur and 80% opacity.
- **Active States:** Instead of elevation, use "Ghost Outlines" (1px solid #1A1A1A) or slight scale-up transitions (1.02x) for interactive elements.

## Shapes

The design system utilizes **Sharp (0px)** corners across all primary components. This choice reinforces the "architectural" and "editorial" nature of the brand.

- **Imagery:** Portfolio images and thumbnails must always have 0px radius.
- **Buttons:** Rectangular containers with sharp corners create a sense of precision and formality.
- **Exceptions:** Form inputs may use a hairline 1px bottom border only, rather than a full box, to maintain the minimalist aesthetic.

## Components

### Buttons
- **Primary:** Solid #1A1A1A background with #F9F9F9 text. No rounded corners. Large padding (16px 40px).
- **Secondary (Ghost):** 1px border of #1A1A1A. Hover state fills the background with #1A1A1A.
- **Label:** All labels in buttons must use `label-caps`.

### Cards & Image Placeholders
- **Portfolio Card:** Full-bleed image with a sharp 0px crop. Typography appears below the image in `label-caps` (category) and `headline-md` (project title).
- **Hover Interaction:** Images should have a subtle grayscale-to-color transition or a slight zoom-in effect (1.05x) within their container.

### Navigation
- **Desktop:** A top-aligned, persistent bar with a transparent background that turns into a blurred Parchment surface on scroll.
- **Links:** Use `label-caps` with a 1px bottom border that appears on hover/active states.

### Input Fields
- Underline-only style. 1px solid #555555. On focus, the border transitions to #1A1A1A with a 0.3s ease. 
- Placeholder text should be in `body-md` using the Neutral color.

### Lists
- Minimalist bullet points (small squares or dashes) using the Primary color.
- Generous vertical padding between list items (16px) to maintain the "airy" rhythm.