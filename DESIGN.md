---
name: Midnight Metallic RTL
colors:
  surface: '#0b1326'
  surface-dim: '#0b1326'
  surface-bright: '#31394d'
  surface-container-lowest: '#060d20'
  surface-container-low: '#131b2e'
  surface-container: '#171f33'
  surface-container-high: '#222a3e'
  surface-container-highest: '#2d3449'
  on-surface: '#dbe2fd'
  on-surface-variant: '#cac4d0'
  inverse-surface: '#dbe2fd'
  inverse-on-surface: '#283044'
  outline: '#948f9a'
  outline-variant: '#49454f'
  surface-tint: '#d0bcff'
  primary: '#e9ddff'
  on-primary: '#37265e'
  primary-container: '#d0bcff'
  on-primary-container: '#594983'
  inverse-primary: '#665590'
  secondary: '#4cd7f6'
  on-secondary: '#003640'
  secondary-container: '#03b5d4'
  on-secondary-container: '#00424e'
  tertiary: '#d8e3fb'
  on-tertiary: '#263143'
  tertiary-container: '#bcc7de'
  on-tertiary-container: '#485366'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e9ddff'
  primary-fixed-dim: '#d0bcff'
  on-primary-fixed: '#210f48'
  on-primary-fixed-variant: '#4d3d76'
  secondary-fixed: '#acedff'
  secondary-fixed-dim: '#4cd7f6'
  on-secondary-fixed: '#001f26'
  on-secondary-fixed-variant: '#004e5c'
  tertiary-fixed: '#d8e3fa'
  tertiary-fixed-dim: '#bcc7de'
  on-tertiary-fixed: '#111c2d'
  on-tertiary-fixed-variant: '#3c475a'
  background: '#0b1326'
  on-background: '#dbe2fd'
  surface-variant: '#2d3449'
  electric-violet: '#d0bcff'
  cyan-glow: '#4cd7f6'
  outline-metallic: '#958ea0'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 64px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: 0px
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: 0px
  headline-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Manrope
    fontSize: 13px
    fontWeight: '600'
    lineHeight: '1.2'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 4px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 48px
  container-max: 1280px
---

## Brand & Style
The design system is a high-end, automotive-inspired interface tailored for the luxury brokerage market, now optimized for **Hebrew (RTL)** environments. The brand personality remains prestigious, precise, and cinematic, targeting high-net-worth individuals who appreciate the intersection of engineering and elegance.

The design style is **Modern Glassmorphism** with a **Dark Metallic** foundation. It mimics the light-reflective surfaces of luxury vehicles through layered transparency, backdrop blurs, and "Neon Underglow" accents. The RTL adaptation ensures that the visual flow respects the reading direction of the Hebrew script, maintaining the "cockpit" feel while ensuring logical hierarchy and technical authority.

## Colors
The palette is rooted in a "Midnight Metallic" theme, using deep navy and slate tones to provide a structural skeleton that allows vibrant accents to pop.

- **Primary (Electric Violet):** Used for primary calls to action, focus states, and key navigational highlights.
- **Secondary (Cyan Glow):** Used for technical data, success indicators, and secondary highlights.
- **Metallic Neutrals:** Layered shades of deep navy (Level 0 to Level 2) create depth.
- **RTL Considerations:** Gradients and light-source effects (rim lighting) are mirrored. Linear gradients for buttons and headers should flow from right-to-left (Electric Violet on the right, Cyan Glow on the left).

## Typography
Typography is tuned for Hebrew legibility while maintaining the assertive, executive feel of the original design. 

- **Hebrew Support:** **Hanken Grotesk** is retained for headlines due to its modern, open forms that translate well to Hebrew characters. Tracking (letter spacing) is neutralized for Hebrew scripts to avoid breaking character connections.
- **Hierarchy:** Headlines are bold and impactful. **Manrope** is used for body text to ensure a balanced, readable experience for vehicle specs and reports. 
- **Technical Data:** **JetBrains Mono** is utilized for VINs and performance metrics. Note that while the UI is RTL, numeric technical data (e.g., 0-100 km/h, VIN numbers) should remain LTR as per international automotive standards.

## Layout & Spacing
The layout uses a **Fluid Grid** model with a 12-column desktop and 4-column mobile structure. All layouts are strictly **Right-to-Left (RTL)**.

- **Directionality:** Page flow starts from the top-right. Sidebars, navigation icons, and back buttons are mirrored to the right side.
- **Rhythm:** An 8px/4px hybrid scale ensures precision in technical layouts. 
- **Gaps & Margins:** Padding and margins use logical properties (`padding-inline-start` instead of `padding-left`) to ensure seamless switching between locales. 
- **Negative Space:** Maintains a "Luxury Gallery" feel—avoiding clutter to let vehicle photography dominate the visual field.

## Elevation & Depth
Depth is achieved through **Tonal Layers** and **Glassmorphism**. Shadows are replaced by light-based indicators.

- **Glass Surfaces:** Containers use a semi-transparent white tint (15%) with a 40px backdrop blur. 
- **Rim Lighting:** Higher-level modals feature a 1px border on the top and *right* sides (mirrored for RTL) to simulate a light source coming from the upper right.
- **Neon Underglow:** Active elements use a soft outer glow (10px-20px blur) of Electric Violet instead of traditional drop shadows, mimicking the under-chassis lighting of a performance car.

## Shapes
The system utilizes **Rounded** (0.5rem) geometry to bridge the gap between technical precision and premium comfort.

- **Action Elements:** Buttons and tags use `rounded-lg`. High-priority "Contact Broker" triggers use pill-shapes (`rounded-full`) for immediate visual distinction.
- **Data Inputs:** Use a smaller `rounded-sm` (0.25rem) radius to reinforce a sense of "engineered" accuracy.

## Components
- **Buttons:** Feature a horizontal gradient. In RTL, the gradient starts with Electric Violet on the right. Icon placement in buttons is mirrored (icon leads on the right, text follows on the left).
- **Inventory Cards:** 16:9 aspect ratio imagery with a glassmorphic overlay at the bottom. Data points within the overlay flow right-to-left.
- **Status Chips:** Indicators for "Available" or "Sold" use a soft inner glow. In RTL, the status icon (if present) is placed to the right of the text.
- **Input Fields:** Dark surfaces with slate borders. On focus, the border transitions to a violet gradient. Floating labels move to the top-right of the field.
- **Car Specs List:** Zebra-striped rows using transparency. Technical units (e.g., HP, km/h) remain LTR for clarity, while their labels are RTL.
- **Verified Badge:** A silver metallic badge with a 3D effect, typically anchored to the top-left of a card in RTL layouts (the "end" position).