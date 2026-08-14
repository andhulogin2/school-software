---
name: Academic Precision
colors:
  surface: '#f7f9fb'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#45474c'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#75777d'
  outline-variant: '#c5c6cd'
  surface-tint: '#545f73'
  primary: '#091426'
  on-primary: '#ffffff'
  primary-container: '#1e293b'
  on-primary-container: '#8590a6'
  inverse-primary: '#bcc7de'
  secondary: '#006c4a'
  on-secondary: '#ffffff'
  secondary-container: '#82f5c1'
  on-secondary-container: '#00714e'
  tertiary: '#240f00'
  on-tertiary: '#ffffff'
  tertiary-container: '#422000'
  on-tertiary-container: '#d97705'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d8e3fb'
  primary-fixed-dim: '#bcc7de'
  on-primary-fixed: '#111c2d'
  on-primary-fixed-variant: '#3c475a'
  secondary-fixed: '#85f8c4'
  secondary-fixed-dim: '#68dba9'
  on-secondary-fixed: '#002114'
  on-secondary-fixed-variant: '#005137'
  tertiary-fixed: '#ffdcc3'
  tertiary-fixed-dim: '#ffb77d'
  on-tertiary-fixed: '#2f1500'
  on-tertiary-fixed-variant: '#6e3900'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  headline-xl:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 44px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 28px
    fontWeight: '600'
    lineHeight: 36px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  data-tabular:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 16px
  lg: 24px
  xl: 32px
  grid-margin: 24px
  grid-gutter: 20px
---

## Brand & Style

This design system is built for a high-utility school management environment. The brand personality is **authoritative yet approachable**, striking a balance between corporate reliability and the warmth required in an educational setting. 

The design style follows **Modern Minimalism with Tactile Depth**. It prioritizes information density without sacrificing clarity, utilizing generous whitespace and a systematic approach to hierarchy. The emotional response should be one of "calm control"—reducing the cognitive load for administrators and educators handling complex data sets through a clean, structured interface.

## Colors

The palette is anchored by **Deep Slate (Primary)** to provide a professional, grounded foundation for navigation and headers. **Emerald Green (Secondary/Success)** is used strategically for positive data trends and primary actions, while **Soft Amber (Tertiary/Warning)** highlights pending tasks or alerts.

The background uses a cool **Off-White (Neutral)** to reduce eye strain during long periods of use. All semantic colors (Success, Warning, Error) must meet WCAG AA contrast ratios against the neutral background to ensure accessibility in data-heavy tables.

## Typography

The typography system utilizes **Inter** for its exceptional legibility and modern, neutral character. It is optimized for data density by employing a modular scale that favors clarity at smaller sizes.

A specific **Data Tabular** style is defined for use within spreadsheets and dashboards, ensuring that numbers align vertically for easy comparison. Headlines use tighter letter spacing to maintain a strong visual "lockup," while labels use increased spacing and uppercase styling to provide clear section markers without requiring excessive weight.

## Layout & Spacing

This design system employs a **Fluid Grid with Fixed Max-Width**. Content is organized on a 12-column grid for desktop, transitioning to a 4-column layout for mobile devices. 

- **Desktop (1440px+):** 24px margins, 20px gutters. Main content area capped at 1600px.
- **Tablet (768px - 1024px):** 16px margins, 16px gutters. Sidebar often collapses into an icon-only rail.
- **Mobile (<768px):** 16px margins, 12px gutters. Vertical stacking for all card-based content.

Spacing follows an 8px linear scale to ensure consistent rhythm across all components.

## Elevation & Depth

Hierarchy is established through **Tonal Layering and Ambient Shadows**. 

1.  **Level 0 (Base):** Neutral background (`#F8FAFC`).
2.  **Level 1 (Surface):** Pure white containers for cards, tables, and content blocks. These use a very soft, diffused shadow: `0px 1px 3px rgba(0,0,0,0.05), 0px 4px 6px rgba(0,0,0,0.02)`.
3.  **Level 2 (Interaction):** Hovered states or active dropdowns use a slightly more pronounced shadow to indicate "lift" from the page: `0px 10px 15px -3px rgba(0,0,0,0.08)`.

Avoid high-contrast borders; instead, use 1px strokes in a subtle light-gray (`#E2E8F0`) to define boundaries between Level 0 and Level 1.

## Shapes

The design system uses a **Rounded** shape language to soften the corporate aesthetic and make the application feel modern and accessible.

- **Standard Elements (Buttons, Inputs, Small Cards):** 0.5rem (8px) radius.
- **Large Containers (Main Dashboard Cards):** 1rem (16px) radius.
- **Interactive Indicators (Tags, Status Chips):** 1.5rem (24px) for a "pill" effect to distinguish them from functional buttons.

## Components

### Buttons
Primary buttons use the Secondary Emerald Green (`#059669`) with white text to signify action. Secondary buttons use a light slate ghost-style with a subtle border. Padding should be consistent: `10px 20px` for medium buttons.

### Inputs & Forms
Input fields must feature explicit labels using the `label-md` type style. On focus, the border should transition to Primary Slate with a 2px outer "glow" of the same color at 10% opacity.

### Data Tables
Tables are the core of this system. Use alternating row zebra-striping (Level 0 and Level 1 colors) and a sticky header. Cell padding is tight (`12px 16px`) to maximize data visibility.

### Cards
Cards are the primary container for dashboard widgets. They must include a consistent header section with a `headline-md` title and an optional "actions" area for filtering or exporting data.

### Progress Indicators
Use the Emerald Green for completion and the Primary Slate for the track background to maintain a high-contrast, professional appearance.