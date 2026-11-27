# Privacy & Consent Architecture (Design Concept)

**Primary Reference Screens**:
- [`04-create-profile.png`](../previews/onboarding/04-create-profile.png)
- [`07-ai-assisted-conversation.png`](../previews/chats/07-ai-assisted-conversation.png)
- [`29-ai-personal-digest.png`](../previews/intelligence/29-ai-personal-digest.png)
- [`35-settings-privacy.png`](../previews/profile/35-settings-privacy.png)

> **Transparency Notice**: All privacy switches, consent banners, and disclosure badges in AUREL are product UX designs and proposed policy specifications. No production data pipeline or enforcement backend is implemented in this design repository.

---

## 1. Core Consent Principles Designed Into the UI

1. **Opt-In by Default at Onboarding (`Screen 04`)**: During account setup, `Aurel AI Opt-In Summaries` defaults to **OFF** (`Off by default · Choose spaces individually`).
2. **Private Direct Messages Excluded (`Screens 29 & 35`)**: In Settings & Privacy (`35`), `Exclude Private Direct Chats` is prominently locked **ON** (`Protected · AI only runs when explicitly tapped`). The Personal Digest (`29`) confirms this with a green banner: `Authorized Sources: 2 Spaces, Saved Posts · Private DMs Excluded`.
3. **Human Confirmation Before Sending (`Screen 07`)**: `Aurel Reply Assist` explicitly states `OPT-IN FOR THIS MESSAGE ONLY · NEVER AUTO-SENDS` and inserts drafts into the editable composer rather than transmitting automatically.
4. **On-Request Media Analysis (`Screen 28`)**: AI Media Vision notes `Image analyzed on request only. Never stored in training sets` as the proposed product policy for future implementation.
5. **AI-Assisted Content Disclosure (`Screens 18, 24 & 35`)**: Publishing posts or Clips surfaces a transparent `AI-Assisted Label Disclosure` switch so audiences know when subtitles or caption edits used AI tools.
6. **Notification Privacy (`Screen 35`)**: Supports `Hide Previews` and `Quiet Hours` controls so lock-screen alerts do not leak message contents.
