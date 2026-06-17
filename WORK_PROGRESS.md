# Cookiy Motion HTML - Work Progress

Last updated: 2026-06-17

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

1. Personal hero
   - "Hi, I'm Devin."
   - Positions Devin as an AI Product Designer / Design Engineer.
   - Uses a grid/editorial personal website style.

2. Cookiy hero
   - Title: "Teaching an AI to listen."
   - Explains Cookiy AI as an AI-native research SaaS.
   - Focus: making the AI observable, controllable, and trustworthy for researchers.

3. `01 Context`
   - Explains the research workflow:
     discussion guide creation, participant recruitment, AI-moderated interviews, observation, insight generation, and reporting.

4. `02 My Role` and `03 Core Challenge`
   - Role: Founding Product Designer.
   - Scope: AI workflow design, complex states, core modules, interactive demos, and customer-facing presentation experiences.
   - Core challenge: AI interviews cannot feel like automation running in the dark.

5. `04 Design System of Trust`
   - The main case-study section.
   - Uses `assets/observe-room-trust.png`.
   - Frames Observe Room as a trust layer, not just a dashboard.
   - Trust signals include:
     - Live Transcript
     - AI Behavior Monitoring
     - Participant Status
     - Quality Judgment
     - Human Intervention
     - Follow-up / Signals

6. `05 Outcome`
   - Uses bounded language for the metrics:
     - `50,000+ entries / participations`
     - `4 core modules shipped`
     - `6-month validation phase`
     - International demos across Singapore, Germany, and North America
   - Keep the boundary language. Do not rewrite this as if Devin personally generated all users.

7. `Design Reflection`
   - Editorial closing section with three reflection prompts:
     - Does Every AI Startup Eventually Lose Its App?
     - Enterprise Product, Consumer Dynamics?
     - Confidentiality vs. Visibility?
   - Ends with a callout using `assets/dv.png`.

8. Old website link
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

- The old CSS-made `DV` pixel mark in the reflection callout was replaced with `assets/dv.png`.
- The PNG should stay attached to the lower-right edge of the reflection callout.
- A favicon link now points to `assets/cookiy-logo.png` to avoid a missing favicon request.

## Content Guardrails

Do not add back:

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

