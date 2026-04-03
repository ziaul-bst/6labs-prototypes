# Apparatus Design System — Style Guide
> Figma source: https://www.figma.com/design/Nt21OzTRlJKgvSLMoSxTyT/Apparatus
> Last modified: 2026-03-23 | Author: Ziaul Islam

---

## 1. Brand & Identity

The design system is named **Apparatus** and underpins the **6Labs** product family. The branding section contains:
- **Logo Mark** — icon-only mark (component set)
- **Full Logo** — wordmark + mark combination (component set)

The logo has two placement contexts:
- `Image/Blur Logo Dark Bg` — logo treatment for dark backgrounds
- `Image / Blur Logo Light Bg` — logo treatment for light backgrounds

---

## 2. Color Palette

### 2.1 Primitive Colors

#### Base Scale

| Token | Hex | Usage |
|---|---|---|
| `Base/Base-950` | `#080D1A` | Dark mode page background (deepest) |
| `Base/Base-925` | `#111827` | Dark mode card/surface background |
| `Base/Base-910` | `#1A2236` | Dark mode elevated surface (modals, popovers) |
| `Base/Base - 900` | `#030D2D` | Primary text (headings), dark backgrounds |
| `Base/Base - 800` | `#1C2542` | Very dark navy, secondary dark text |
| `Base/Base - 700` | `#353D57` | Dark navy-grey, body text on dark bg |
| `Base/Base - 600` | `#4F566C` | Mid-dark grey, secondary text |
| `Base/Base - 500` | `#686E81` | Mid grey, disabled text, dividers |
| `Base/Base - 400` | `#818696` | Medium grey, secondary icons, light borders |
| `Base/Base - 300` | `#9A9EAB` | Light grey, inactive elements |
| `Base/Base - 200` | `#B3B6C0` | Pale grey, hover backgrounds |
| `Base/Base - 100` | `#CDCFD5` | Card borders, dividers (default border color) |
| `Base/Base - 50` | `#E6E7EA` | Tag/chip bg, subtle fills |

#### Neutral

| Token | Hex | Usage |
|---|---|---|
| `Neutral/White` | `#FFFFFF` | Pure white |
| `Neutral/Black` | `#000000` | Pure black |
| `Neutral/Surface` | `#F1F1F1` | Default card/panel background (light mode) |
| `Neutral/Surface-Pale` | `#F5F5F5` | Page backgrounds, section dividers |

#### Brand Blue

| Token | Hex | Usage |
|---|---|---|
| `Brand Blue/600` | `#0D5ED4` | Primary button pressed/active |
| `Brand Blue/500` | `#1770EF` | Core brand — CTAs, links, active states |
| `Brand Blue/400` | `#4D8FF5` | Hover state, dark mode primary |
| `Brand Blue/Tint Dark` | `#1770EF66` | 40% opacity — dark bg selected state |
| `Brand Blue/Tint` | `#1770EF24` | 14% opacity — selected bg, focus rings |
| `Brand Blue/Tint Light` | `#1770EF12` | 7% opacity — light hover tint |

#### Complementary

| Token | Hex | Usage |
|---|---|---|
| `Complimentary/Pink/500` | `#C20568` | Hot-pink secondary accent CTAs |
| `Complimentary/Pink/400` | `#E31776` | Lighter pink — complementary hover |
| `Complimentary/Purple/500` | `#7B4CFF` | Accent purple — AI features, premium |
| `Complimentary/Purple/400` | `#9873FF` | Purple hover |

#### Status Colors

| Token | Hex | Usage |
|---|---|---|
| `Status/Error` | `#C9392A` | Error — WCAG AA 4.5:1 on white |
| `Status/Error Dark` | `#A52E20` | Destructive button pressed |
| `Status/Error Light` | `#DE5A48` | Error hover on dark bg |
| `Status/Warning` | `#FFB700` | Warning amber |
| `Status/Success` | `#16A34A` | Success green |
| `Status/Notice` | `#67C3BB` | Teal — informational messages |

### 2.2 Semantic Colors (Light / Dark)

The **Semantic** collection provides Light and Dark mode aliases for all contextual uses. Always use these tokens over primitives for component fills, text, and borders.

#### Backgrounds

