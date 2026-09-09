# CLAUDE.md — Locking Bible Website

This file defines the design direction (DA) and brand rules for the Locking Bible
marketing website. It is derived from the approved iOS app design system, which is
the visual source of truth. Do not reinterpret or "modernize" it.

## What Locking Bible is

A behavior-change iOS app: it pauses the distracting apps you choose (via Apple
Screen Time) and gives you a short moment with Scripture before you can scroll.

Core loop: Distracting app → Locking Bible shield → Scripture → Reflection →
Prayer → choose unlock duration (1/15/30 min) → apps unlock → automatic re-protection.

Positioning: **Less scrolling. More Scripture.**
Supporting idea: *Scripture before scrolling.*

It is NOT: an AI Bible, a chatbot, a full Bible reader, a social network, or a
theological authority. Never imply those.

## Brand feeling

Sacred calm. Modern restraint. Editorial, premium, warm, minimal, intentional.
Think high-end print editorial meets quiet spiritual product — never SaaS,
never techy, never gamified, never childish.

The name is always **Locking Bible** (never "LockingBible" in copy, never
"Looking Bible", never "Bible Mode").

## Color palette (exact values — do not deviate)

| Token | Hex | Role |
|---|---|---|
| Ivory | `#FAF7F0` | Page background — the environment |
| Warm Ivory | `#FFF3D8` | Atmospheric radial warmth (top-left glow) |
| Surface | `#FFFDF9` | Cards / raised surfaces |
| Ink | `#171411` | Primary text, dark surfaces (shield mock) |
| Soft Ink | `#5B554E` | Secondary/body text |
| Muted Ink | `#999189` | Captions, eyebrows, tertiary text |
| Gold | `#F1C45A` | PRIMARY ACTION ONLY (CTAs, key accents) |
| Deep Gold | `#D6A43A` | Gold hover/pressed, small gold details |
| Soft Gold | `#F9E8B3` | Selected states, gold tints, badges |
| Coral | `#E5685B` | EMPHASIS ONLY (one accent phrase per headline, key stats) |
| Soft Coral | `#F7D9D4` | Subtle coral tint (rare) |
| Moss | `#6F8A72` | Protection / active / success semantics |
| Soft Moss | `#DEE7DE` | Moss tint pills ("Paused until Scripture") |
| Hairline | `#EAE3D9` | 1px borders, dividers |

Semantic law: **Ivory = environment · Gold = action · Coral = emphasis ·
Moss = protection/success · Ink = content.** Never swap these roles.

## Background treatment

Never flat white. The canvas is Ivory with a soft atmosphere:
- radial warm-ivory glow from the top-left (center ~16%/4%, large radius, fades out)
- faint soft-coral radial from bottom-right (~10% opacity)
- whisper of soft-gold in a top-to-bottom linear gradient (~3% opacity)
No heavy gradients, no glassmorphism, no noise textures, no dark mode.

## Typography

Two voices only:
- **Serif = meaning / Scripture / emotion.** Headlines, verses, stats, titles.
  App uses the system serif (New York); on the web use a close editorial serif
  (e.g. "New York"-like: Source Serif 4, or similar warm transitional serif).
  Regular-to-medium weight, tight tracking on display sizes (−0.5 to −1 px),
  generous line-height on verses.
- **Sans-serif = product / controls / function.** Buttons, labels, nav, body UI
  copy. System sans (SF-like: Inter or system-ui stack). 14–17px body.

Signature elements:
- **Eyebrow labels**: 10–11px sans, semibold, uppercase, letter-spacing ~0.2em,
  Muted Ink. Used above every headline (e.g. `HOW IT WORKS`, `TODAY'S SCRIPTURE`).
- **Accented headline phrase**: one phrase per big serif headline set in Coral
  (e.g. "Less scrolling. **More Scripture.**" — coral on the second sentence).
- Scripture is always set in serif, quoted with real curly quotes “…”, with the
  reference (e.g. `Psalm 46:10`) in small semibold coral.

## Components

- **Primary button**: Gold fill `#F1C45A`, Ink text, semibold ~16px, height ~54px,
  radius ~16px (continuous/squircle feel), optional small arrow icon. Press/hover:
  scale 0.985 + slight opacity, 150ms ease-out. ONE primary action per section.
- **Cards**: Surface at ~92% opacity, radius 24–28px, 1px Hairline border at
  ~85% opacity, padding ~20–24px. No drop shadows heavier than a whisper.
- **Option rows / pills**: Surface bg, 14px radius, gold-soft tint + gold border
  when selected, small gold check circle.
- **Status pill**: capsule, Soft Moss bg, 7px Moss dot + semibold ink text
  ("Paused until Scripture", "Protection active").
- **Duration pills**: capsules `1 MIN / 15 MIN / 30 MIN`, soft-gold fill + gold
  border when selected.
- **Stats strip**: serif numbers (~22px) over 11px muted labels, hairline
  vertical dividers ("6 / day streak · 42 min / reclaimed · 12 / verses").

## The logo / mark

An ink rounded-square book cover with: thin soft-gold inset frame, an ivory
cross (two rounded capsules), and a gold clasp/lock on the right edge that can
animate open. Wordmark: "LOCKING" in tiny tracked-out sans over "Bible" in
serif. Never replace with a generic book or lock icon.

## The shield (key product visual to showcase)

The real in-product shield is deliberately dark: warm Ink background, the mark,
serif ivory title **"Scripture before scrolling."**, warm-ivory subtitle
"Take a short moment with God's Word before opening this app.", and a gold
capsule button **"Open Locking Bible"**. Reproduce it faithfully in phone mockups
— it's the hero demo of the product.

## Motion

Restrained and calm: short fades (~240ms ease-in-out), soft springs on
selection, small gold sparkle bursts for success moments (6–10 tiny gold dots
radiating + fading, ~600ms). The book clasp animating open is the signature
success motion. NO confetti, no bounce, no parallax circus, no scroll-jacking.
Respect `prefers-reduced-motion`.

## Copy voice

Calm, warm, honest, short. One idea per section. Sentence case headlines with
periods ("Pause before you scroll."). No hype, no guilt, no streak-shaming.
Never fabricate: no fake testimonials, review counts, user numbers, or
statistics. The only numbers allowed are honest ones (e.g. 3–4h/day ≈ 1,278
hours/year ≈ 53 days; 10 min/day ≈ 61 hours of Scripture/year).

Reference copy bank: "Less scrolling. More Scripture." · "Scripture before
scrolling." · "Create a quiet pause before the scroll begins." · "Choose the
apps you want to protect." · "When the scroll can wait, Scripture comes first."
· "Then choose when to return." · "You stay in control of your attention." ·
"Less noise. More Scripture." · "Build a rhythm that lasts."

Real features only: protect chosen apps · Scripture → Reflection → Prayer pause
· 1/15/30 min unlock durations · automatic re-protection · simple streak ·
time reclaimed. Pricing: Weekly $4.99/week · 3-Day Free Trial then $39.99/year.

## Hard don'ts

No dark mode. No neon, purple/blue SaaS gradients, or glassmorphism. No generic
Tailwind-template look. No stock photos of people praying. No competitor
branding/assets. No AI claims. No tab-bar-style nav metaphors. No more than one
gold CTA competing per viewport. Wide layouts stay airy: generous whitespace is
part of the brand — when in doubt, remove elements rather than add.

