# WAKEUP.md — sentys.ai redesign overnight run

**Started:** 2026-07-12 01:45 CEST · **Branch:** `redesign` · **Protocol:** ~/sensory/docs/OVERNIGHT_PROTOCOL.md
**Prompt:** RUN_PROMPT.md (untracked, kept out of git via .git/info/exclude along with sensory/)

## Current milestone
M1 — Concept bake-off (3 hero prototypes under /concepts, screenshot, judge, pick winner)

## Done
- [x] M0 Setup: read ONE_PAGER/VISION/MANIFESTO/EVIDENCE/WORLD_MODEL + current site copy;
      branch `redesign`; 5 staggered resume pings armed (03:00/04:15/05:45/07:15/08:45);
      tasks #1–#9 created (TaskList); Chrome + GEMINI_API_KEY + python3/node verified.

## Next step
Build 3 genuinely different hero prototypes in /concepts/{a,b,c}/index.html,
screenshot at 1440px + 390px with headless Chrome, judge, record verdict here.

## Milestone map
M1 bake-off → M2 full site build → M3 media assets → M4 guide+concepts notes →
M5 brand kit + og.png → M6/M7/M8 iteration passes 1–3 → M9 mirror to
~/sensory/docs/product/website/ + PR.

## Key constraints (from prompt — binding)
- Claims ONLY from current site copy or ~/sensory/docs/EVIDENCE.md. WORLD_MODEL = inspiration, never claims.
- ≤6 shipped generated images; Gemini ≤15 calls total incl. retries; ≤2 short clips (Higgsfield unlimited models preferred: Wan 2.2 motion / Soul 2.0 stills); watermark-free only.
- Preserve routes: demo/, sample-report.html, data-spec.html, CNAME. Keep SEO metadata.
- prefers-reduced-motion respected; fast on mobile; accessible contrast.
- Mirror final files to ~/sensory/docs/product/website/ (BOTH copies get edits).
- /guide unlinked page crediting Claude; losing concepts stay in /concepts.
- brand/logo.png (≥1024², readable at 48px round crop) + brand/linkedin-cover.png (1128×191 center-safe).
- NEVER `git add` sensory/ or RUN_PROMPT.md (excluded locally).
- Open PR when 3 iteration passes complete. Do not merge.

## Spend tally (paid/credit generations)
| # | When | Service | Model | What | Result |
|---|------|---------|-------|------|--------|
| — | — | — | — | nothing spent yet | — |
Gemini calls used: 0/15 · Higgsfield metered credits used: 0 · Clips shipped: 0/2 · Images shipped: 0/6

## Open problems
- ffmpeg not on PATH (only `convert`) — check again before video work; degrade to code-driven motion if clips can't be compressed.

## Re-orientation (on any revival)
1. Read this file. 2. `git log --oneline -5` + `git status`. 3. TaskList → find first non-completed task. 4. Continue idempotently — NEVER redo paid generations (check spend tally + assets/ on disk first).
