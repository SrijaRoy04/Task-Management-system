---
name: Task & Flow Modern Work
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
  on-surface-variant: '#474554'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#787586'
  outline-variant: '#c8c4d7'
  surface-tint: '#5847d2'
  primary: '#5341cd'
  on-primary: '#ffffff'
  primary-container: '#6c5ce7'
  on-primary-container: '#faf6ff'
  inverse-primary: '#c6bfff'
  secondary: '#0058be'
  on-secondary: '#ffffff'
  secondary-container: '#2170e4'
  on-secondary-container: '#fefcff'
  tertiary: '#006645'
  on-tertiary: '#ffffff'
  tertiary-container: '#008259'
  on-tertiary-container: '#e1ffec'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e4dfff'
  primary-fixed-dim: '#c6bfff'
  on-primary-fixed: '#160066'
  on-primary-fixed-variant: '#4029ba'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#adc6ff'
  on-secondary-fixed: '#001a42'
  on-secondary-fixed-variant: '#004395'
  tertiary-fixed: '#6ffbbe'
  tertiary-fixed-dim: '#4edea3'
  on-tertiary-fixed: '#002113'
  on-tertiary-fixed-variant: '#005236'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
  canvas-bg: '#F8FAFC'
  surface-card: '#FFFFFF'
  border-subtle: '#E2E8F0'
  border-strong: '#CBD5E1'
  text-primary: '#0F172A'
  text-secondary: '#475569'
  text-muted: '#94A3B8'
  status-raised-bg: '#EFF6FF'
  status-raised-text: '#2563EB'
  status-pending-bg: '#FEF3C7'
  status-pending-text: '#D97706'
  status-closed-bg: '#ECFDF5'
  status-closed-text: '#059669'
  priority-high-bg: '#FFE4E6'
  priority-high-text: '#E11D48'
  priority-med-bg: '#EFF6FF'
  priority-med-text: '#2563EB'
  priority-low-bg: '#DCFCE7'
  priority-low-text: '#16A34A'
typography:
  display:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: -0.015em
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 26px
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 15px
    fontWeight: '600'
    lineHeight: 22px
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  label-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 14px
    letterSpacing: 0.04em
  display-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 26px
    fontWeight: '700'
    lineHeight: 34px
    letterSpacing: -0.02em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  gutter: 1.25rem
  margin: 2rem
  gutter-mobile: 0.75rem
  margin-mobile: 1rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 0.75rem
  space-lg: 1.25rem
  space-xl: 2rem
---

## Brand & Style

This design system establishes a high-performance, focused work environment for modern cross-functional teams, project managers, and operations leads. Drawing direct inspiration from clean productivity software and robust enterprise tracking tools, the design pairs extreme clarity with energetic, purposeful color accents.

The design movement centers on **Corporate / Modern Minimalist SaaS**:
- **Purity of Surface:** Crisp white canvases grounded by subtle, cool gray secondary surfaces (`#F8FAFC`, `#F1F5F9`) keep cognitive load at absolute zero.
- **Intentional Vivid Accents:** A primary electric violet/purple acts as the signature anchor for focal interactions, primary actions, and selected workspace states.
- **Scannable Status Architecture:** High-contrast semantic pills and iconography (flame for urgent priority, clean dot and pill meters for completion) transform dense task backlogs and Kanban boards into instantly digestible visual systems.
- **Micro-Delight & Professional Poise:** Subtle border definitions, pill-shaped avatar groups, and razor-sharp typographic hierarchies provide a refined sense of structure without feeling heavy or industrial.

## Colors

The palette is tuned specifically for complex productivity workspaces where legibility, fast categorization, and visual hierarchy take priority.

### Surface and Structure
- **Canvas Base (`canvas-bg`):** `#F8FAFC` provides a cool, non-glare foundation that elevates `#FFFFFF` cards and sheet panels naturally.
- **Dividers & Strokes (`border-subtle` & `border-strong`):** Crisp 1px lines using slate variations establish strict table rows, card perimeters, and vertical splitters without adding heavy contrast.

