# Workspace Page Overrides

> **PROJECT:** Prompt Optimizer
> **Generated:** 2026-11-17 22:13:39
> **Page Type:** Dashboard / Data View

> ⚠️ **IMPORTANT:** Rules in this file **override** the Master file (`design-system/MASTER.md`).
> Only deviations from the Master are documented here. For all other rules, refer to the Master.

---

## Page-Specific Rules

### Layout Overrides

- **Max Width:** 1680px, centered
- **Layout:** Desktop two-column workbench with a resizable divider; single-column stacked flow on compact screens
- **Desktop hierarchy:** App shell → two-column workspace → prompt/material/settings/preview/result cards
- **Left column:** original prompt, model, strategy and actions in the first card; optimized workspace and versions in the second
- **Right column:** test material, group/output settings, preview and final results in layered cards
- **Avoid:** marketing hero sections, a centered 800px single-column dashboard, or hidden context that forces page switching

### Spacing Overrides

- **Content Density:** Compact but breathable
- **Canvas Padding:** 20–24px desktop, 12–16px tablet, 8–12px compact
- **Card Gap:** 16px desktop, 12px tablet, 8–12px compact
- **Card Padding:** 16–20px desktop, 12–16px compact

### Typography Overrides

- **Preferred Family:** SF Pro on Apple platforms; fall back to PingFang SC, Segoe UI and the platform UI font
- **Titles:** 15–18px, 600 weight
- **Labels:** 12–13px, 500 weight
- **Body/editor:** 14–16px, 1.6–1.7 line-height
- Avoid downloading Plus Jakarta Sans for the application shell; preserve fast startup and native CJK rendering

### Color Overrides

- **Page Background:** `#F6F8FC`
- **Card Background:** `#FFFFFF`
- **Primary:** `#6366F1`
- **Secondary:** `#8B5CF6`
- **Primary Text:** `#1F2937`
- **Muted Text:** `#6B7280`
- **Border:** `#E8EDF5`
- **Success:** `#059669`
- Use a faint indigo-to-white radial wash in the page background, not saturated card gradients

### Component Overrides

- **Cards:** 14–16px radius, 1px cool border, restrained shadow `0 12px 32px rgba(15, 23, 42, 0.06)`
- **Header:** translucent white material with blur; navigation uses compact pill tabs
- **Actions:** one visual primary CTA per panel; configuration utilities collapse visually and retain text labels in accessible names/tooltips
- **Inputs:** white or near-white field surfaces with a visible indigo focus ring
- **Icons:** Lucide only; no emoji as structural icons
- **Empty states:** calm neutral illustration/icon treatment; no large raster mockup screenshots
- **Motion:** 150–220ms for normal transitions; press feedback on pointer-down; reduced-motion cross-fade only

---

## Page-Specific Components

- No unique components for this page

---

## Recommendations

- Use restrained indigo highlights and active pills rather than gradients on every surface.
- Keep the dual-column workflow visible on desktop and preserve existing scroll/state ownership.
- Use translucency only for floating app chrome and overlays, not for nested content cards.
- Preserve existing functionality and E2E selectors while changing visual density and hierarchy.
- Validate at 1440×900, 1280×800, 768px and 375px, with both light and dark themes.