| Token | Light | Dark |
|---|---|---|
| `Background/Elements` | `#FFFFFF` | `#080D1A` |
| `Background/Card` | `#FFFFFF` | `#111827` |
| `Background/Page BG` | `#F1F1F1` | `#1A2236` |
| `Background/Page BG 2` | `#F5F5F5` | `#1A2236` |
| `Background/Subtle` | `#E6E7EA` | `#1C2542` |
| `Background/Highlighted` | `#1770EF` | `#1770EF` |
| `Background/Highlighted Tint` | `#1770EF24` | `#1770EF24` |
| `Background/Highlighted Tint Light` | `#1770EF12` | `#1770EF12` |
| `Background/Highlighted Tint Dark` | `#1770EF66` | `#1770EF66` |

#### Text & Icon

| Token | Light | Dark |
|---|---|---|
| `Text & Icon/Primary` | `#030D2D` | `#FFFFFF` |
| `Text & Icon/Secondary` | `#4F566C` | `#9A9EAB` |
| `Text & Icon/Tertiary` | `#818696` | `#686E81` |
| `Text & Icon/Placeholder` | `#9A9EAB` | `#686E81` |
| `Text & Icon/Disabled` | `#9A9EAB` | `#4F566C` |
| `Text & Icon/OnBrand` | `#FFFFFF` | `#FFFFFF` |
| `Text & Icon/OnDark` | `#FFFFFF` | `#FFFFFF` |
| `Text & Icon/Brand` | `#1770EF` | `#1770EF` |

#### Borders

| Token | Light | Dark |
|---|---|---|
| `Border/Default` | `#CDCFD5` | `rgba(255,255,255,0.12)` |
| `Border/Hover` | `#9A9EAB` | `rgba(255,255,255,0.25)` |
| `Border/Focus` | `#1770EF` | `#4D8FF5` |
| `Border/Error` | `#C9392A` | `#C9392A` |
| `Border/Subtle` | `#E6E7EA` | `rgba(255,255,255,0.12)` |
| `Border/Tint` | `#1770EF24` | `#1770EF24` |
| `Border/Brand Hover` | `#4D8FF5` | `#4D8FF5` |

#### Interactive

| Token | Light | Dark |
|---|---|---|
| `Interactive/Brand` | `#1770EF` | `#1770EF` |
| `Interactive/BrandHover` | `#4D8FF5` | `#4D8FF5` |
| `Interactive/BrandPressed` | `#0D5ED4` | `#0D5ED4` |

### 2.3 Gradient Styles

| Style Name | Type | Usage |
|---|---|---|
| `Gradient/Blue` | Linear | Primary blue gradient fill |
| `Gradient/Blue Hover` | Linear | Blue gradient hover state |
| `Gradient/Glass` | Linear | Glassmorphism surface fill |
| `Gradient/Linear Dark 1` | Linear | Dark background gradient |
| `Gradient/Radial Dark 1` | Radial | Dark radial background accent |

### 2.4 Translucent Values Reference

**Black (Dark overlays):** Black-4 (0.04), Black-8 (0.08), Black-10 (0.10), Black-16 (0.16), Black-20 (0.20), Black-30 (0.30), Black-40 (0.40), Black-50 (0.50), Black-60 (0.60), Black-70 (0.70), Black-80 (0.80), Black-90 (0.90)

**White (Light overlays/glassmorphism):** White-10 (0.10), White-12 (0.12), White-20 (0.20), White-25 (0.25), White-30 (0.30), White-40 (0.40), White-50 (0.50), White-60 (0.60), White-70 (0.70), White-80 (0.80), White-90 (0.90)

---

## 3. Typography

### 3.1 Font Families

| Font | Variable | Usage |
|---|---|---|
| **Bricolage Grotesque** | `DisplayFont` | All Title styles, Button Labels, Labels |
| **Inter** | `BodyFont` | All Body and Paragraph styles |
| **Roboto Mono** | (no variable token) | Code blocks only |

### 3.2 Font Size Tokens (Default / Compact modes)

| Token | Default | Compact |
|---|---|---|
| `size/2xs` | 10px | 10px |
| `size/xs` | 12px | 11px |
| `size/s` | 14px | 13px |
| `size/m` | 16px | 14px |
| `size/l` | 20px | 18px |
| `size/xl` | 24px | 20px |
| `size/2xl` | 32px | 28px |
| `size/3xl` | 36px | 32px |
| `size/4xl` | 48px | 40px |
| `size/5xl` | 64px | 56px |

### 3.3 Text Style Hierarchy

Naming convention: `Category/Size/Weight`

#### Title Styles — Font: Bricolage Grotesque

