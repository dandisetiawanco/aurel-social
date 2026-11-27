# AUREL Chats (Messaging Experience)

**FigCraft Location**: Page 03 (Aurel Chats) + Page 10 (`Dark 01`, `Dark 02`)
**Completed Screens**: 8 Light Mode screens (`05`–`12`) + 2 Midnight Navy Dark Mode screens

---

## 1. Screen Coverage

| Screen | File | Core Interaction Focus |
| :--- | :--- | :--- |
| **05 · Chats Home** | [`05-chats-home.png`](../previews/chats/05-chats-home.png) | Search bar, active notes strip, `All / Unread / Groups / Channels` filters, pinned threads, floating Liquid Glass bottom nav |
| **06 · Personal Conversation** | [`06-personal-conversation.png`](../previews/chats/06-personal-conversation.png) | High-contrast white canvas, embedded editorial photography, voice note player with transcript link, floating glass composer |
| **07 · AI-Assisted Conversation** | [`07-ai-assisted-conversation.png`](../previews/chats/07-ai-assisted-conversation.png) | Dimmed live chat underlay (`#0F172A40`) beneath a translucent Liquid Glass sheet offering Suggest, Rewrite, Translate, and Tone tools |
| **08 · Group Conversation** | [`08-group-conversation.png`](../previews/chats/08-group-conversation.png) | `NGOPREK Design Core` multi-participant thread, pinned decision banner, `@mentions`, shared desk attachment, opt-in catch-up chip |
| **09 · Voice Message Experience** | [`09-voice-message-experience.png`](../previews/chats/09-voice-message-experience.png) | Expanded 23-bar acoustic waveform, `1.5x` speed pill, `-10s/+10s` scrub controls, synced transcript card, optional AI takeaways |
| **10 · Audio Call** | [`10-audio-call.png`](../previews/chats/10-audio-call.png) | Deep blue atmospheric call stage, concentric voice pulse rings, on-device live caption preview concept, dark glass call deck |
| **11 · Video Call** | [`11-video-call.png`](../previews/chats/11-video-call.png) | Full-bleed portrait video feed, frosted caller status pill, top-right PiP self-view, floating 5-action dark glass control bar |
| **12 · Shared Media** | [`12-shared-media.png`](../previews/chats/12-shared-media.png) | Tabbed `Photos / Videos / Links / Files / Voice` archive with 3-column media grid and PDF/URL/WAV attachment cards |

## 2. Human-in-the-Loop AI Boundaries

Messaging assistance on Screen `07` (`Aurel Reply Assist`) enforces three UX guardrails:

1. **Per-message opt-in**: The sheet activates only when the user explicitly taps the `AI` action in the composer.
2. **Never auto-sends**: The primary button reads `Insert Draft to Composer`, placing text into the editable composer rather than transmitting directly.
3. **Structured utility over noise**: Alongside two reply tones, the sheet surfaces actionable extractions (such as confirming a rescheduled studio critique time).

## 3. Designed vs. Implemented Scope

All chat layouts, receipt states (`Sending`, `Delivered`, `Read`, `Failed`), voice waveforms, and WebRTC call screens are visual and interactive FigCraft designs. Live messaging transport, push notifications, and real-time voice/video media streams belong to future engineering Phases 03 and 07.
