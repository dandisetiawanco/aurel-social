# AUREL Design System

**FigCraft Location**: Page 01 (Brand Identity) & Page 09 (Liquid Glass Design System)
**Reference Previews**:
- [`01-liquid-glass-materials-controls.png`](../previews/design-system/01-liquid-glass-materials-controls.png)
- [`02-domain-component-library.png`](../previews/design-system/02-domain-component-library.png)
- [`03-all-19-states-and-empty-states.png`](../previews/design-system/03-all-19-states-and-empty-states.png)

---

## 1. Verified Token & Component Inventory

Inspected directly from `design/AUREL-Social.figcraft` (`document.json`):

- **Variable Collections**: `2` (`AUREL Colors` with `Light` and `Dark` modes; `AUREL Scale` with `Default` mode)
- **Bound Variables**: `25` color, surface, border, spacing, and radius tokens
- **Native Reusable FigCraft Components**: `25` (`type: component`) spanning materials, buttons, inputs, switches, navigation, composers, feedback toasts, context menus, messaging bubbles, voice cards, AI cards, social posts, clip overlays, communities, and notifications
- **Documented Component States**: `19` explicit UI states + `5` empty states

## 2. Color System (Light & Dark Modes)

| Semantic Role | Light Value | Dark Value | Notes |
| :--- | :--- | :--- | :--- |
| Brand Signature | `#0866FF` | `#0866FF` | Primary CTAs, outgoing bubbles, active AI emblem |
| Interaction Accent | `#007AFF` | `#3B82F6` | Hover states, links, active dark rings |
| Deep Accent | `#0047C7` | `#0E234E` | Pressed state, splash depth, featured AI banner |
| Crystal / Glacier Tint | `#9BCBFF` / `#DCEBFF` | `#9BCBFF` / `#18263C` | Active nav capsule, subtle accents, dark borders |
| Primary Canvas | `#F7FAFF` / `#FFFFFF` | `#080E1C` | Screen background and clean reading surfaces |
| Elevated Card Surface | `#FFFFFF` / `#F2F5FA` | `#111B2C` | Containers, grouped lists, inactive pills |
| Border Hairline | `#E0E7F0` | `#253550` | Subtle 1 px container separation |
| Primary Text | `#101828` | `#F5F8FF` | High contrast (`16.4:1` light, `17.2:1` dark) |
| Secondary Text | `#52627A` | `#9FB0C9` | WCAG AA verified (`6.1:1` light, `7.9:1` dark) |
| Success / Consent | `#24B47E` (`#16865C` ink) | `#24B47E` (`#6EE7B7` ink) | Online presence, authorized AI scope banners |
| Warning / Offline | `#F59E0B` (`#A16207` ink) | `#F59E0B` | Offline banner, local draft indicator |
| Destructive / Error | `#EF4444` (`#B91C1C` ink) | `#EF4444` (`#FCA5A5` ink) | End call, failed message retry, reporting |

## 3. Typography & Spacing Scale

- **Display / Headings**: `Avenir Next` (`Demi Bold`, `Bold`), `22–38 px` mobile headings, `14–18 px` card titles.
- **UI Body & Chat**: `Helvetica Neue` (`Regular`, `Medium`, `Bold`), `13–15 px` body copy with `18–20 px` line height.
- **Technical Metadata & Timestamps**: `JetBrainsMonoNL Nerd Font` (`Regular`, `Bold`), `9–11 px` for timestamps, durations (`0:38`, `1.5x`), and scope tags.
- **4 pt / 8 pt Rhythm**: Mobile screen margins `16 px`–`24 px`, card padding `14 px`–`20 px`, section gaps `12 px`–`20 px`, primary touch heights `44 px`–`54 px`.

## 4. Complete 19-State Coverage

Board `DS 03` verifies every required state across four domains:

- **Core Controls (7)**: Default, Hover, Pressed (`0.97x`), Selected, Focused Ring (`3 px #0866FF`), Disabled, Loading.
- **Messaging & Voice (6)**: Sending, Delivered, Read, Failed (Retry), Recording Audio, Playing Voice Note.
- **Aurel Intelligence & System (6)**: Listening (Blue Orb), Thinking (Scoped Context), AI Responding (Streaming + Stop), Empty State, Offline Mode (Local Drafts), Error Recovery.
- **Empty States (5)**: Chats Empty, Saved Posts Empty, Communities Empty, Notifications Caught Up, New AI Thread Ready.