### Action & Identification
- **Primary Violet (`primary_color_hex` - `#6C5CE7`):** Powers key global actions ("+ Add New", active navigation indicators, checkboxes on completion). 
- **Secondary Blue (`secondary_color_hex` - `#3B82F6`):** Drives secondary analytics, info states, and linked metadata.

### Semantic Status & Priority Scale
- **Status Indicators:**
  - **Raised / In Review:** Soft tint `#EFF6FF` with `#2563EB` text.
  - **Pending / In Progress:** Soft tint `#FEF3C7` with `#D97706` text or warm violet variant.
  - **Closed / Completed:** Crisp fresh tint `#ECFDF5` with `#059669` text.
- **Priority Indicators:**
  - **High (Urgent):** Vibrant rose `#FFE4E6` fill with `#E11D48` text and flame glyphs.
  - **Medium:** Cool blue/amber `#EFF6FF` with `#2563EB` badge indicator.
  - **Low:** Subdued pasture `#DCFCE7` with `#16A34A` label.

## Typography

The design system standardizes on **Plus Jakarta Sans** across all roles. Its geometric yet slightly rounded character shapes deliver modern warmth while retaining high legibility in dense tabular structures and micro-badge interfaces.

### Hierarchy Guidelines
- **Display & Main Titles:** Display and `headline-lg` are reserved for major board views (e.g., "Tasks", "Project Closing Phase"), using tight negative letter spacing for crisp presence.
- **Table & Column Headers:** Column groups and Kanban titles utilize `headline-sm` (`15px, 600`) to present unambiguous section starts.
- **Data Rows & Task Labels:** `body-md` (`14px, 400`) handles interactive task descriptions. When tasks are marked complete, apply strikethrough styling alongside `text-muted` color.
- **Tags, Pills & Table Column Metas:** Utilize `label-sm` (`11px, 700`, uppercase) for table headers (`DONE`, `ASSIGNEE`, `PRIORITY`, `%`, `STATUS`) to maintain industrial-grade scanning speed.

## Layout & Spacing

The layout adopts a multi-tier dashboard model combining fixed operational rails with fluid content areas.

### Layout Structure
- **Persistent Left Navigation:** A compact or expanded sidebar (`72px` collapsed or `240px` expanded) docked to the left edge, maintaining clear separation between top-level workspaces, boards, and personal views.
- **Top Utility Header:** A unified header (`64px` height) incorporating global search, workspace switchers, notification bells with unread badges, and user profile badges.
- **View Switcher Subheader:** Direct view toggles (List, Grid, Calendar, Gantt, Kanban) aligned cleanly above data surfaces with filter dropdowns anchored to the right.
- **Main Canvas:** Fluid grid adapting smoothly between Kanban card columns (`min-width: 260px`, `max-width: 340px`) and comprehensive data tables spanning 100% available viewport width.

### Breakpoints & Responsive Behavior
- **Desktop (1200px+):** Full multi-column Kanban boards scrollable horizontally; complete tabular data with all metadata columns expanded.
- **Tablet (768px - 1199px):** Sidebar collapses into icon-only mode; Kanban views retain column swiping; table rows collapse secondary percentages into inline micro-tags.
- **Mobile (< 768px):** Navigation migrates to an off-canvas drawer or sticky bottom nav; task views present segmented single-column lists with full-width cards.

## Elevation & Depth

Visual depth follows a minimalist, low-shadow paradigm, relying on tonal layering, delicate perimeter strokes, and diffused ambient shadows.

