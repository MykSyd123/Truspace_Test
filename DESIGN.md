---
name: Operational Taskboard & Work Orders
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
  secondary: '#006780'
  on-secondary: '#ffffff'
  secondary-container: '#76dcff'
  on-secondary-container: '#006077'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#25005a'
  on-tertiary-container: '#9863ff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#b7eaff'
  secondary-fixed-dim: '#6cd3f7'
  on-secondary-fixed: '#001f28'
  on-secondary-fixed-variant: '#004e61'
  tertiary-fixed: '#eaddff'
  tertiary-fixed-dim: '#d2bbff'
  on-tertiary-fixed: '#25005a'
  on-tertiary-fixed-variant: '#5a00c6'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 30px
    fontWeight: '600'
    lineHeight: 38px
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Inter
    fontSize: 22px
    fontWeight: '600'
    lineHeight: 28px
  headline-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: '400'
    lineHeight: 22px
  body-md:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-lg:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '600'
    lineHeight: 18px
  label-md:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '600'
    lineHeight: 14px
  label-sm:
    fontFamily: Inter
    fontSize: 10px
    fontWeight: '700'
    lineHeight: 12px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  gutter: 1rem
  gutter-mobile: 0.75rem
  margin: 1.5rem
  margin-mobile: 1rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 0.75rem
  space-lg: 1.25rem
  space-xl: 2rem
---

## Brand & Style

The design system establishes a high-performance, precision-driven operational workspace built for mission-critical task orchestration and work order management. It conveys absolute reliability, quiet technical authority, and frictionless clarity under high cognitive load.

The design philosophy combines **Precision Minimalism** with structured data density:
- **Calm, Distraction-Free Canvas:** Neutral slate foundations step backward, allowing active operational data and status state-changes to command immediate focus.
- **Architectural Rigor:** Sharp alignment, deliberate border delineations, and disciplined micro-interactions replace heavy shadows or decorative ornamentation.
- **Information Density with Breathing Room:** Compact data presentation engineered for scanning speed, paired with exact vertical rhythms so dense board views remain readable over extended operational shifts.
- **Vibrant Status Signatures:** Functional color acts as unambiguous telemetry. State indicators cut cleanly through neutral surfaces to communicate health, urgency, and flow at a glance.

## Colors

The palette is anchored by a deep slate core, supported by clinical neutral grays and dedicated semantic channels for operational telemetry:

- **Primary (`#0F172A` - Slate 900):** Anchors primary text, dominant controls, and structural boundaries. Conveys stability and institutional precision.
- **Neutral Foundations:**
  - Canvas / Surface Neutral: `#F8FAFC` (Slate 50) for underlying board canvasing.
  - Card & Container Surface: `#FFFFFF` (Pure White) for task units and inspectable panels.
  - Subtle Surface Tint: `#F1F5F9` (Slate 100) for column tracks, inner wells, and disabled fills.
  - Border Hairlines: `#E2E8F0` (Slate 200) for default containment borders; `#CBD5E1` (Slate 300) for structural splitters and hover transitions.
  - Typography Neutral: `#0F172A` (Slate 900, Primary Text), `#334155` (Slate 700, Secondary Details), `#64748B` (Slate 500, Metadata & Icons), `#94A3B8` (Slate 400, Placeholders).
- **Status Channels & Work Order Semantics:**
  - **In-Progress (`#0891B2` Cyan / `#06B6D4` Teal):** Signals active throughput and underway assignments. Applied with 10% tinted background fills (`#ECFEFF`) for containment badges.
  - **Pending / New (`#D97706` Amber / `#F59E0B` Gold):** Denotes items requiring dispatch, triage, or unassigned backlog entries. Accompanied by `#FFFBEB` pill surfaces.
  - **Completed (`#059669` Emerald):** Represents terminal success, closed work orders, and verified tasks. Accompanied by `#ECFDF5` background fills.
  - **In Review (`#7C3AED` Purple / `#8B5CF6` Violet):** Denotes quality audits, supervisory sign-offs, and compliance verification. Accompanied by `#F5F3FF` fills.
  - **Urgent / Blocked (`#DC2626` Crimson):** Reserved strictly for critical escalations, blocking dependencies, and SLA breaches. Accompanied by `#FEF2F2` alert fills.

