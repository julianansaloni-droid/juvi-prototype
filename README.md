# JUVI — Fitness, your way

Interactive dark-mode prototype for a personalized fitness app with AI-powered training plans, trainer marketplace, and community features. Built for millennials and Gen Z.

**Version:** v0.4 · 18 screens · 56+ features · Dark mode  
**Stack:** Vanilla HTML/CSS/JS — no build step, no dependencies  
**Deploy:** GitHub Pages (include `.nojekyll`)

---

## Design philosophy

Grounded in 2026 UX research on what actually works for the target demographic:

- **Dark mode default** — 82% of smartphone users prefer dark mode (EarthWeb 2024), 73% of Gen Z specifically (Adobe 2025). Dark backgrounds make warm accents pop, reduce eye strain for evening use, and save OLED battery. The Sol/Blaze warm palette becomes more distinctive against the dark canvas, not less.
- **Bold, expressive typography** — 2026 fitness design leads with oversized type (84px wordmark, 28px dashboard greeting). Words should vibrate with energy before any image loads.
- **Anti-shame gamification** — weekly quests and rest day rewards, not punitive streak pressure. Research shows gamification increases adherence by 27%, but "streak stress" causes overtraining. JUVI rewards recovery as much as activity.
- **AI-first personalization** — dynamic nudges based on training data ("your pace improved 12 sec/km"), not static tips. Content slots change based on user state.

## Screens (18)

### Onboarding
Goal selection with race picker (Dublin Marathon, Half, Parkrun 5K, custom) → experience & frequency sliders → day picker with "I'm flexible" toggle → AI-generated plan summary reflecting all choices

### Dashboard
Time-aware greeting · streak badge · live marathon countdown · week strip · today's workout hero card with shimmer · stats · **weekly quest** with progress bar · quick actions · weekly bar chart · **AI insight** card · travel schedule adjustment modal

### Training
8-week plan with selector · day cards with **rest day rewards** (recovery messaging, not blank) · workout detail with exercises · intensity modal (−20%/planned/+15%) · active workout with gradient timer ring · workout complete with stats + emoji feedback

### Trainers
Search with live filter · category pills · 4 trainer profiles with initial avatars · reviews · pricing · chat · booking

### Community
Feed/Challenges/My circle tabs · compose button · challenge progress · social feed with SVG heart likes

### Profile
Adherence ring · achievement badges · workout history with "See all" → full history screen · **goal progress** with milestone timeline · notifications (5) · connected devices with toggles · subscription (Free/Pro/Pro+Coach) · reset

## Design system

| Token | Value | Role |
|-------|-------|------|
| Chalk | `#0E0E14` | Dark background |
| White | `#1C1C26` | Card surface |
| Paper | `#181822` | Elevated surface |
| Ink | `#F0EDE8` | Primary text (warm off-white) |
| Sol | `#D9A62E` | Primary accent — warm amber |
| Blaze | `#C44235` | Secondary accent — warm red |
| Peach | `#E8935A` | Tertiary — warm orange |
| Glow | Sol → Blaze | Gradient — CTAs, progress, badges |
| Display | Space Grotesk | Headlines, numbers |
| Body | DM Sans | Body text |

98 SVG stroke icons · Initial-based avatars · PWA meta tags · Full accessibility labels

## Deploy

```bash
gh repo create juvi-prototype --public
git init && git add .
git commit -m "v0.4 — dark mode, 18 screens"
git branch -M main
git remote add origin git@github.com:YOUR_USER/juvi-prototype.git
git push -u origin main
```

Settings → Pages → Source: main → / (root) → Save  
Include `.nojekyll` in repo root.

## Product

**Model:** Freemium + trainer marketplace cut  
**Differentiator:** AI-first adaptive training where human trainers optionally plug in  
**Target:** Millennials & Gen Z, urban markets, starting Dublin  
**Pricing:** Free → Pro €9.99/mo → Pro+Coach €29.99/mo

---

Built by Julian & Victor · 2026
