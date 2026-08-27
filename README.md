# JUVI — Fitness, your way

Interactive prototype for a personalized fitness app with AI-powered training plans, trainer marketplace, and community features.

**Version:** v0.3 · 18 screens · 56 features  
**Stack:** Vanilla HTML/CSS/JS — no build step, no dependencies  
**Deploy:** GitHub Pages (include the `.nojekyll` file)

---

## Screens

### Onboarding (3 steps + plan summary)
Goal selection with race picker sub-flow (Dublin Marathon, Half, Parkrun 5K, custom) → experience level & frequency sliders → day picker with "I'm flexible" toggle → dynamic plan summary reflecting all choices, built by JUVI AI

### Dashboard
Time-aware greeting · 5-day streak badge · Dublin Marathon countdown (live) · weekly calendar strip with workout indicators · today's workout card with shimmer · distance + session stats · quick actions (trainers, adjust plan, community) · weekly progress bar chart with legend · coach tip card · travel schedule adjustment modal

### Training
Weekly plan with 8-week selector · day-by-day cards (completed/today/upcoming/rest) with difficulty tags · workout detail with 6-exercise list · "Feeling tired?" intensity modal (−20% / planned / +15%) · active workout with animated gradient timer ring, pause/skip/previous controls · workout complete with stats, pace splits, emoji feedback, share to community

### Trainers
Search bar with live filtering · category filter pills · 4 trainer cards with initial avatars, ratings, tags · full trainer profile with bio, specialties, pricing tiers, 3 reviews · "Message" opens chat screen with realistic conversation · "Book intro call" with toast confirmation

### Community
Feed/Challenges/My circle tabs · compose button · weekly challenge banner with progress · social feed with activity cards (distance, time, pace) · interactive SVG heart likes with count · comment and reaction icons

### Profile & Settings
Stats with SVG adherence ring · horizontally scrollable achievement badges (3 earned, 3 locked) · recent workout history with "See all" → full history screen with filters · goal progress screen with large progress ring, 5-phase milestone timeline, training totals · notifications screen (5 notifications, unread highlighting) · connected devices (Apple Watch, Garmin, Strava, Apple Health with toggles) · subscription plans (Free / Pro €9.99 / Pro+Coach €29.99) · reset to redo onboarding

---

## Design system

| Token | Value | Usage |
|-------|-------|-------|
| Sol | `#D9A62E` | Primary warm amber |
| Blaze | `#C44235` | Accent warm red |
| Peach | `#E8935A` | Secondary warm orange |
| Chalk | `#FAFAF7` | Background |
| Ink | `#1C1816` | Primary text |
| Glow | Sol → Blaze | Gradient — CTAs, progress, badges |
| Display | Space Grotesk | Headlines, numbers |
| Body | DM Sans | Body text |

98 SVG stroke icons · Initial-based avatars · No emoji in UI (except workout feedback mood selector)

## Interactions & polish

- Animated welcome gradient (3-color shift)
- Staggered entrance animations on lists
- Slide transitions for drill-in, cross-fade for tab switches
- Sliding gradient indicator on bottom nav
- Shimmer sweep on today's workout card
- Scroll guard prevents accidental taps while scrolling
- Toast notifications on all screens
- Pulsing timer ring on active workout
- Bottom sheet modals with backdrop blur
- Fullscreen toggle (top-right corner)
- PWA meta tags (theme-color, apple-mobile-web-app)
- All inputs have aria-labels
- Smooth scroll behavior

## Deploy

```bash
gh repo create juvi-prototype --public
git init && git add .
git commit -m "v0.3 — 18 screens, 56 features"
git branch -M main
git remote add origin git@github.com:YOUR_USER/juvi-prototype.git
git push -u origin main
# Settings → Pages → Source: main → / (root) → Save
```

Don't forget `.nojekyll` in the repo root.

Live at `https://YOUR_USER.github.io/juvi-prototype/`

## Product concept

**Model:** Freemium + trainer marketplace cut  
**Differentiator:** AI-first adaptive training where human trainers optionally plug in  
**Target:** Millennials & Gen Z in urban markets, starting Dublin  
**Pricing:** Free → Pro €9.99/mo → Pro+Coach €29.99/mo

---

Built by Julian & Victor · 2026
