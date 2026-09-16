# TriQuil

*Ideas Today. A Calmer Tomorrow.*

TriQuil is a wearable relaxation device from Auvara Wellness Inc., a Canadian wearable-technology company. It targets three inner-wrist points known as the "TriQuil Triangle" (P6, LU9, H7) using three independently controlled vibration actuators to deliver spatial, multi-point relaxation patterns called Rhythms.

## Overview

- **Core device:** Haptic-only wearable with three independently addressable actuators (P6, LU9, H7), enabling directional, sweeping, and rotating Rhythms that no direct competitor currently offers.
- **Sessions:** Scheduled, brief (typically 15–20 minutes), designed for everyday relaxation, focus, sleep prep, and recovery.
- **AI layer:** Session recommender, conversational coach, plain-language explainer, and a constrained Rhythm generator — all validated against a deterministic safety check (actuator mapping, 40-step limit, timing, amplitude/duration ranges, 20-minute cap) before any AI-generated content reaches the device.
- **Business model:** A genuinely usable free tier, with subscription value built around expanded Rhythm variety and deeper AI coaching — not gating core function behind a paywall.
- **PulseCore:** A second, premium product line bringing the same three-point concept to electrical stimulation, currently in development pending a validated, comfortable skin-contact solution.

## Positioning

TriQuil competes across haptic wellness wearables, electrical-stimulation wearables, point-stimulation devices, and software-only wellness apps. It differentiates through:

- Three-point spatial patterning (vs. single/dual-point competitors)
- A dual-credibility brand story: Traditional Chinese Medicine acupoint science plus modern vibration science
- A free tier that stays functional without a forced membership
- A youth/young-adult beachhead underserved by existing players, supported by parental-consent flows

Planned launch price: **US$399**. Initial focus: Canada/US, direct-to-consumer.

## Important Notes

- TriQuil is a **general wellness product, not a medical device**. It does not diagnose or treat disease and does not measure physiological readings.
- All AI-generated coaching and content is wellness-framed, never diagnostic, and is bounded by firmware-enforced safety limits.
- Electrical safety and biocompatibility testing for PulseCore are deferred to formal product validation.

## Repository Structure

This repo is a Next.js application:

```
app/
  page.tsx                # Main customer-facing app
  customer-parity.tsx     # Additional customer-facing screens
  admin/                  # Admin portal
  api/ai/                 # AI endpoints (coach, pattern generation, recommendations)
lib/
  ai/                     # AI provider integrations (Ollama, OpenRouter)
  demo-data.ts            # Demo sessions and device data
public/                   # Static assets
```

## Getting Started

Install dependencies and run the development server:

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the app. The admin portal is available at `/admin`.

## Attribution

This project was developed as a submission to the **WIMTACH Hackathon 2026**, covering the Business Strategy, Electronic Device Design, and AI App Integration tracks.
