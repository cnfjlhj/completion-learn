---
name: completion-learn
description: Use when and only when the user explicitly asks for a post-task learning debrief or invokes /learn-complete after the work is done. Include a brief audit for reusable skill opportunities, but do not auto-trigger during normal execution or mid-task checkpoints.
---

# Completion Learn

## Overview

Use this skill for an explicit end-of-task learning debrief. It turns a finished task into durable takeaways, stronger judgment, deliberate practice ideas, and a brief audit of whether any part of the finished workflow deserves to become a new or expanded skill, rather than just producing a nicer summary of what happened.

The default user experience should stay simple: if the user just says `/learn-complete`, treat it as "help me become better after this task" without requiring any extra framing.

The default output should optimize for user benefit, not analytical completeness. A shorter debrief that changes the user's next behavior is better than a richer debrief that stays abstract.

In default mode, the debrief should cover three improvement axes:
- how the user gets better
- how the user and tool get better together
- how the tool stack gets better

## Rules

- Require explicit user intent for the learning debrief; never slip into this mode automatically.
- Only run when the task is actually complete enough to reflect on outcomes and mistakes honestly.
- If the user supplies a focus area, treat it as the primary learning lens. If not, run the default `three-axis evolution mode`: cover the three improvement axes in `references/improvement-axes.md`.
- Focus on reusable judgment, collaboration quality, failure patterns, and what to practice next instead of replaying the whole session.
- Use `references/question-bank.md` to deepen the debrief when the task was novel, messy, or expensive.
- Map mistakes to one or two entries in `references/mistake-patterns.md` instead of leaving them as vague regrets.
- Produce the debrief using the smallest fitting structure from `references/output-structure.md`.
- In default mode, make sure the result contains concrete behavior change across all three axes: what to keep, what to stop, one durable rule, and one next deliberate practice.
- Prefer one strong actionable change over five weak observations.
- If the task was emotionally noisy or cognitively heavy, compress the lesson into a calm, reusable rule rather than mirroring the mess back to the user.
- Include a short `skill sedimentation` check inside the tool-improvement axis: ask whether the right move is to evolve an existing skill, add a second complementary skill, or do nothing.
- In default mode, the priority order is fixed unless the user overrides it: `self improvement > collaboration improvement > tool improvement`.
- Inside tool improvement, cover both `skill sedimentation` and `skill self-evolution / optimize`, not only one of them.
- `completion-learn` owns the diagnosis, not every downstream edit. First decide the right move, then route.
- If the tool-improvement result is "existing skill boundary is right but the skill is weak", route to `skill-optimizer` first.
- If the tool-improvement result is "the boundary should be revised or a new complementary skill should exist", route to `skill-creator`.
- In low-confidence cases, stop at recommendation instead of chaining more skills.
- In sessions where the user has already authorized autonomous improvement, a high-confidence tool-evolution result may continue into `skill-optimizer` or `skill-creator` without another approval step.
- Prefer extending an existing skill over inventing a broad new skill when the boundary is already nearby.
- Keep the skill audit recommendation separate from execution; identifying a candidate does not itself authorize editing local skill files.
- Keep the result easy to absorb and worth reading, not a stiff postmortem report.
- If completion is still unclear, say so and stop rather than forcing the retrospective.

## When to Use

Use when:

- the user invokes `/learn-complete`
- the user explicitly asks for a completion debrief, retrospective, or task-level learning artifact
- the work is done and the next value is reflection rather than execution
- the user wants to know whether the just-finished workflow should be turned into a reusable skill

Do not use when:

- the task is still in progress
- the user only wants a quick checkpoint or status update
- the main need is implementation, debugging, or normal summarization

## Workflow

1. Confirm the task is complete enough for honest reflection.
2. If no explicit focus is given, enter default `three-axis evolution mode`.
3. Choose `Light`, `Standard`, or `Deep` depth and a primary learning lens.
4. Extract the durable lessons, repeatable wins, mistake patterns, and future guardrails.
5. Convert the learning into behavior change for the user axis: what to keep, what to stop, and what to try next.
6. Convert the learning into collaboration improvement: what interaction pattern between the user and tool should become default.
7. Convert the learning into tool improvement: what in the tool stack, workflow, prompts, or skills should evolve.
8. Add one concrete deliberate-practice or next-drill suggestion so the learning can be reused.
9. Run a brief skill-evolution audit: what, if anything, should be optimized in an existing skill, added as a second complementary skill, or left alone.
10. If the result is `optimize existing skill`, route to `skill-optimizer` unless confidence is too low.
11. If the result is `extend existing skill` or `add second complementary skill`, route to `skill-creator` unless confidence is too low.
12. If the result is `no tool change`, stop at the recommendation.

## Resource Map

- `references/skill-sedimentation.md` -> checklist for deciding whether a completed workflow should extend an existing skill or become a new one
- `references/examples.md` -> representative user phrasings for explicit completion debriefs and skill-sedimentation checks
- `references/focus-lenses.md` -> choose the best learning angle such as debugging, design, workflow, collaboration, or research-writing
- `references/improvement-axes.md` -> default three-axis evolution rubric: self, tool stack, and human-tool collaboration
- `references/self-improvement.md` -> keep the self axis grounded in attention, judgment, discipline, and self-noticing
- `references/collaboration-evolution.md` -> improve the operating pattern between the user and the tool
- `references/skill-evolution.md` -> decide whether tool improvement should be an existing skill upgrade, a second complementary skill, or a no-op
- `references/tool-evolution-routing.md` -> decide when to stop at recommendation, when to invoke `skill-optimizer`, and when to invoke `skill-creator`
- `references/question-bank.md` -> deeper reflection questions to use when the user wants richer learning
- `references/output-structure.md` -> `Light`, `Standard`, and `Deep` output shapes
- `references/sample-output.md` -> example of a strong default three-axis debrief with short, actionable wording
- `references/mistake-patterns.md` -> compact taxonomy for turning failures into reusable pattern names

