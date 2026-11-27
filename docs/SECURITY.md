# Proposed Security Architecture

> **Status Notice**: This document outlines the **proposed security architecture** for future AUREL engineering phases. No cryptographic protocols, authentication servers, compliance audits, or certifications exist in this design repository.

---

## 1. Authentication & Session Design (Proposed)

- **Passwordless-First Onboarding (`Screen 03`)**: Proposed support for WebAuthn / Apple Device Passkeys, Sign in with Apple, and time-limited one-time verification codes.
- **Session Hygiene**: Short-lived access tokens paired with rotating refresh tokens stored in the iOS Keychain, device session management, and instant remote revocation.

## 2. Authorization & Scope Boundaries (Proposed)

- **Role & Audience Checks**: Every feed query, Story view, Space channel fetch, and media URL respects explicit audience scoping (`Public`, `Followers`, `Close Circle`, `Space Members`).
- **AI Context Guard**: Before passing any content to the proposed multi-provider LLM gateway, a server-side policy check verifies that the requesting user explicitly opted in for that exact Space, saved item, or per-message tap. Private 1:1 threads remain inaccessible to background indexing jobs.

## 3. Transport & Data Protection Plan (Proposed)

- **In Transit**: TLS 1.3 enforced across REST APIs, WebSocket gateways, and media CDN endpoints; DTLS-SRTP for WebRTC voice and video calls.
- **At Rest & Future E2EE Evaluation**: Database encryption at rest for user records and S3 media buckets, with an explicit future engineering milestone in Phase 09 to evaluate end-to-end encryption (E2EE) key management for direct chats versus optional cloud-synced multi-device threads.

## 4. Safety, Blocking & Moderation Controls (`Screen 35`)

Designed UX flows cover:
- Per-account blocking and muted word lists (`Blocked Accounts & Muted Words`).
- Context-menu reporting on messages, comments, posts, and Clips (`Aurel/Overlay/GlassContextMenu`).
- User data export and account deletion controls (`Safety Reporting & Export My Data`).