| Style Name | px | Font Style | Line Height | Text Case |
|---|---|---|---|---|
| `Title/5XL` | 64px | Bold | 110% | Normal |
| `Title/4XL/ExtraBold` | 48px | ExtraBold | 120% | Normal |
| `Title/4XL/Semibold` | 48px | Bold | 120% | Normal |
| `Title/3XL/ExtraBold` | 36px | ExtraBold | 150% | Normal |
| `Title/3XL/Medium` | 36px | Bold | 150% | Normal |
| `Title/3XL/Regular` | 36px | Regular | 150% | Normal |
| `Title/2XL/ExtraBold` | 32px | ExtraBold | 150% | Normal |
| `Title/2XL/Medium` | 32px | Bold | 150% | Normal |
| `Title/2XL/Regular` | 32px | Regular | 150% | Normal |
| `Title/XL/Medium` | 24px | Bold | 150% | Normal |
| `Title/XL/Regular` | 24px | Regular | 150% | Normal |
| `Title/XL/CAPS` | 24px | Bold | 130% | UPPER |
| `Title/L/Medium` | 20px | Bold | 150% | Normal |
| `Title/L/Regular` | 20px | Regular | 150% | Normal |
| `Title/L/Caps` | 20px | Bold | 130% | UPPER |
| `Title/M/Bold` | 16px | Bold | 150% | Normal |
| `Title/M/Semibold` | 16px | SemiBold | 150% | Normal |
| `Title/S/Bold` | 14px | Bold | 150% | Normal |
| `Title/S/Semibold` | 14px | SemiBold | 150% | Normal |
| `Title/XS/Bold` | 12px | Bold | 150% | Normal |
| `Title/XS/Semibold` | 12px | SemiBold | 150% | Normal |

> **Weight note:** "ExtraBold" style name = `96pt ExtraBold` font style. "Medium" = Bold weight. The naming reflects visual hierarchy, not literal font weight names.

#### Body / Paragraph Styles — Font: Inter

| Style Name | px | Font Style | Line Height | Notes |
|---|---|---|---|---|
| `Body/L/Regular` | 16px | Regular | 150% | Default body |
| `Body/L/Medium` | 16px | Medium | 150% | Emphasized body |
| `Body/L/Semibold` | 16px | Semi Bold | 150% | Strong body |
| `Body/M/Regular` | 14px | Regular | 150% | Secondary body |
| `Body/M/Medium` | 14px | Medium | 150% | Emphasized secondary |
| `Body/M/Semibold` | 14px | Semi Bold | 150% | Strong secondary |
| `Body/M/Underlined` | 14px | Regular | 150% | Links, underlined text |
| `Body/S/Regular` | 12px | Regular | 150% | Captions, metadata |
| `Body/S/Medium` | 12px | Medium | 150% | Emphasized captions |
| `Body/S/Underlined` | 12px | Regular | 150% | Small underlined links |
| `Body/S/Graph Legend` | 12px | Regular | 100% | Chart/graph labels — tight LH |
| `Body/XS/Regular` | 10px | Regular | auto | Helper text, fine print |
| `Body/XS/Medium` | 10px | Semi Bold | 16px fixed | Fine print emphasized; 2% letter-spacing |

#### Button Label Styles — Font: Bricolage Grotesque

| Style Name | px | Font Style | Line Height |
|---|---|---|---|
| `Button Label/XLarge` | 16px | SemiBold | 24px |
| `Button Label/Large` | 14px | SemiBold | 20px |
| `Button Label/Medium` | 12px | SemiBold | 18px |
| `Button Label/Small` | 10px | SemiBold | 16px |

#### Label Styles — Font: Bricolage Grotesque, ALL CAPS

| Style Name | px | Font Style | Letter Spacing | Line Height |
|---|---|---|---|---|
| `Label/Medium` | 10px | Bold | 15% | auto |
| `Label/Regular` | 10px | Regular | 14% | auto |

> Labels are always rendered in **ALL CAPS** (`textCase: UPPER`).

#### Code Styles — Font: Roboto Mono

| Style Name | px | Font Style | Line Height |
|---|---|---|---|
| `Code/Regular` | 12px | Regular | 150% |
| `Code/Small` | 11px | Regular | 150% |

---

## 4. Effects & Shadows

### 4.1 Shadow Styles (Drop Shadows)