## Typography

The type system prioritizes mechanical legibility and tabular density through Inter. Letter forms are calibrated for high-speed scanning across kanban boards, data grids, and execution logs:

- **Monospace Numerics:** All dynamic counters, order identifiers (e.g., `WO-8924`), time estimates, and timestamps must leverage tabular figures (`font-variant-numeric: tabular-nums`) to prevent horizontal jitter during real-time board updates.
- **Hierarchy Rules:**
  - Board and Module Titles utilize `headline-lg` / `headline-md` at 600 weight to set clear context without visual dominance over task lists.
  - Task and Work Order Titles default strictly to `body-md` with semi-bold (600) emphasis for immediate scanning.
  - Metadata, assignee roles, timestamps, and secondary card annotations use `body-sm` and `label-md`.
  - Micro-tags, SLA badges, and priority indicators employ `label-sm` with uppercase transformation and `+0.04em` tracking for crisp delineation at tiny scales.

## Layout & Spacing

The layout is built around an enterprise operational canvas optimized for horizontal and vertical flow:

- **Layout Grid & Flow:**
  - **Desktop (>= 1280px):** Multi-column horizontal board viewport (`min-width: 300px`, `max-width: 360px` per column) over a fixed-height, full-bleed viewport. Columns scroll independently. Main board area features a `1.5rem` canvas margin and `1rem` column gutters.
  - **Tablet (768px - 1279px):** Horizontally panning board with snapping columns; active swimlanes expand to `320px`. Top command bar collapses filter pills into an expandable drawer.
  - **Mobile (< 768px):** Segmented tab switcher for task stages (Pending, In Progress, Review, Completed) rendering a single vertical stream at a time, backed by `1rem` edge margins and `0.5rem` item gaps.
- **Internal Spacing Discipline:**
  - Cards utilize `space-md` (`0.75rem` / 12px) internal padding to preserve tight information density while maintaining clean tap and click targets.
  - Compact sub-elements (avatar stacks, tag rows, action triggers) align with `space-xs` (4px) and `space-sm` (8px) gaps.

## Elevation & Depth

Visual hierarchy is maintained through crisp border outlines supplemented by subtle, non-intrusive ambient shadows that never muddy board clarity:

- **Resting Layer (Surface):** Default task cards rest on `surface-primary` (`#FFFFFF`) with a 1px solid border of `#E2E8F0` (Slate 200). Resting elevation uses a feather-light shadow: `0 1px 2px 0 rgba(15, 23, 42, 0.04)`.
- **Hover Layer:** When hovering over an interactive task card or work order row, the border transitions smoothly to `#CBD5E1` (Slate 300) and the shadow expands subtly: `0 4px 12px -2px rgba(15, 23, 42, 0.08), 0 2px 4px -1px rgba(15, 23, 42, 0.04)`. The card elevates by `-1px` on the Y-axis.
- **Active Drag / In-Transit State:** Dragged cards gain elevated focus via a primary accent ring hint: border color shifts to `#0891B2` with an ambient lift shadow of `0 12px 28px -4px rgba(15, 23, 42, 0.16), 0 4px 8px -2px rgba(15, 23, 42, 0.06)`. Opacity is sustained at 0.96.
- **Drop Zones:** Column drop targets display a 1.5px dashed border in `#94A3B8` (Slate 400) filled with an ultra-light tint `#F8FAFC`.
- **Overlays & Drawers:** Detail inspection drawers and modal popovers cast an authoritative depth shadow: `0 20px 32px -6px rgba(15, 23, 42, 0.18), 0 8px 16px -4px rgba(15, 23, 42, 0.08)` bordered by `#CBD5E1`.

