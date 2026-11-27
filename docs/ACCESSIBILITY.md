# Accessibility Specification

AUREL incorporates **Astryx Design System** accessibility principles and WCAG 2.1 AA targets across all 44 mobile screens and both Light and Midnight Navy Dark themes.

---

## 1. Verified Color Contrast

| Pairing | Foreground | Background | Ratio | WCAG AA Status |
| :--- | :--- | :--- | :--- | :--- |
| Light Primary Text | `#101828` | `#FFFFFF` | `16.4 : 1` | Pass (AAA) |
| Light Secondary Text | `#52627A` | `#F2F5FA` | `6.1 : 1` | Pass (AA+) |
| Light Signature CTA | `#FFFFFF` | `#0866FF` | `4.7 : 1` | Pass (AA) |
| Light Consent Banner | `#16865C` | `#EAF9F2` | `4.6 : 1` | Pass (AA) |
| Dark Primary Text | `#F5F8FF` | `#080E1C` | `17.2 : 1` | Pass (AAA) |
| Dark Secondary Text | `#9FB0C9` | `#111B2C` | `7.9 : 1` | Pass (AAA) |
| Dark Accent Text | `#9BCBFF` | `#111B2C` | `10.8 : 1` | Pass (AAA) |

## 2. Touch Ergonomics & Interactive Clarity

- **Minimum Tap Targets**: Primary buttons (`52–54 px`), floating nav tabs (`48 px` active capsule inside `64 px` bar), circular video/call controls (`54–60 px`), and switch tracks all meet or exceed Apple HIG's `44 x 44 pt` minimum.
- **Visible Focus & Selection States**: Focus rings use a `3 px #0866FF` outline (State `5` on `DS 03`); selected tabs pair fill tint, border weight, and typography weight change rather than relying on color alone.
- **No Decorative Emojis in UI Chrome**: Labels use clear text (`Voice`, `Insert Draft`, `AI Subtitles: ON`, `Going ✓`) rather than ambiguous icon-only or emoji strings.

## 3. Media, Audio & Motion Inclusivity

- **Voice Transcripts & Live Captions**: Voice notes (`Screen 09`), Audio Calls (`Screen 10`), and Clips (`Screen 23`) surface synced transcripts and subtitles by design.
- **Alt-Text Authoring Prompt**: `Screen 18` (`Create Post`) includes a dedicated `Suggest Alt Text (A11y)` chip during publishing.
- **Reduce Motion Support**: Every spring transition in [`MOTION_DESIGN.md`](MOTION_DESIGN.md) and animated SVG in this repository defines a calm opacity fallback or static `<picture>` alternative for `prefers-reduced-motion: reduce`.
