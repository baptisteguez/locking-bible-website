# CLAUDE.md — Lumi Bible website (lockingbible.com)

Marketing, support and legal site for the **Lumi Bible** iOS app (formerly
Locking Bible). The domain stays lockingbible.com. Contact: contact@lockingbible.com.
The iOS app (branch `v2` of the parent repo) is the source of truth for design
and for every claim made here.

## What Lumi Bible is (2.0)

A calm feed of Scripture: swipe through Bible verses, Words of Jesus and
"Did you know?" facts; like, save, share as an image. The complete Bible offline
(KJV, Louis Segond 1910, Reina-Valera 1909, Bíblia Livre). Home Screen and Lock
Screen widgets (Bible Verse, Verse of the Day, My Streak). Streaks, 8 badge
levels (Beginner → Theologian), reminders (1/3/5 a day), 24 backgrounds,
10 app icons. Mascot: **Lumi**, a little lantern. Languages: EN, FR, ES, pt-BR.

It is NOT an app blocker anymore: the Screen Time feature was removed in 2.0.
Never mention blocking apps except to explain the removal (support page).
No AI, no account, no social features.

Free: full Bible, 15 new feed verses/day, all widgets, streaks/badges, the
onboarding background and icon. Premium: unlimited verses, Words of Jesus,
Did you know?, all backgrounds (+ brightness) and icons. Never print prices:
they vary by country and come from StoreKit.

## Design (mirrors Shared/Core/Theme.swift)

| Token | Hex | Role |
|---|---|---|
| cream | `#FBF7EF` | page background |
| cream-deep | `#F4ECDD` | alternate bands |
| card | `#FFFDF8` | cards |
| ink | `#3A2E22` | text |
| ink-soft | `#8A7A68` | secondary text, eyebrows |
| line | `#E8DCC8` | borders |
| brown | `#8C5D2B` | primary buttons, accent phrase |
| gold / amber | `#D9A23E` / `#E59A3C` | quote marks, small details |
| glow | `#F8E3B4` | radial golden halo |

- Serif (Lora on the web, New York in the app) for headlines and verses;
  system sans for UI. One italic brown accent phrase per headline.
- Eyebrows: serif, uppercase, tracked ~0.22em, ink-soft.
- Primary button: brown fill, white text, 58px high, 22px radius.
- Golden radial glow behind key visuals (`.glow`), like the app's GlowBackground.
- Real app screenshots in phone frames; Lumi illustrations from the app assets.
- Calm motion only (fade-up on scroll, Lumi float), respect reduced motion.

## Rules

- Never fabricate: no reviews, ratings, user counts or statistics.
- Every feature claim must exist in the app. Keep privacy/terms consistent with
  the app (Amplitude analytics, PrivacyInfo.xcprivacy) and App Store Connect.
- Credit Bíblia Livre (CC BY 4.0) wherever Bible translations are listed.

## Structure

`index.html`, `support/`, `privacy/`, `terms/`, `404.html`, shared
`assets/site.css` + `assets/site.js`, images in `assets/`. Netlify publishes
only `deploy/` (see `netlify.toml`): add any new top-level file to its build
command.