### Elevation Levels
- **Level 0 (Canvas Base):** Flat `#F8FAFC` background surface.
- **Level 1 (Card & Row Surfaces):** Pure white (`#FFFFFF`) containers framed by a crisp `1px solid #E2E8F0` hairline border. Ambient shadow is ultra-soft: `box-shadow: 0 1px 3px rgba(15, 23, 42, 0.04), 0 1px 2px rgba(15, 23, 42, 0.02)`.
- **Level 2 (Hover States & Active Cards):** Applied to Kanban cards on hover or drag: `box-shadow: 0 10px 15px -3px rgba(108, 92, 231, 0.08), 0 4px 6px -2px rgba(15, 23, 42, 0.03)` with border shifting subtly to `#CBD5E1`.
- **Level 3 (Dropdowns & Modals):** Crisp overlays featuring `box-shadow: 0 20px 25px -5px rgba(15, 23, 42, 0.1), 0 10px 10px -5px rgba(15, 23, 42, 0.04)`.

## Shapes

The design system maintains a balanced, friendly geometric standard. The core shape radius is set to **`2` (Rounded)**:
- Standard interactive elements (buttons, inputs, dropdown menus, table container shells) use `8px` (`0.5rem`) corner rounding.
- Kanban task cards and floating surface panels utilize `12px` (`0.75rem`) to `16px` (`1rem`) corner rounding to communicate modularity.
- Status badges, priority tags, and avatar frames follow a pure **pill / circular geometry** (`rounded-full` / `9999px`), creating immediate visual separation between structural containers and metadata chips.

## Components

### Primary & Action Buttons
- **Primary CTA ("+ Add New", "+ New Task"):** Vibrant violet background (`#6C5CE7`), white text, `8px` radius, `0 10px 20px -5px rgba(108, 92, 231, 0.4)` subtle glow. Hover triggers `#5B4DFF`.
- **Ghost / Utility Buttons:** Transparent background with subtle `#E2E8F0` border, `#475569` text, and clean SVG icons.

### Status & Priority Pills
- **Status Badges:** Height `24px`, horizontal padding `10px`, pill-shaped (`9999px`), `font-size: 11px`, `font-weight: 700`.
  - *Raised / Backlog:* Tinted blue background (`#EFF6FF`), text `#2563EB`.
  - *In Review / In Progress:* Tinted violet or warm amber (`#FEF3C7`), text `#D97706`.
  - *Done / Closed:* Emerald background (`#ECFDF5`), text `#059669`.
- **Priority Indicators:**
  - *High:* Pill with flame icon, soft pink background (`#FFE4E6`), text `#E11D48`.
  - *Medium:* Upward chevron or dash badge in blue/amber.
  - *Low:* Subdued green badge (`#DCFCE7`), text `#16A34A`.

### Tables & List Views
- **Header Row:** Crisp uppercase typography (`11px`, slate-500, tracking-wider), light gray bottom border (`#E2E8F0`), compact vertical spacing (`12px`).
- **Data Rows:** `56px` height, clean horizontal separator line, `#FFFFFF` background. Hover triggers `#F8FAFC`.
- **Checkboxes:** Custom square checkboxes with `4px` radius. Inactive: `1.5px solid #CBD5E1`. Active: solid fill `#0F172A` or `#6C5CE7` with white checkmark. Completed row triggers text strike-through and `opacity: 0.5`.
- **Progress Indicators:** Slim horizontal progress bars (`6px` height, `rounded-full`), track `#F1F5F9`, fill `#10B981` (emerald) or `#6C5CE7` (violet) accompanied by a precise percentage readout (`12px`, tabular nums).

### Cards (Kanban)
- **Container:** `#FFFFFF` background, `12px` rounded corners, `1px solid #F1F5F9` perimeter stroke, soft shadow.
- **Internal Card Hierarchy:**
  1. Top Row: Task title in bold `14px` next to right-aligned status or priority pill.
  2. Middle Row: Due date metadata with calendar icon (`12px`, muted gray).
  3. Bottom Track: Slim progress bar (`4px`) with completion fill.
  4. Footer: Overlapping assignee avatar stack (`24px` circles with `2px` white border) and a lightweight `+` add assignee button.

### Form Inputs & Search Fields
- Single-line search bar with inset search magnifying glass icon, flat `#FFFFFF` or `#F8FAFC` fill, `1px solid #E2E8F0` border, `8px` corner radius, smoothly transitioning to `#6C5CE7` focus ring with `2px` offset.