## Shapes

The design system embraces a **Soft / Engineering Precision** geometry (`roundedness: 1`):

- **Core Radius (`0.25rem` / 4px):** Applied to standard controls, checkboxes, text input fields, tooltips, and compact status pills.
- **Medium Radius (`0.375rem` - `0.5rem` / 6px - 8px):** Applied to kanban task cards, dropdown menus, filter badges, and operational action buttons.
- **Large Radius (`0.75rem` / 12px):** Reserved for column container wells, side inspection drawers, and work order creation modals.
- **Circular (`9999px`):** Used exclusively for assignee avatars, active status dots, and round icon trigger buttons (e.g., quick-add or overflow menus).

## Components

### Cards (Taskboard & Work Order Cards)
- **Structure:** White background, 1px solid `#E2E8F0` border, 6px corner radius.
- **Header:** Top row houses the tabular Work Order ID (e.g., `#WO-1042` in Slate 500) aligned left, and priority indicator aligned right.
- **Body:** Task title set in 13px semi-bold slate-900 with a 2-line clamp maximum, followed by optional contextual summary in 12px slate-600.
- **Footer:** Separated by a hairline rule or 8px vertical spacing: Left-aligned status chip and tag; right-aligned assignee avatar and due-date counter.
- **Hover State:** 150ms ease-in-out transition elevating shadow and shifting border to Slate 300.

### Status Badges & Priority Chips
- **Status Pills:** Pill geometry with 4px radius. 11px semi-bold uppercase label. Tinted background (10-15% opacity) coupled with saturated text:
  - *In-Progress:* `#ECFEFF` background, `#0E7490` text, optional `#06B6D4` pulsing dot.
  - *Pending:* `#FFFBEB` background, `#B45309` text.
  - *Review:* `#F5F3FF` background, `#6D28D9` text.
  - *Completed:* `#ECFDF5` background, `#047857` text.
- **Priority Indicators:** Compact vertical bars or directional chevrons:
  - *Critical:* Crimson `#DC2626` with double upward chevron.
  - *High:* Amber `#D97706` single upward chevron.
  - *Medium:* Slate `#64748B` horizontal dash.
  - *Low:* Slate `#94A3B8` single downward chevron.

### Buttons & Quick Actions
- **Primary Button:** `#0F172A` (Slate 900) fill, `#FFFFFF` text, 6px radius, hover to `#1E293B`, active pressed to `#020617`.
- **Secondary / Action Button:** `#FFFFFF` fill with 1px `#E2E8F0` border, `#334155` text. Hover to `#F8FAFC` background and `#CBD5E1` border.
- **Icon Actions:** 28x28px square with 4px radius, transparent fill, hover with `#F1F5F9` background, Slate 500 icon shifting to Slate 900 on hover.

### Form Inputs & Search Fields
- **Search Bar:** `#FFFFFF` fill, 1px `#CBD5E1` border, 6px radius, inset search glyph in Slate 400. Focus ring: 2px solid `#0891B2` with zero offset blur.
- **Filter Chips:** 28px height, Slate 100 resting background, text Slate 700. Active filtered state toggles to `#0F172A` text and `#0891B2` border accent.

### Avatars & Assignee Clusters
- **Avatar Geometry:** Exactly circular (24px for card footers, 32px for detail headers).
- **Assignee Ring:** Bordered by a 2px `#FFFFFF` halo to allow clean overlapping in assignee stacks. Over-count badges (e.g., `+3`) use `#F1F5F9` fill and 10px bold text.

### Checkboxes & Stage Checklists
- **Checkboxes:** 16x16px with 4px radius, 1.5px border `#94A3B8`. Checked state fills `#0F172A` with a crisp white check glyph. Indeterminate states use a centered 8px horizontal bar.