# Source design synthesis

Research checked on 2026-09-08. This file records design provenance and maintenance decisions; it is not a phrase bank.

| Source | Distinctive design | Adopted | Rejected or limited |
|---|---|---|---|
| [dating-chat-helper](https://github.com/2218675712/dating-chat-helper) | Fast context inference, short intent/temperature analysis, several response styles, pacing reminders | Immediate-problem-first routing, brevity, relationship-stage calibration, multiple reply trade-offs when wording is requested | A "real intent" label can overstate what one message proves; mandatory hooks can make every reply feel instrumental |
| [LoveHelper.skill](https://github.com/Mowon0303/LoveHelper.skill) | Copilot orchestration, stage assessor, evidence/counterevidence/missing-data discipline, fast and full modes, one primary strategy | Concrete transcript evidence, confidence and counterevidence, observable stage, one objective per turn, quick versus full review | Numeric stage points and fixed aggression/tension ratios create false precision; adversarial frame language can encourage over-escalation |
| [socialization-practice](https://github.com/weiambt/socialization-practice) | Consultation and deliberate-practice modes with scenario, user attempt, evaluation, and repeat loop | Separate coaching from practice, evaluate the user's draft, preserve strengths, train one dimension at a time | Universal formulas and 0–100 scoring can look objective without validated measurement; relationship outcomes are too contextual for that precision |
| [flirting-skill](https://github.com/erikraft/flirting-skill) | Strong personalization, short playful messages, context-specific observations, single versus relationship modes | Specificity, brevity, calibrated playfulness, avoid generic appearance compliments | Claims about triggering dopamine/oxytocin/adrenaline, "99% of men," cold reading, obsession, and guaranteed response are not established by the repository; do not use them as facts or goals |
| [guanxi-skills](https://github.com/yubowen123/guanxi-skills) | Broad intake, goals, stages/signals, risk and consent layers, scenario references | Goal-aware intake, evidence-weighted signals, privacy/consent boundaries, explicit stop conditions | Do not collect irrelevant assets/status data, stereotype by gender, or use PUA labels as evidence; avoid optimizing for conquest over mutual fit |

## Integrated architecture

The synthesis uses three layers:

1. **Evidence layer** — reconstruct the transcript and distinguish fact, interpretation, alternative, and unknown.
2. **State layer** — assess continuity, reciprocity, depth, romantic framing, action, and boundaries; then estimate an observable stage without pretending to read feelings.
3. **Learning layer** — answer the immediate question, review the user's decision process, and create one testable improvement experiment.

This architecture intentionally shifts value away from canned wording. Generated text is optional output; the durable product is better observation, calibration, and self-authored communication.

## Claims discipline

The repositories are design examples, not scientific validation. Descriptions such as "neuroscience-based," stage scores, attraction triggers, or universal interest signals remain author claims unless independently supported. This skill treats them as hypotheses or discards them when they encourage false certainty or manipulation.

No source messages are copied into this skill. Concepts were restructured and rewritten around evidence, reciprocity, autonomy, and learning.