| Style Name | Offset Y | Blur | Spread | Color | Usage |
|---|---|---|---|---|---|
| `Shadow/Small` | 2px | 8px | 0 | `rgba(0,0,0,0.04)` | Subtle card lift, tooltip shadows |
| `Shadow/Normal` | 4px | 16px | 0 | `rgba(0,0,0,0.08)` | Standard card/panel elevation |
| `Shadow/Big` | 8px | 24px | 0 | `rgba(0,0,0,0.08)` | Modals, drawers, prominent overlays |
| `Shadow/Button Shadow` | 8px | 16px | 0 | `rgba(0,0,0,0.10)` | Dedicated button drop shadow |
| `Shadow / Dark` | 4px | 8px | 0 | `rgba(0,0,0,0.30)` | Dark-mode / high-contrast shadows |

### 4.2 Border Styles (Inner Shadows — 1px directional)

All borders use color `rgba(0,0,0,0.16)` except `Border/Top`.

| Style Name | Direction | Offset | Color |
|---|---|---|---|
| `Border/Top` | Top edge | `x:0 y:1` | `rgba(245,245,245,1.0)` — light fill |
| `Border/Bottom` | Bottom edge | `x:0 y:-1` | `rgba(0,0,0,0.16)` |
| `Border/Left` | Left edge | `x:1 y:0` | `rgba(0,0,0,0.16)` |
| `Border/Right` | Right edge | `x:-1 y:0` | `rgba(0,0,0,0.16)` |

### 4.3 Blur Styles

| Style Name | Type | Blur Amount |
|---|---|---|
| `Blur/Bg Blur - Small` | Background blur | 24px |
| `Blur/Bg Blur - Medium` | Background blur | 64px |
| `Blur/Bg Blur - Large` | Background blur | 120px |
| `Blur/Layer Blur - 120` | Layer blur | 120px |

---

## 5. Layout & Grid

| Style Name | Description |
|---|---|
| `12 Col - Desktop` | Standard 12-column desktop grid |
| `Cover Safe Area` | Safe area constraints for cover/thumbnail frames |

---

## 6. Iconography

### 6.1 Icon Sizes

| Size | Frame Name | Use Case |
|---|---|---|
| 16px | `16 px` | Inline text icons, compact UI |
| 24px | `24 px` | Standard UI icons (default) |
| 32px | `32 px` | Medium emphasis icons |
| 40px | `40 px` | Large touch targets |
| 48px | `48 px` | Feature icons |
| 128px | `128 px` | Illustrative / hero icons |
| Additional | `Additional` | Special-case icons outside standard sizes |

### 6.2 Icon Style

- Icons are built as Figma **Components** — instantiable and swappable
- Icons within 24px include subcategories: standard, outlined, filled, and color variants
- The 16px set includes: `Video Ad`, `Radio`, `Restart`, `Like`, `Timer`, `Clock`, `Tags`
- Icon source library references MingCute icons (e.g. `mingcute:search-ai-line` visible in canvas)
- Typical fill: `transparent` background with colored vector path

### 6.3 Icon Library Structure (24px rows)

The 24px frame contains multiple rows organized by:
1. Standard icons row
2. Outlined/monochrome row
3. Filled/colored row
4. App-specific icons row

---

## 7. Components

### 7.1 Buttons

Located in: `Components → Buttons → 💠 Buttons`

#### Core Button Component

| Component | Node ID | Description |
|---|---|---|
| `Button` | `12943:1310` | Primary button component set with all variants |
| `Button Attributes` | `12945:1352` | Button property/state variants |
| `Tooltips` | `12454:3025` | Tooltip popovers attached to buttons |

**Button color variants:**
- White button
- Black button
- Accent / Blue (`#1770EF`) button
- Accent 6Labs button
- White-80 (translucent)
- Black-80 (translucent)
- Complementary Pink (`#C20568`)
- Complementary Purple (`#7B4CFF`)

**Button properties:**
- Size variants: Small, Medium, Large, XLarge
- State: Default, Hover, Pressed, Disabled, Loading
- With/without leading icon
- With/without trailing icon
- Shape: Standard (rounded) or Pill

