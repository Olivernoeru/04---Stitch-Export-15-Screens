---
name: Sanctuary Calm
colors:
  surface: '#f2fbff'
  surface-dim: '#d0dce1'
  surface-bright: '#f2fbff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eaf6fb'
  surface-container: '#e4f0f5'
  surface-container-high: '#deeaef'
  surface-container-highest: '#d8e4ea'
  on-surface: '#121d21'
  on-surface-variant: '#3f4849'
  inverse-surface: '#273236'
  inverse-on-surface: '#e7f3f8'
  outline: '#6f7979'
  outline-variant: '#bfc8c9'
  surface-tint: '#26676b'
  primary: '#045357'
  on-primary: '#ffffff'
  primary-container: '#2a6b6f'
  on-primary-container: '#aae9ed'
  inverse-primary: '#93d1d5'
  secondary: '#a53b25'
  on-secondary: '#ffffff'
  secondary-container: '#fe7d61'
  on-secondary-container: '#721604'
  tertiary: '#005637'
  on-tertiary: '#ffffff'
  tertiary-container: '#226f4d'
  on-tertiary-container: '#a3efc4'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#aeeef2'
  primary-fixed-dim: '#93d1d5'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f53'
  secondary-fixed: '#ffdad3'
  secondary-fixed-dim: '#ffb4a4'
  on-secondary-fixed: '#3e0500'
  on-secondary-fixed-variant: '#852410'
  tertiary-fixed: '#a7f3c8'
  tertiary-fixed-dim: '#8bd6ad'
  on-tertiary-fixed: '#002112'
  on-tertiary-fixed-variant: '#005234'
  background: '#f2fbff'
  on-background: '#121d21'
  surface-variant: '#d8e4ea'
typography:
  display-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 30px
    fontWeight: '700'
    lineHeight: 38px
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  title-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 15px
    fontWeight: '400'
    lineHeight: 22px
  label-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '600'
    lineHeight: 20px
  label-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 13px
    fontWeight: '500'
    lineHeight: 18px
  caption:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  gutter: 1rem
  margin: 1.25rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.25rem
  space-xl: 1.5rem
---

## Brand & Style

This design system is engineered for trauma-informed, high-stakes mobile environments where safety, clarity, and emotional containment are paramount. The product serves individuals experiencing acute stress, distress, or danger, alongside advocates and supporters seeking structured guidance.

### Design Movement & Archetype
The visual language operates on **Soft Humanist Minimalism with Tactile Reassurance**. Rather than adopting an austere institutional look or an overly clinical healthcare facade, the design integrates organic warmth, gentle visual boundaries, and radical visual clarity:
- **Calm & Non-Intimidating:** Eliminates aggressive alarms, harsh high-frequency vibrations, or disorienting saturated accents.
- **Supportive & Grounding:** Uses soft ivory canvas backdrops paired with grounding slate and teal tones that reduce cognitive load during panic or hyperarousal.
- **Immediate Discretion & Safety:** Prioritizes persistent safety architecture, including a non-stigmatizing Quick Exit affordance and rapid navigation shielding.

## Colors

The palette operates under a strict light-only mandate. High-stress contexts require unambiguous daylight contrast ratios that avoid the harsh glare of stark blue-white backgrounds or the low-light visibility pitfalls of dark themes.

### Color Tokens & Semantic Roles
- **Canvas Base (`#FAF8F5`):** Soft Ivory canvas providing a comforting, non-sterile foundation.
- **Surface Elevation (`#FFFFFF`):** Pure white container backgrounds creating soft, legible isolation for cards and modals.
- **Primary Teal (`#2A6B6F`):** Deep oceanic teal used for trusted primary actions, verified legal statuses, and confident progress indicators.
- **Primary Soft (`#E3EFEC`):** Gentle wash for active selection states, chips, and safe category highlights.
- **Help / Emergency Terracotta (`#B3452E`):** A warm, protective terracotta tone reserved exclusively for hotlines, immediate help triggers, and crisis contacts—deliberately avoiding clinical siren red.
- **Help Soft (`#FBE9E4`):** Soft rose-peach tint for alert containers and emergency card surfaces.
- **Success / Protective Green (`#2F7A57`):** Earthy forest green indicating recorded evidence, sent reports, and secured notes.
- **Attention / Warning (`#8A5A00` over `#FFF3D6`):** Warm amber on soft marigold backing for privacy warnings and legal disclaimers.
- **Typography & Structure:**
  - Primary Text: `#1F2A2E` (Charcoal Teal, passes AAA at 13.86:1 contrast against `#FAF8F5`).
  - Secondary Text: `#5B6B70` (Muted Slate Teal, passes AA at 5.24:1 contrast).
  - Subtle Border / Hairline: `#E4DFD8` (Low-contrast warm stone outline for tactile structure).
  - Quick Exit: `#1F2A2E` high-contrast solid/pill outline for instantaneous visual acquisition.

## Typography

The typography uses **Plus Jakarta Sans** across all hierarchies. Its open apertures, warm geometric curves, and clean letterforms deliver legibility without clinical detachment.

### Hierarchy & Cognitive Rules
- **Line Length & Heights:** Body text maintains an intentional 1.5 ratio (`16px/24px`) to reduce ocular fatigue and visual tracking jumps when reading complex legal documents or safety steps.
- **Headlines:** Set in Bold (`700`) and SemiBold (`600`) to anchor scanning eyes. Maximum mobile headline size is capped at 30px to prevent awkward multiline line breaks in small portrait viewports.
- **Metadata & Labels:** Captions and labels avoid thin weights; all utility text stays at Medium (`500`) or SemiBold (`600`) at or above `12px` to ensure complete accessibility under low screen brightness.

