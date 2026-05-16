---
name: InfoLove Digital Gift
colors:
  surface: '#fff8f5'
  surface-dim: '#e3d8d0'
  surface-bright: '#fff8f5'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#fdf1e9'
  surface-container: '#f8ece4'
  surface-container-high: '#f2e6de'
  surface-container-highest: '#ece0d9'
  on-surface: '#201b16'
  on-surface-variant: '#5b403c'
  inverse-surface: '#352f2a'
  inverse-on-surface: '#fbefe7'
  outline: '#906f6b'
  outline-variant: '#e4beb8'
  surface-tint: '#ba1b16'
  primary: '#b61714'
  on-primary: '#ffffff'
  primary-container: '#da342a'
  on-primary-container: '#fffbff'
  inverse-primary: '#ffb4a9'
  secondary: '#b22b19'
  on-secondary: '#ffffff'
  secondary-container: '#ff624a'
  on-secondary-container: '#630500'
  tertiary: '#5c4fa7'
  on-tertiary: '#ffffff'
  tertiary-container: '#7568c1'
  on-tertiary-container: '#fffbff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdad5'
  primary-fixed-dim: '#ffb4a9'
  on-primary-fixed: '#410001'
  on-primary-fixed-variant: '#930005'
  secondary-fixed: '#ffdad4'
  secondary-fixed-dim: '#ffb4a7'
  on-secondary-fixed: '#400200'
  on-secondary-fixed-variant: '#8f1003'
  tertiary-fixed: '#e5deff'
  tertiary-fixed-dim: '#c8bfff'
  on-tertiary-fixed: '#1a0064'
  on-tertiary-fixed-variant: '#463990'
  background: '#fff8f5'
  on-background: '#201b16'
  surface-variant: '#ece0d9'
typography:
  hero-lg:
    fontFamily: Playfair Display
    fontSize: 96px
    fontWeight: '600'
    lineHeight: 92px
    letterSpacing: -0.03em
  hero-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 48px
    fontWeight: '600'
    lineHeight: 52px
    letterSpacing: -0.02em
  headline-section:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '500'
    lineHeight: 38px
    letterSpacing: -0.01em
  stat-value:
    fontFamily: Playfair Display
    fontSize: 72px
    fontWeight: '500'
    lineHeight: 76px
    letterSpacing: -0.03em
  quote-italic:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '400'
    lineHeight: '1.3'
  body-base:
    fontFamily: Nunito Sans
    fontSize: 15px
    fontWeight: '400'
    lineHeight: 24px
    letterSpacing: 0.01em
  label-caps:
    fontFamily: Nunito Sans
    fontSize: 11px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.18em
rounded:
  sm: 0.5rem
  DEFAULT: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  full: 9999px
spacing:
  xs: 0.5rem
  sm: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  xxl: 5rem
  container-max: 1200px
---

## Brand & Style

The design system is centered on a "Digital Gift" philosophy, transforming raw data into an intimate, high-fidelity narrative. The brand personality is human, affectionate, and deeply personal, evoking the nostalgia of a physical scrapbook or a premium editorial magazine. 

The aesthetic blends **Editorial Minimalism** with **Tactile Glassmorphism**. It utilizes soft 3D illustrations—specifically the "envelope and heart" characters—to provide a sense of playfulness and physical depth. To enhance the tactile quality, a subtle paper grain overlay should be applied globally to all surfaces, ensuring the UI feels like organic cotton cardstock rather than a digital screen.

Emotional response goals:
- **Nostalgia:** Through serif typography and warm, muted tones.
- **Warmth:** Through candlelight-inspired lighting effects and soft radial glows.
- **Intimacy:** Through generous whitespace and focused, data-driven storytelling.

## Colors

This color palette is a warm, romantic spectrum that pairs intense reds with an unexpected, dreamy lavender to create a modern editorial feel.

- **Primary (Vibrant Passion):** A bright, energetic red used for core brand signifiers, main CTAs, and emotional peaks.
- **Secondary (Deep Garnet):** A rich, dark red for high-emphasis typography and editorial headers, providing grounded contrast.
- **Tertiary (Dreamy Lavender):** A soft purple used for secondary accents, special highlights, and "magical" data moments.
- **Neutral (Antique Parchment):** The foundational page background, setting a warm, antique tone.

