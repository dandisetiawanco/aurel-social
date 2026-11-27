# AUREL Product Roadmap

This roadmap separates verified completed design work from planned future engineering phases.

---

## Phase 01: Product Design and Interactive Prototype (Completed)

- Brand identity system, Signature Blue & Liquid Glass palette, and `512 x 512` iOS App Icon.
- 36 Light Mode screens across Onboarding, Chats, Social, Clips, Aurel Intelligence, Spaces, and Personal Account.
- 8 Midnight Navy Dark Mode screens redesigned for nocturnal depth and smoked glass legibility.
- Liquid Glass Design System with 25 native reusable FigCraft Components, 25 variables across 2 collections, all 19 interactive/messaging/AI/system states, and 5 empty states.
- Motion specification board and 7 wired FigCraft interactive prototype flows (`25` transitions).
- 3 editorial Product Showcase boards, `1280 x 640 px` social preview, animated SVGs, and 16 technical specs.

---

## Phase 02: Mobile Application Foundation (Planned)

- Bootstrap Flutter / Dart mobile app workspace aligned with AUREL's 25 Light/Dark design tokens.
- Build native SwiftUI platform bridge for iOS translucent materials, haptics, and Dynamic Island spacing.
- Implement core 5-tab floating navigation capsule and offline local storage shell.

## Phase 03: Real-Time Messaging (Planned)

- Stand up Go WebSocket messaging gateway and FastAPI conversation services backed by PostgreSQL and Redis.
- Implement 1:1 chats, group rooms, delivery/read receipts, reactions, voice note uploads, and offline draft queuing.

## Phase 04: Social Networking (Planned)

- Implement photo feeds, 24-hour Stories, asymmetric Explore discovery, threaded comments, creator profiles, and audience controls.

## Phase 05: Short Video Infrastructure (Planned)

- Build FFmpeg 9:16 Clips transcoding pipeline, S3 object storage, CDN streaming, vertical swipe feed, and clip publishing with AI disclosure tags.

## Phase 06: Contextual AI Intelligence (Planned)

- Build multi-provider LLM gateway, `pgvector` semantic indexing strictly bounded by explicit user opt-in records, on-request Media Vision, and voice STT/TTS pipeline.

## Phase 07: Voice and Video Communication (Planned)

- Integrate WebRTC audio and HD video calling with Picture-in-Picture self-view and optional on-device live captions.

## Phase 08: Communities and Creator Tools (Planned)

- Deliver Aurel Spaces channels, pinned announcements, event RSVPs, and creator analytics.

## Phase 09: Security, Privacy, and Moderation (Planned)

- Complete passkey authentication hardening, security review, encryption design implementation, abuse reporting queues, and data export tooling.

## Phase 10: Production Deployment (Planned)

- Staged TestFlight rollout, observability dashboards, load testing, and App Store release preparation.
