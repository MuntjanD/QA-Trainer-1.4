# AI Prompt Log — Beginner Prompts for QA-Trainer-1.4

Purpose
- Short, copy-paste prompts for a newbie or intern to use when working on this QA Trainee sandbox (single-file HTML app).
- Each prompt is tailored to this project so you get useful, actionable answers quickly.

How to use
- Copy one prompt exactly (or tweak the parts in <>), paste into your AI assistant, and run.
- After applying changes, add a short log entry using the template at the bottom.

Entry template (one-line each)
- Date: YYYY-MM-DD | Role: Newbie | Prompt-used: short title | Commit: message or link

Beginner prompts (copy-paste)

1) Project orientation / MVP
"I am new. Give me a 1-paragraph explanation of what the repo QA-Trainer-1.4 does and a 3-step checklist to get the single-file app running locally in a browser. Mention the main file `QA_Trainee_Vers_1_4.html` and README.md."

2) Find visual bugs quickly
"Act like a junior QA. Explain 5 easy checks I can do in the browser to find visual bugs in `QA_Trainee_Vers_1_4.html` (layout, overflow, z-index, colors, responsive). Provide exact browser tools/steps (DevTools panels and what to look for)."

3) Reproduce and fix a functional bug (coupon stacking)
"I am new. The app has a coupon code `FREE100` that may stack infinitely. What quick code change (1–4 lines) can I make in `QA_Trainee_Vers_1_4.html` to prevent stacking the discount? Show the exact JS change and where to paste it."

4) Mobile testing checklist
"List 6 focused tests I should run on mobile/emulator for QA-Trainer-1.4 (touch, input focus, modals, form submission, breakpoints, cart interactions). For each test include one expected result and one quick debugging tip."

5) SQL lab starter query
"I am learning the Warehouse SQL Lab in QA-Trainer-1.4. Give me 3 simple SELECT queries to practice (all products, products with stock 0, products price > 100) and explain what each query returns in one sentence."

6) Write a helpful PR description
"I fixed a bug in `QA_Trainee_Vers_1_4.html` and added a short test. Write a concise PR description (3-5 lines) that explains the problem, the change, and how to test it in the browser. Include suggested commit message."

7) Accessibility quick fix
"I am new. Suggest 3 small accessibility improvements I can make to `QA_Trainee_Vers_1_4.html` (aria attributes, focus order, color contrast) and show the minimal code changes needed for each."

8) Logging AI usage (how to add an AI log entry)
"Show me one short AI log entry I can add to docs/AI_PROMPT_LOG.md after I used a prompt to fix the coupon bug. Use the entry template and include a sample commit message."

Quick commit/branch steps (for newbies)
- Create a branch: git checkout -b feature/ai-prompts
- Add file: git add docs/AI_PROMPT_LOG.md
- Commit: git commit -m "ai-log: add beginner AI prompts for interns"
- Push: git push origin feature/ai-prompts
- Open a PR with the short description from prompt #6 above.

Template log example (copy into docs/AI_PROMPT_LOG.md)
- Date: 2026-10-14 | Role: Newbie | Prompt-used: "Fix coupon stacking" | Commit: ai-fix: prevent coupon stacking | Notes: Applied check to avoid double-apply; tested in browser.