The interface should feel "lit from within," using low-opacity radial gradients in the corners of the viewport to mimic a soft, candlelit glow.

## Typography

The typography system relies on a high-contrast pairing: an expressive, organic serif for emotion and a soft, friendly sans-serif for technical data.

- **Headlines:** Use **Playfair Display** for all major headings. The ampersand (&) should be treated as a decorative element—stylized in a lighter weight, italicized, and colored in the primary red.
- **Body & Data:** Use **Nunito Sans** for all functional text. Its rounded terminals complement the soft shape language of the brand.
- **Tracking:** Headings use tight tracking (-0.03em) to feel poetic and compact. Small labels use high tracking (0.18em) to maintain an editorial, structured finish.
- **Quotes:** Always rendered in a large, italicized serif to emphasize the "human" voice behind the data.

## Layout & Spacing

The layout philosophy follows an **Editorial Grid** model with a focus on generous whitespace ("Muito Respiro").

- **Grid Model:** A 12-column fixed grid for desktop (max-width 1200px), collapsing to a single-column flow on mobile.
- **Rhythm:** Sections should be separated by a minimum of 80px (xxl) on desktop to ensure the narrative feels digestible. 
- **Structural Dividers:** Use thin, 1px horizontal rules in a low-opacity Deep Garnet (`rgba(137, 9, 0, 0.15)`) to demarcate sections without cluttering the visual field.
- **Margins:** Heavy page padding (64px+) keeps the central story focused and mimics the margins of a printed book.

## Elevation & Depth

Hierarchy is established through **Tonal Layering** and **Soft Ambient Shadows**. 

Instead of traditional material shadows, this system uses "glow-shadows"—diffused, low-opacity dropshadows tinted with the primary red or deep garnet colors to maintain the warm atmosphere. 

- **Level 1 (Surface):** The background (Antique Parchment) is the base.
- **Level 2 (Containers):** Cards use the Vibrant Cream color. They appear to rest "on" the paper with a subtle 1px hairline border.
- **Level 3 (Interactive/Floating):** 3D assets and primary buttons use "Candlelight Shadows" (blur: 24px, opacity: 0.1, color: #890900) to create a soft, physical lift.
- **Depth Breaks:** 3D characters should occasionally "break" the container bounds (overflowing cards) to add a playful, tactile dimension.

## Shapes

The shape language is ultra-soft and organic, emphasizing a friendly and approachable "pill-shaped" aesthetic.

- **Cards:** Use large, consistent corner radii (rounded-lg/xl) to reinforce the friendly, "gift" feel.
- **Interactive Elements:** Buttons and tags use a full pill-shape (rounded-full) to maximize tactile appeal.
- **Heatmap/Data Cells:** Use a generous radius (rounded-md) to maintain a grid-like structure while softening the overall look.
- **Hairlines:** All decorative lines should be extremely thin (1px) to mimic high-end stationery printing.

## Components

### Buttons
- **Primary:** Fully rounded pill-shaped. Background: Vibrant Passion Red; Text: Antique Parchment (Label-caps style).
- **Secondary:** Transparent background with a 1px border in Deep Garnet. Italicized serif text labels.

### Cards & Containers
- **Data Card:** Vibrant Cream surface with a 1px Deep Garnet hairline border. Content should be padded generously (32px).
- **Featured Stat Card:** Deep Garnet background with Antique Parchment text for maximum emotional impact.

### Input Fields
- Soft, warm parchment background with a 1px border. On focus, the border transitions to Vibrant Passion Red with a soft, tinted outer glow.

### Specialized Data Components
- **Heart Heatmap:** A 7x24 grid. Inactive cells use Antique Parchment; active cells scale to Vibrant Passion Red. Peak values are outlined with a 1.5px Dreamy Lavender border.
- **Emoji Podium:** A 3-column vertical podium. The center (1st place) card is elevated with a Y-axis offset and styled in the "Featured" card theme.
- **VS Blocks:** Symmetrical cards separated by a decorative floating heart icon or a serif "vs".

### Navigation
- Avoid standard sticky bars. Use "Corner Deco" indicators in the top corners of the page frame with small, italicized serif labels (e.g., "— a story —") to reinforce the ledger feel.