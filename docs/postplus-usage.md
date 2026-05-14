# How to Use PostPlus Hook Skills

PostPlus Hook Skills are installed in this project under `.agents/skills/` for a social media content workflow.

## Installed Skills

| Skill | Use it when you need to... | Main output |
| --- | --- | --- |
| `pattern-router` | choose the right short-form opening route before writing | Route Summary |
| `hook-design` | turn a fuzzy or product-first hook into a stable brief | Hook Brief |
| `reference-decode` | analyze a benchmark clip, frame, screenshot, or rough reference | Decode Block |
| `visual-hook` | strengthen the first frame, first slide, or first 1-3 seconds | Visual Hook Plan or Critique |
| `prompt-preflight-qa` | review a storyboard or generation prompt before spending credits | Preflight Report |

## Recommended Workflow

1. **Route the segment** with `pattern-router`.
   - Give the platform, segment type, audience, goal, duration, and whether references exist.
2. **Lock the hook mechanism** with `hook-design`.
   - Use this before writing final captions, storyboards, or provider-ready prompts.
3. **Decode references** with `reference-decode` when you have benchmark videos, frames, or screenshots.
   - The skill separates reusable structure from things that should not be copied.
4. **Strengthen the visual opening** with `visual-hook`.
   - Use this for frame one, first slide, first 1-3 seconds, carousels, or AI video/image prompts.
5. **Run final QA** with `prompt-preflight-qa`.
   - Use this before generating images/video or publishing a storyboard.

## Prompts You Can Use

```text
Use PostPlus to route this TikTok opening before writing the script:
Product:
Audience:
Platform:
Goal:
Duration:
Reference links or screenshots:
Product reveal constraint:
```

```text
Use PostPlus hook-design on this rough opening. Make the Hook Brief explicit before writing variants:
Audience:
Current hook:
Pain/desire:
Offer/product:
What must not feel like an ad:
```

```text
Use PostPlus reference-decode on this benchmark. Extract reusable structure, not exact identity:
Reference description or frames:
What we sell:
Target audience:
What we like about the reference:
What we must avoid copying:
```

```text
Use PostPlus visual-hook to improve the first 3 seconds:
Platform:
Storyboard draft:
Frame-one idea:
Hook mechanism, if known:
Brand/product reveal rule:
```

```text
Use PostPlus prompt-preflight-qa before generation:
Prompt/storyboard:
Target platform:
Reference constraints:
Product timing rule:
Output format needed:
```

## Best Input Checklist

For reliable results, include:
- platform: TikTok, Reels, Shorts, carousel, UGC ad, etc.
- audience state: what the viewer already feels, wants, or believes
- product or offer: what is being sold or promoted
- segment type: hook, benefit, CTA, creator, lifestyle, testimonial, or custom
- references: links, screenshots, frame descriptions, or benchmark notes
- constraints: duration, aspect ratio, brand safety, claims, style, product reveal timing
- success signal: retention, click-through, saves, comments, or generation quality

## Example End-to-End Request

```text
Use the full PostPlus hook workflow for a 20-second TikTok UGC ad.

Product: caffeine-free focus gummies
Audience: remote workers who crash at 3pm but hate coffee jitters
Goal: generate a publish-ready hook brief, first-frame plan, and generation prompt
References: no specific benchmark; use proxy mode
Constraints: product should not appear in frame one; avoid medical claims
Success signal: viewer recognizes the 3pm crash in the first 2 seconds
```

The expected flow is:

1. `pattern-router` produces the route summary.
2. `hook-design` produces the Hook Brief.
3. `reference-decode` runs in proxy mode if there is no benchmark.
4. `visual-hook` creates the first-frame plan.
5. `prompt-preflight-qa` checks the final generation prompt.