**Button border radius by size** (from Semantic/button/* tokens):
- Small → `4px`
- Medium → `6px`
- Large → `8px`
- XLarge → `10px`
- Pill → `9999px`

#### App Store Buttons

| Component | Description |
|---|---|
| `App Store Badge` | Standard Apple/Google app store badge |
| `App Store Button` | Custom styled app store CTA button |

Sizes available: Rectangle (256×44) and Square (44×44)

#### Additional Buttons

| Component | Node ID | Description |
|---|---|---|
| `Like Button` | `11884:39675` | Thumbs up / like toggle button |
| `Icon Btn` | `11884:39703` | Icon-only circular/square buttons |
| `Social SignIn Buttons` | `11884:39637` | OAuth sign-in buttons (Google, Apple, etc.) |
| `Oval/Confetti Animation` | `12090:746` | Animated celebration button state |
| `Like - Dislike Animation` | `12078:699` | Animated like/dislike toggle |
| `Like-Disklike Button/Bar` | `12074:1277` | Rating bar with like/dislike |

### 7.2 Inputs

Located in: `Components → Inputs → 💠 Inputs`

| Component | Description |
|---|---|
| `Input` | Text input field variants |
| `Checkbox` | Checkbox with label |
| `List` | List selection component |
| `Dislike Form` | Feedback/dislike reason form |
| `Extra Info Tooltip` | Inline information tooltip |
| `Tag Pill / Tag Element` | Tag and pill UI elements |

**Input border radius:** `6px` (→ `Semantic/input`)

### 7.3 Notifications

Located in: `Notifications` page — notification banners and toasts.

---

## 8. Design Tokens (CSS Variables Reference)

```css
/* Fonts */
--font-title: 'Bricolage Grotesque', sans-serif;
--font-body: 'Inter', sans-serif;
--font-code: 'Roboto Mono', monospace;

/* Font Sizes */
--text-2xs: 0.625rem;  /* 10px */
--text-xs: 0.75rem;    /* 12px */
--text-s: 0.875rem;    /* 14px */
--text-m: 1rem;        /* 16px */
--text-l: 1.25rem;     /* 20px */
--text-xl: 1.5rem;     /* 24px */
--text-2xl: 2rem;      /* 32px */
--text-3xl: 2.25rem;   /* 36px */
--text-4xl: 3rem;      /* 48px */
--text-5xl: 4rem;      /* 64px */

/* Line Heights */
--leading-tight: 110%;   /* Title/5XL */
--leading-snug: 120%;    /* Title/4XL */
--leading-loose: 130%;   /* CAPS styles */
--leading-normal: 150%;  /* Most styles */
--leading-graph: 100%;   /* Body/S/Graph Legend only */

/* Brand */
--color-accent: #1770EF;
--color-accent-hover: #4D8FF5;
--color-accent-pressed: #0D5ED4;
--color-accent-tint: rgba(23,112,239,0.14);
--color-accent-tint-light: rgba(23,112,239,0.07);

/* Surfaces — Light */
--color-bg: #FFFFFF;
--color-bg-card: #FFFFFF;
--color-bg-page: #F1F1F1;
--color-bg-page-pale: #F5F5F5;
--color-bg-subtle: #E6E7EA;

/* Surfaces — Dark */
--color-bg-dark: #080D1A;
--color-bg-card-dark: #111827;
--color-bg-page-dark: #1A2236;

/* Text — Light */
--color-text-primary: #030D2D;
--color-text-secondary: #4F566C;
--color-text-tertiary: #818696;
--color-text-placeholder: #9A9EAB;
--color-text-disabled: #9A9EAB;

/* Borders — Light */
--color-border: #CDCFD5;
--color-border-hover: #9A9EAB;
--color-border-focus: #1770EF;
--color-border-error: #C9392A;
--color-border-subtle: #E6E7EA;

/* Status */
--color-error: #C9392A;
--color-warning: #FFB700;
--color-success: #16A34A;
--color-notice: #67C3BB;
--color-error-bg: rgba(201,57,42,0.07);
--color-warning-bg: rgba(255,183,0,0.07);
--color-success-bg: rgba(22,163,74,0.07);
--color-notice-bg: rgba(103,195,187,0.07);

/* Shadows */
--shadow-small: 0px 2px 8px rgba(0,0,0,0.04);
--shadow-normal: 0px 4px 16px rgba(0,0,0,0.08);
--shadow-big: 0px 8px 24px rgba(0,0,0,0.08);
--shadow-button: 0px 8px 16px rgba(0,0,0,0.10);
--shadow-dark: 0px 4px 8px rgba(0,0,0,0.30);

/* Blur */
--blur-bg-small: blur(24px);
--blur-bg-medium: blur(64px);
--blur-bg-large: blur(120px);
--blur-layer: blur(120px);

/* Spacing */
--space-xxxs: 2px;
--space-xxs: 4px;
--space-xs: 8px;
--space-s: 12px;
--space-m: 16px;
--space-l: 20px;
--space-xl: 24px;
--space-xxl: 32px;
--space-xxxl: 40px;
--space-xxl2: 48px;
--space-xxl3: 64px;
--space-xxl4: 80px;
--space-xxl5: 96px;

/* Border Radius */
--radius-null: 0px;
--radius-xxs: 2px;
--radius-xs: 4px;
--radius-s: 6px;
--radius-m: 8px;
--radius-l: 10px;
--radius-xl: 12px;
--radius-2xl: 16px;
--radius-3xl: 20px;
--radius-4xl: 24px;
--radius-5xl: 32px;
--radius-6xl: 40px;
--radius-round: 9999px;

/* Semantic Radius */
--radius-btn-small: 4px;    /* Semantic/button/small */
--radius-btn-medium: 6px;   /* Semantic/button/medium */
--radius-btn-large: 8px;    /* Semantic/button/large */
--radius-btn-xlarge: 10px;  /* Semantic/button/xlarge */
--radius-btn-pill: 9999px;  /* Semantic/button/Pill */
--radius-input: 6px;        /* Semantic/input */
--radius-card: 12px;        /* Semantic/card */
--radius-modal: 8px;        /* Semantic/modal */
--radius-tag: 4px;          /* Semantic/tag */
--radius-avatar: 9999px;    /* Semantic/avatar */
--radius-container: 20px;   /* Semantic/Container */
```

---

## 9. Spacing & Layout Conventions

| Token | Value | Usage |
|---|---|---|
| `xxxs` | `2px` | Hairline gaps |
| `xxs` | `4px` | Tight inline spacing |
| `xs` | `8px` | Internal component padding |
| `s` | `12px` | Compact padding — buttons, tags |
| `m` | `16px` | Default gap/padding |
| `l` | `20px` | Section padding |
| `xl` | `24px` | Card padding, section gaps |
| `xxl` | `32px` | Layout gutters |
| `xxxl` | `40px` | Major section breaks |
| `xxl2` | `48px` | Large section padding |
| `xxl3` | `64px` | Hero section padding |
| `xxl4` | `80px` | Page-level vertical rhythm |
| `xxl5` | `96px` | Maximum spacing — marketing |

**Card conventions** (from Semantic tokens):
- `border-radius: 12px` (`Semantic/card`)
- `border: 1px solid #CDCFD5` (`Border/Default`)
- `box-shadow: 0 8px 24px rgba(0,0,0,0.08)` (`Shadow/Big`)
- Typical card padding: `24px` (xl spacing token)

---

## 10. File Structure Overview

```
Apparatus.fig
├── Cover
├── Branding
│   └── Logo (Logo Mark, Full Logo)
├── Atoms
│   ├── Typography
│   └── Colors (Solid, Logo, Semantics, Gradients, Neutral, Overlay, Translucent)
├── Iconography
│   └── Icon Library (16px, 24px, 32px, 40px, 48px, 128px, Additional)
├── Components
│   ├── Buttons (Button, Button Attributes, Tooltips, App Store, Additional Buttons)
│   ├── Inputs (Input, Checkbox, List, Tags, Tooltip, Dislike Form)
│   └── Notifications
├── Patterns
└── Proto/File Helpers
```

---

## 11. Usage Notes for 6Labs

- **Primary brand color is `#1770EF`** (`Brand Blue/500`). Use for primary CTAs, active states, links, focus rings. Hover: `#4D8FF5`. Pressed: `#0D5ED4`.
- **Dark mode** is supported via the Semantic collection. Always bind to Semantic tokens (not primitives) for any component that supports dark mode.
- **Buttons** use `Shadow/Button Shadow` effect style (`0 8px 16px rgba(0,0,0,0.10)`). Always apply on interactive button components.
- **Glass/blur aesthetic** (`Gradient/Glass`, `Blur/Bg Blur-*`) is a key visual signature — use on floating panels and surface overlays.
- **Icon sizing default** for interactive elements: **24px**. Use **16px** for inline/compact UI. Use **32px+** for featured/empty states.
- **Typography defaults**: Body text → `Body/M/Regular` (Inter 14px Regular 150%). Supporting text → `Body/S/Regular` (12px). Headings → Bricolage Grotesque `Title/*`.
- **Card radius** is `12px` (`Semantic/card` → `xl`), not 24px.
- **Code blocks** use `Roboto Mono` — the only third font in the system.
- **Button labels** use their own dedicated `Button Label/*` text styles (Bricolage Grotesque SemiBold), not `Title/S` styles.
- **Complementary colors**: Pink (`#C20568`) and Purple (`#7B4CFF`) are available for secondary/accent button variants.
