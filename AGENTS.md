# PostPlus Social Media Workflow

This repository is configured for social media content workflow, not coding-first assistance.

## Skill Priority

When the user asks for social media strategy, short-form video, UGC ads, AI image/video prompts, TikTok, Reels, Shorts, carousels, hooks, references, storyboards, or pre-generation review, use the installed PostPlus Hook Skills from `.agents/skills/`.

Use the skills as an operator workflow:

1. `pattern-router` — choose the opening route before writing prompts or storyboards.
2. `hook-design` — turn rough hook ideas into a structured Hook Brief.
3. `reference-decode` — decode benchmark videos, frames, screenshots, or rough references into reusable opening structure.
4. `visual-hook` — strengthen the first frame, first slide, or first 1-3 seconds.
5. `prompt-preflight-qa` — review drafts before spending generation credits.

## Default Behavior

- Start with content goals, audience state, platform, segment type, references, and product reveal timing.
- Prefer concrete viewer questions, visible proof, and self-recognition over generic phrases like "viral" or "cinematic."
- Keep the product out of the opening until the hook has earned curiosity, proof, or self-recognition unless `proofFirst` explicitly supports early product presence.
- Produce handoff blocks before final prompt writing so downstream work does not guess the opening logic.
- If the user's input is under-specified, state exactly which missing fields block a reliable hook or prompt.

## Non-Coding Mode

Do not default to implementation plans, tests, or code-review language for social media requests. Treat PostPlus tasks as marketing operations: routing, creative strategy, prompt planning, QA, and publish-ready content handoff.
