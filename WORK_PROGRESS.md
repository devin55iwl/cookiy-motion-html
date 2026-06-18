# Cookiy Motion HTML - Work Progress

Last updated: 2026-06-18

## Project Purpose

This repository hosts Devin Wang's Cookiy AI portfolio case study for GitHub Pages:

https://devin55iwl.github.io/cookiy-motion-html/

The page is a static, single-file portfolio site. It presents Cookiy AI as an AI-native research SaaS case study, with the core narrative:

> I designed a trust system for AI-moderated research.

The target reader is a hiring manager, recruiter, or interviewer for AI Product Designer, AI Product Experience Designer, Design Engineer, or AI Product Manager adjacent roles.

## Repository Shape

- Main page: `index.html`
- Static assets: `assets/`
- Deployment target: GitHub Pages from this repository
- No build step is required
- Local preview command:

```bash
python3 -m http.server 8765
```

Then open:

```text
http://127.0.0.1:8765/
```

## Current Page Structure

The current case study is organized as:

1. Cookiy case-study hero
   - Uses the Cookiy wordmark as the main visual identity.
   - Secondary line: "Designing trust into AI-native research."
   - Devin appears as a byline: `Devin Wang · Founding Product Designer`.
   - Uses `assets/hero-tradeshow.png` to immediately show live market/customer validation.

2. Thesis and brief
   - Main thesis: "Researchers couldn't trust what they couldn't see."
   - Compact meta strip: role, product, scope, and evidence links.
   - Keeps Figma, Agent Skill, and Live Product links visible as proof points.

3. Product visual proof
   - Shows the Cookiy product/device composition using `orb-mask.svg`, monitor assets, and `ipad-complete.png`.
   - Includes the trade-show/customer demo photo below the device composition.

4. `Observe Room`
   - The main case-study section.
   - Uses `assets/observe-room-trust.png`.
   - Frames Observe Room as a trust layer, not just a dashboard.
   - Focuses on session state, AI intent surfaced, verbatim transcript, and quality in real time.

5. `Outcome`
   - Uses bounded language for the metrics:
     - `50,000+ entries / participations`
     - `4 core modules shipped`
     - `6-month validation phase`
     - International demos across Singapore, Germany, and North America
   - Keep the boundary language. Do not rewrite this as if Devin personally generated all users.

6. `Reflection`
   - Opens with a conversational callout and `assets/pet.svg`.
   - Includes a "What I'd do differently" note.
   - Keeps two reflection prompts:
     - Does Every AI Startup Eventually Lose Its App?
     - Confidentiality vs. Visibility?
   - This section is intentionally quieter than the main case sections. It should feel like an afterword, not a second hero.

7. Old website link
   - Links to https://devinwang.net/

## Important Links

Keep these links mapped to the correct page elements:

- Try Demo: https://cookiy-ai-portfolio-demo.vercel.app/
- GitHub Agent Skill: https://github.com/devin55iwl/report-everything
- Figma: https://www.figma.com/design/tfhrrU7GYrmNbKXBvQklmA/Cookiy-AI-2026-?node-id=6-104&t=gnEC8pAiabKZaKxl-1
- Cookiy.AI: https://cookiy.ai/
- Old website: https://devinwang.net/

## Visual Direction

Preserve the current portfolio voice:

- Calm, editorial, high-contrast portfolio case study
- Black, white, warm orange, light grid, and quiet enterprise surfaces
- Use fewer generic cards and more "case study evidence"
- Motion should feel subtle, not flashy
- Avoid making the page feel like a SaaS landing page
- Avoid adding marketing hero blocks unless the user explicitly asks

Recent design decisions:

- The 2026-06-18 refinement moved the page toward a more recruiter-readable product case: Cookiy wordmark, trade-show proof image, concise thesis, and stronger Observe Room evidence.
- `uploads/` from the refinement zip is intentionally not deployed. It contains redundant backups and a nested asset zip.
- `support.js` and `Cookiy AI Case Study.dc.html` are kept in the repository as source/runtime artifacts from the exported package, but `index.html` is the deployed GitHub Pages entry.
- The hero was changed from a personal homepage opening to a project-first Cookiy AI case-study opening.
- The old rotating Daily AI Design Note card was replaced with a static Case Focus card.
- `Design Reflection` was visually reduced so it supports the case instead of overpowering Observe Room.
- The old CSS-made `DV` pixel mark in the reflection callout was replaced with `assets/dv.png`.
- A favicon link now points to `assets/cookiy-logo.png` to avoid a missing favicon request.

## Content Guardrails

Do not add back:

- A `Hi, I'm Devin` first-screen hero on this page
- The rotating Daily AI Design Note card as the main hero support
- "18-person team" framing
- Unbounded "50,000 users" claims
- Generic "I designed many things" language
- Overly broad Design Engineer claims that imply deep engineering ownership

Preferred language:

- "AI-native research SaaS"
- "trust layer"
- "observable, controllable, and trustworthy"
- "entries / participations"
- "validation phase"
- "customer demos and market validation"

## Verification Notes

Latest local checks:

- Desktop reflection layout checked at `1272 x 817`
- Mobile reflection layout checked at `390 x 844`
- `assets/dv.png` loaded correctly at `332 x 334`
- Reflection PNG does not overflow the mobile viewport
- Favicon request fixed by adding `assets/cookiy-logo.png`

Before pushing future visual edits, check:

- Hero on desktop and mobile
- Observe Room section on desktop and mobile
- Outcome section metric wrapping
- Reflection callout and `assets/dv.png`
- All outbound links

## Deployment Notes

This repo is intended to be pushed directly to GitHub Pages. After pushing to `main`, the public URL may take a short time to update:

https://devin55iwl.github.io/cookiy-motion-html/
