# JUVI — Fitness, your way

> Interactive prototype for a personalized fitness app with AI-powered training plans, trainer matching, and community features.

**Status:** v0.1 prototype · Clickable mockup  
**Stack:** Vanilla HTML/CSS/JS (no build step)  
**Deploy:** GitHub Pages — just push and enable Pages on `main`

## What this shows

Five complete flows navigable via bottom tab bar:

1. **Onboarding** — 3-step goal-setting flow (goal → experience → schedule)
2. **Dashboard** — Today's workout, weekly strip, stats, quick actions
3. **Training** — Workout detail with exercise list and intensity adjustment
4. **Trainers** — Discovery grid with filters, individual trainer profiles with pricing
5. **Community** — Weekly challenges and social activity feed

## Design system

| Token | Value | Usage |
|-------|-------|-------|
| Sol | `#D9A62E` | Primary (warm amber) |
| Blaze | `#C44235` | Accent (warm red) |
| Chalk | `#FAFAF7` | Background |
| Ink | `#1C1816` | Text |
| Gradient | Sol → Blaze | CTAs, progress, avatar rings |
| Display | Space Grotesk | Headlines, numbers |
| Body | DM Sans | Everything else |

## Deploy to GitHub Pages

```bash
# 1. Create repo
gh repo create juvi-prototype --public

# 2. Push
git init
git add .
git commit -m "v0.1 prototype"
git branch -M main
git remote add origin git@github.com:YOUR_USER/juvi-prototype.git
git push -u origin main

# 3. Enable Pages
# Settings → Pages → Source: Deploy from branch → main → / (root) → Save
```

Your prototype will be live at `https://YOUR_USER.github.io/juvi-prototype/`

## Product concept

**Monetization:** Freemium + trainer marketplace cut  
**Differentiator:** AI-first adaptive training engine where human trainers can optionally plug in — bridging the gap between expensive walled-garden coaching ($200/mo) and generic AI-only plans  
**Target:** Millennials and Gen Z fitness-conscious users in urban markets (starting Dublin)

## Next steps

- [ ] Name decision (JUVI is working title)
- [ ] Pick the wedge feature for v1 (onboarding → plan, trainer matching, or tracking)
- [ ] Design: avatar/photo system, actual illustrations, motion design
- [ ] Tech: decide React Native vs PWA vs Flutter for production
- [ ] Backend: auth, user profiles, training plan engine
- [ ] Trainer marketplace: onboarding flow for trainers, payment integration

---

Built by Julian & Victor · 2026
