# Design Engineering Workflow

AUREL was conceived, designed, audited, and packaged through a transparent, AI-assisted design engineering workflow directed by **Dandi Setiawan / NGOPREK DIGITAL**.

---

## 1. Tooling Stack & Exact Responsibilities

| Tool / Methodology | Role in AUREL Production |
| :--- | :--- |
| **Google Antigravity** | Agentic orchestration environment coordinating planning, visual media generation, live MCP tool calls, visual export auditing, and repository packaging |
| **FigCraft Desktop (Live Mode)** | Primary native canvas (`127.0.0.1:7979`) rendering all 12 pages, 2,168 nodes, native `backgroundBlur` glass materials, 25 reusable Components, 25 variables, and 7 interactive prototype flows |
| **FigCraft MCP** | Direct live streaming bridge (`FIGCRAFT_AUTO_LAUNCH=1`, `FIGCRAFT_STREAM_STEPS=1`) executing batched canvas updates with automatic viewport framing rather than headless scripts or static HTML mockups |
| **Astryx Design Principles** | Design system foundation guiding `44 pt+` touch targets, WCAG AA contrast verification, optical corner nesting, and complete 19-state + empty-state matrices |
| **Anti-Slop (Mode 1: During)** | Continuous creative quality filter rejecting generic purple AI styling, decorative badge clutter, blurred dense reading surfaces, em-dash copywriting tells, and fabricated technical claims |
| **Editorial Media Generation** | Generated 5 cohesive architectural, coastal, Tokyo night-cinema, studio portrait, and desk flatlay photographs placed natively via `image.place` |

## 2. Iterative Visual Audit Process

Every page was exported at `2x` directly from FigCraft Desktop and visually inspected during production rather than assumed complete. Visual audits caught and resolved:

- Headline line-wrap overlap and floating nav active-pill offset on Screen `25` (`AI Assistant Home`).
- Button label alignment inside `Dismiss` on Screen `07` (`AI-Assisted Conversation`).
- Two-line caption vertical centering inside the glass sticker on Screen `14` (`Story Viewer`).
- Typography and copy hygiene checks across chat bubbles and showcase credits.

## 3. Repository Asset Pipeline

1. Preserved the canonical editable document at `design/AUREL-Social.figcraft` (`12 MB`, verified zero local filesystem paths and zero secrets).
2. Optimized all 54 exported PNG previews with `ffmpeg` (`lanczos` scaling + zlib level 9) from `48 MB` down to `28.2 MB` while retaining `1.5x` mobile retina sharpness and exact `1280 x 640 px` dimensions for `assets/github/social-preview.png`.
3. Authored 5 custom animated SVGs, 2 architecture diagrams, and an exported screen-flow walkthrough GIF with `prefers-reduced-motion` static fallbacks.
