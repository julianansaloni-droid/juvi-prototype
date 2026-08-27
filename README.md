# JUVI — Fitness, your way

> Interactive prototype for a personalized fitness app with AI-powered training plans, trainer marketplace, and community features.

**Status:** v0.2 prototype · 15 interactive screens  
**Stack:** Vanilla HTML/CSS/JS (no build step, no dependencies)  
**Deploy:** GitHub Pages — push and enable Pages on `main`

## What this covers

### Onboarding (3 steps)
Goal selection with race picker sub-flow (Dublin Marathon, Half, 5K, custom) → experience & frequency sliders → day picker with "I'm flexible" toggle → personalized plan summary

### Dashboard
Dynamic greeting, 5-day streak badge, today's workout card with shimmer, weekly calendar strip, stats (distance + sessions), quick actions (find trainer, adjust plan, community), weekly progress bar chart

### Training
Full weekly plan view with week selector, day-by-day breakdown (completed/today/upcoming/rest), workout detail with exercise list, "Feeling tired?" intensity adjustment modal (−20% / planned / +15%), active workout screen with animated timer ring and pause/skip controls, workout complete screen with stats, pace splits, emoji feedback

### Trainers
Search bar, filter pills (Running, Strength, HYROX, Nutrition, Mobility), trainer cards with ratings, full trainer profile with bio, specialties, pricing, 3 reviews, "Message" chat screen with realistic conversation, "Book intro call" with toast confirmation

### Community
Weekly challenge banner with progress bar, social feed with activity cards (distance, time, pace), interactive like toggle with count animation, notification badge on tab

### Profile & Settings
Stats overview (workouts, km, adherence), horizontally scrollable achievement badges (earned + locked), recent workout history, connected devices screen (Apple Watch, Garmin, Strava, Apple Health with toggles), subscription screen (Free / Pro €9.99 / Pro+Coach €29.99), reset to re-run onboarding

### Design system

| Token | Hex | Role |
|-------|-----|------|
| Sol | `#D9A62E` | Primary — warm amber |
| Blaze | `#C44235` | Accent — warm red |
| Peach | `#E8935A` | Secondary — warm orange |
| Chalk | `#FAFAF7` | Background |
| Ink | `#1C1816` | Text |
| Glow | Sol → Blaze | Gradient on CTAs, progress, badges |
| Display | Space Grotesk | Headlines, numbers, labels |
| Body | DM Sans | Everything else |

### Interactions
- Animated gradient on welcome screen
- Staggered entrance animations on all lists
- Slide transitions for drill-in, cross-fade for tab switches
- Sliding gradient indicator on bottom nav
- Shimmer sweep on today's workout card
- Scroll-guard prevents accidental taps while scrolling
- Toast notifications on key actions
- Pulsing timer ring on active workout

## Deploy to GitHub Pages

```bash
gh repo create juvi-prototype --public
git init && git add .
git commit -m "v0.2 prototype"
git branch -M main
git remote add origin git@github.com:YOUR_USER/juvi-prototype.git
git push -u origin main
# Settings → Pages → Source: main → / (root) → Save
```

Live at `https://YOUR_USER.github.io/juvi-prototype/`

Don't forget the `.nojekyll` file (included) to bypass Jekyll processing.

## Product concept

**Monetization:** Freemium + trainer marketplace cut  
**Differentiator:** AI-first adaptive training where human trainers optionally plug in  
**Target:** Millennials & Gen Z in urban markets (starting Dublin)  
**Pricing model:** Free (basic) → Pro €9.99/mo (AI plans) → Pro+Coach €29.99/mo (includes trainer)

---

Built by Julian & Victor · 2026
