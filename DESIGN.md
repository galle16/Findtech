---
name: Modern Fiscal Minimalism
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#45464d'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#006a61'
  on-secondary: '#ffffff'
  secondary-container: '#86f2e4'
  on-secondary-container: '#006f66'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#001a42'
  on-tertiary-container: '#3980f4'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#89f5e7'
  secondary-fixed-dim: '#6bd8cb'
  on-secondary-fixed: '#00201d'
  on-secondary-fixed-variant: '#005049'
  tertiary-fixed: '#d8e2ff'
  tertiary-fixed-dim: '#adc6ff'
  on-tertiary-fixed: '#001a42'
  on-tertiary-fixed-variant: '#004395'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  display:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.02em
  caption:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  container-max: 1280px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 40px
  stack-sm: 12px
  stack-md: 24px
  stack-lg: 48px
---

## Brand & Style

The design system is rooted in the "Modern Professional" movement, emphasizing clarity, precision, and financial empowerment. It balances the cold efficiency of traditional banking with the approachability of a modern lifestyle app.

The core aesthetic is **Minimalist with Card-based Architecture**. By utilizing generous whitespace and a restricted color palette, the interface reduces cognitive load, allowing users to focus on complex financial data without feeling overwhelmed. The atmosphere is one of calm control—conveying that the user's finances are organized, secure, and transparent. High-contrast elements are reserved specifically for data visualization and critical calls to action, ensuring the hierarchy is functional rather than decorative.

## Colors

This design system employs a "Trust-First" palette. 

- **Primary (Slate 900):** Used for headlines and core brand elements to provide a grounded, authoritative feel.
- **Secondary (Teal 600):** Represents growth and precision; used for primary actions and "Safe-to-Spend" indicators.
- **Tertiary (Blue 500):** Used for interactive elements like links and toggles to maintain a professional tech aesthetic.
- **Semantic Accents:** Income and positive trends use a vibrant Emerald green, while expenses and alerts use a soft but legible Rose red. 

Backgrounds should remain neutral (Slate 50) to allow white cards to pop with subtle depth.

## Typography

The design system relies on **Inter** for its exceptional legibility in data-dense environments. Its tall x-height and neutral character make it ideal for both large balance displays and small-print transaction details.

For numerical data, such as account numbers or transaction IDs, **JetBrains Mono** is introduced as the label font. This monospaced addition adds a layer of technical "FinTech" sophistication and ensures that columns of numbers align perfectly for easy visual scanning. Use high-weight variants (600/700) sparingly for primary headings to maintain the minimalist feel.

## Layout & Spacing

The layout follows a **Fixed-Fluid Hybrid** model. On desktop, content is contained within a 1280px maximum width, centered on the screen to prevent line-lengths from becoming unreadable. On mobile, the layout shifts to a single-column fluid stack with 16px side margins.

A strict 8px grid governs all spacing. 
- **Cards** are separated by 24px (stack-md) to provide "breathing room."
- **Internal Card Padding** should be a consistent 24px on desktop, scaling down to 16px on mobile.
- **Section Headers** use 48px (stack-lg) of top margin to clearly delineate different financial modules (e.g., separating "Accounts Overview" from "Recent Transactions").

## Elevation & Depth

The design system uses **Tonal Layers** combined with **Ambient Shadows** to create a sense of organized hierarchy.

1.  **Base (Level 0):** The background color (Slate 50).
2.  **Surface (Level 1):** Pure white (#FFFFFF) cards. These carry a very soft, diffused shadow: `0px 4px 20px rgba(15, 23, 42, 0.05)`.
3.  **Overlay (Level 2):** Modals and dropdowns. These use a more pronounced shadow to indicate focus: `0px 10px 32px rgba(15, 23, 42, 0.12)`.

Borders are used minimally. Instead of heavy outlines, a 1px stroke in Slate 200 is used only on card edges to define shape against the background if the shadow is insufficient.

## Shapes

The shape language is **Rounded**, reflecting a modern and approachable tool. 

- **Cards and Containers:** Use a 0.5rem (8px) radius to feel sturdy and structural.
- **Buttons and Inputs:** Use a 0.5rem radius to match the containers.
- **Status Tags/Chips:** Use a 1.5rem (24px) radius for a "Pill" shape, differentiating them from interactive buttons and making them feel like distinct labels.
- **Charts:** All bar charts and progress bars should feature rounded caps (4px radius) to maintain the soft aesthetic even in data visualization.

## Components

### Buttons
- **Primary:** Solid Primary color with white text. No gradient. 
- **Secondary:** Transparent background with a 1px Slate 200 border.
- **Actionable (Income):** Solid Secondary (Teal) for "Add Funds" or "Save."

### Cards
Cards are the primary container. They must always have a white background, 8px corner radius, and the Level 1 ambient shadow. Use a 24px internal padding.

### Input Fields
Inputs should be clean with a 1px Slate 200 border. On focus, the border transitions to Tertiary (Blue 500) with a 2px outer glow of the same color at 10% opacity.

### Data Visuals
- **Trend Lines:** Use a 2px stroke width. 
- **Success State:** Emerald 500.
- **Danger State:** Rose 500.
- **Empty States:** Use monochromatic Slate illustrations with subtle "Secondary" color accents to guide the user.

### Lists (Transactions)
Transaction rows should have a hover state that changes the background to Slate 50. Icons for categories (Food, Rent, etc.) should be housed in 40px circular containers with a low-opacity tint of the category's assigned color.