## Layout & Spacing

The layout is built specifically for portrait mobile screens (`360x800px` to `390x844px`), structured around a strict 4px/8px incremental rhythm.

### Grid & Margins
- **Screen Margins:** Fixed `20px` (`1.25rem`) horizontal margins on canvas edges provide breathing room and prevent accidental touch dismissals near device bezels.
- **Vertical Flow:**
  - `space-xs` (4px): Micro-spacing between paired label-value items.
  - `space-sm` (8px): Gaps between list card elements and badge internal padding.
  - `space-md` (16px): Standard gap between related form fields and stacked cards.
  - `space-lg` (20px): Structural screen padding and component cluster separation.
  - `space-xl` (24px): Clear thematic section transitions.
- **Touch Ergonomics:** All primary interactive components maintain a minimum tap target height of 48px to accommodate shaky or hurried interaction.

## Elevation & Depth

This design system avoids high-contrast dropshadows and heavy blurs that create visual noise or anxiety. Visual layering is achieved through **Tonal Stacking and Low-Contrast Warm Outlines**.

### Elevation Hierarchy
1. **Level 0 (Canvas Base):** Flat `#FAF8F5` Soft Ivory background.
2. **Level 1 (Card & Content Blocks):** Pure white `#FFFFFF` surface bordered by a 1px hairline stroke in `#E4DFD8`. Soft ambient shadow: `0 2px 8px rgba(31, 42, 46, 0.04)`.
3. **Level 2 (Interactive Floating Elements & Sheets):** Surface `#FFFFFF`, hairline `#E4DFD8`, elevated shadow: `0 8px 24px rgba(31, 42, 46, 0.08)`.
4. **Emergency / Persistent Overlays:** Floating action items (such as the persistent Quick Exit header bar) remain anchored with an edge-to-edge subtle bottom hairline `#E4DFD8` and background opacity of `rgba(250, 248, 245, 0.96)` with a 12px backdrop blur.

## Shapes

The shape system adopts smooth, protective geometry to promote comfort and tactile safety. Sharp corners (0px) are entirely forbidden.

### Geometry Specifications
- **Standard Cards & Containers:** `16px` corner radius. Softens content enclosures and avoids aggressive points.
- **Buttons & Form Fields:** `14px` corner radius. Creates a comfortable, welcoming tap surface.
- **Pills, Chips & Quick Exit Bar:** `9999px` (Full Pill). Used for filters, status tags, and high-visibility exit buttons to indicate urgent tactile responsiveness.

## Components

### Buttons
- **Primary Action:** Background `#2A6B6F`, text `#FFFFFF`, border-radius `14px`, height `52px`. Font `label-lg` (Plus Jakarta Sans 14px SemiBold).
- **Emergency / Crisis Action:** Background `#B3452E`, text `#FFFFFF`, border-radius `14px`, height `54px`. Accompanied by direct call or SOS iconography.
- **Secondary / Ghost:** Background `#E3EFEC`, text `#2A6B6F`, border 0, border-radius `14px`, height `50px`.
- **Outline Alternative:** Background transparent, border `1.5px solid #2A6B6F`, text `#2A6B6F`.

### Quick Exit Control
- **Persistent Header Pill:** Fixed at the top or bottom of every critical screen. Pill shape (`rounded-full`), height `44px`, background `#FFFFFF`, border `2px solid #1F2A2E`, text `#1F2A2E`, font SemiBold 14px with icon. On click: instantaneously purges active cache, closes socket sessions, and opens an innocuous browser tab (e.g., weather or search engine).

### Cards
- **Resource & Legal Cards:** Background `#FFFFFF`, corner radius `16px`, border `1px solid #E4DFD8`, padding `16px` or `20px`. Contains clear hierarchical division: topic badge, headline (`title-md`), summary text (`body-md`), and non-intimidating inline link action.
- **Crisis Callout Card:** Background `#FBE9E4`, border `1px solid #F3C7BE`, corner radius `16px`, padding `16px`. Title in `#B3452E`.

### Form Fields & Inputs
- **Text Inputs:** Background `#FFFFFF`, height `52px`, radius `14px`, border `1px solid #E4DFD8`, text `#1F2A2E`, placeholder `#5B6B70`. Focus ring: `2px solid #2A6B6F` with zero blur offset.
- **Helper & Safety Text:** Placed beneath inputs in `caption` (12px), `#5B6B70`. Never relies solely on red text to signal validation warnings.

### Checkboxes & Radio Elements
- **Selection Controls:** `22px` width and height. Unchecked state: `#FFFFFF` filled with `1.5px solid #E4DFD8` border. Checked state: `#2A6B6F` filled with pure white check or inner dot. Radius `6px` for checkboxes, `9999px` for radios.

### Chips & Filter Tags
- **Informational Chips:** Height `34px`, radius `9999px`, horizontal padding `14px`. Unselected: `#FAF8F5` surface, border `1px solid #E4DFD8`, text `#5B6B70`. Selected: `#E3EFEC` background, text `#2A6B6F`, border `1px solid #2A6B6F`.

### Stealth & Privacy Banner
- **Contextual Safe-Reading Banner:** A dismissible, warm amber card (`#FFF3D6` background, `#8A5A00` text) guiding users on how to clear device logs or browse discreetly without causing panic.