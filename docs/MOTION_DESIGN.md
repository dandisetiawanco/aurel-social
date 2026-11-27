# Motion Design Specification

**FigCraft Location**: Page 11 (Motion & Interactive Prototype)
**Reference Preview**: [`01-motion-and-prototype-architecture.png`](../previews/motion/01-motion-and-prototype-architecture.png)

---

## 1. Five-Tier Spring & Timing Grammar

AUREL motion emphasizes physical clarity and fast responsiveness rather than decorative bounce:

| Tier | Duration | Motion Curve / Physics | Product Interactions |
| :--- | :--- | :--- | :--- |
| **01 · Micro-Interactions** | `120 - 180 ms` | `Spring(response: 0.22, bounce: 0.15)` | Tactile button press (`0.97x`), reaction pill pop, toggle switches, delivery/read receipt ticks |
| **02 · Glass Pill Selection** | `180 - 220 ms` | Matched geometry slide | Floating 5-tab capsule highlight glide, segment switcher morph, filter chip selection |
| **03 · Liquid Glass Sheets** | `250 - 350 ms` | `easeOut` / damped spring + blur ramp | AI Reply Assist sheet (`07`), Clips Comments drawer (`21`), Voice Note player expansion (`09`) |
| **04 · Screen Push / Pop** | `280 - 400 ms` | Interactive iOS push with `20%` parallax | Chats list to conversation, Spaces to Channel, Profile to Settings, edge-swipe back |
| **05 · Immersive Media & Orb** | `350 - 500 ms` | Gentle spring expansion | Story avatar zoom into 9:16 canvas, vertical Clip snap, Video Call PiP snap, Aurel Voice orb breathing pulse |

## 2. Reduce Motion Accessibility Fallback

When iOS `Reduce Motion` (or `prefers-reduced-motion: reduce` on the web) is active:

- All spring scale transforms, horizontal slide pushes, and orbital rotations degrade cleanly to a `180 ms` opacity cross-dissolve.
- Animated SVGs in this repository include static fallbacks wrapped in `<picture>` elements respecting `prefers-reduced-motion: reduce`.

## 3. Conceptual Animations vs. Prototype Scope

The animated SVGs in [`assets/animations/`](../assets/animations/) demonstrate proposed motion intent for brand pathways, Liquid Glass tab gliding, message delivery states, and Aurel Intelligence voice states. Continuous gesture velocity and live FFT voice waveforms are specified for native SwiftUI / Flutter implementation.
