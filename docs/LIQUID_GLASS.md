# Liquid Glass Material System

**FigCraft Location**: Page 09 (Board DS 01: Liquid Glass Materials, Navigation & Controls)
**Reference Preview**: [`01-liquid-glass-materials-controls.png`](../previews/design-system/01-liquid-glass-materials-controls.png)

---

## 1. The Restraint Principle

Liquid Glass fails when applied indiscriminately to every card on a screen. AUREL enforces a strict **surface separation rule**:

- **Floating Interactive Chrome (Liquid Glass)**: Floating 5-tab navigation capsule, message & AI composers, search pills, translucent top headers, contextual bottom sheets, video reaction rails, and call decks.
- **Dense Content Surfaces (Zero Blur)**: Direct chat threads, long-form post text, notification lists, and Settings rows use solid Pure White (`#FFFFFF`), Frosted Surface (`#F7FAFF` / `#F2F5FA`), or Midnight Navy (`#080E1C` / `#111B2C`) so reading contrast remains high regardless of scrolling media.

## 2. Four Material Specifications

| Material Component | Fill Hex / Alpha | Stroke | Native FigCraft Effects | Target Surfaces |
| :--- | :--- | :--- | :--- | :--- |
| `Aurel/Material/LightLiquidGlass` | `#FFFFFFDE` (87% white) | `1.2–1.4 px` `#FFFFFFEE` / `#E0E7F0` | `backgroundBlur` + diffused `dropShadow` | Light floating nav, chat composers, glass headers, AI bottom sheet |
| `Aurel/Material/CrystalBlueGlass` | `#DCEBFFCC` (80% glacier blue) | `1.5 px` `#9BCBFF` | `backgroundBlur` | Active tab capsule, opt-in AI prompt chips, thread catch-up pills |
| `Aurel/Material/DarkLiquidGlass` | `#111B2CC8` / `#18263CCC` | `1.2 px` `#FFFFFF33`–`#FFFFFF38` | `backgroundBlur` | Dark Mode nav, Clips reaction rail, Story reply bar, Video Call deck |
| `Aurel/Material/PureReadingSurface` | `#FFFFFF` / `#080E1C` | `1.0 px` `#E0E7F0` / `#253550` | None | Chat streams, feed cards, settings, transcripts |

## 3. Concentric Optical Geometry

Every nested glass capsule satisfies $R_{\text{inner}} = R_{\text{outer}} - p$:

- Floating 5-tab bar: outer radius `32 px`, inner padding `8 px`, active selection pill radius `24 px`.
- Floating composer bar: outer radius `30 px`, inner padding `10 px`, circular `MIC` / `GO` button radius `20 px`.

## 4. FigCraft vs. Native iOS Implementation Disclosure

The glass refraction visible across the 54 exported PNGs uses FigCraft Desktop's native `backgroundBlur` and `dropShadow` renderer. Real-time hardware optical refraction (`SwiftUI` `.ultraThinMaterial` / `.regularMaterial` or Metal shaders) is specified for future Phase 02 iOS engineering and is not yet implemented in native Swift code.
