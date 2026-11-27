# Interactive Prototype Guide

**Source File**: [`design/AUREL-Social.figcraft`](../design/AUREL-Social.figcraft)
**Verified Wiring**: `7` interactive flow starting points and `25` wired `proto.interaction.add` screen transitions

---

## 1. How to Navigate the Prototype in FigCraft Desktop

1. Open `design/AUREL-Social.figcraft` in **FigCraft Desktop**.
2. Switch to any core experience page (`02`–`08`) or review the complete map on **Page 11 (Motion & Interactive Prototype)**.
3. Press **`Shift + Space`** (live prototype preview pane) or **`Alt + Cmd + Enter`** (Present mode) to click through wired screens with hotspot hints enabled.

## 2. Complete Wired Prototype Flow Map

| Flow | Starting Screen | Wired Screen Sequence & Transitions |
| :--- | :--- | :--- |
| **Flow 01 · Onboarding** | `01 Splash` (`Page 02`) | `01 Splash` *(dissolve 350ms)* -> `02 Welcome` *(push left 320ms)* -> `03 Sign In` *(push left 320ms)* -> `04 Create Profile` |
| **Flow 02 · Aurel Chats** | `05 Chats Home` (`Page 03`) | `05 Chats` *(push left)* -> `06 Personal Convo` *(moveIn bottom 300ms)* -> `07 AI Reply Sheet` *(smartAnimate 280ms)* -> `09 Voice Note` *(dissolve)* -> `11 Video Call` *(push left)* -> `12 Shared Media` |
| **Flow 03 · Aurel Social** | `13 Social Home` (`Page 04`) | `13 Social` *(smartAnimate 380ms)* -> `14 Story Viewer` *(push left)* -> `16 Post Comments` *(dissolve)* -> `17 Explore` *(push left)* -> `19 Creator Profile` |
| **Flow 04 · Aurel Clips** | `20 Clips Feed` (`Page 05`) | `20 Clips Feed` *(moveIn bottom 280ms)* -> `21 Video Comments` *(dissolve)* -> `22 Discovery` *(moveIn bottom)* -> `23 Create Clip` *(push left)* -> `24 Clip Publishing` |
| **Flow 05 · Intelligence** | `25 AI Home` (`Page 06`) | `25 AI Home` branches to `26 AI Conversation` *(push left)*, `27 AI Voice Orb` *(smartAnimate 380ms)*, `28 AI Media Vision` *(push left)*, and `29 Personal Digest` *(push left)* |
| **Flow 06 · Spaces** | `30 Spaces Home` (`Page 07`) | `30 Spaces Home` *(push left)* -> `31 Kyoto Architecture Space` *(push left)* -> `32 #photography Channel` |
| **Flow 07 · Account** | `33 Personal Profile` (`Page 08`) | `33 Profile` *(push left)* -> `35 Settings & Privacy` *(dissolve)* -> `34 Notifications` *(dissolve)* -> `36 Universal Search` |

## 3. Exported Sequence Preview

The file [`assets/animations/aurel-prototype-walkthrough.gif`](../assets/animations/aurel-prototype-walkthrough.gif) is compiled directly from exported FigCraft screens to illustrate screen-to-screen flow inside GitHub Markdown without claiming to be a live compiled iOS runtime capture.
