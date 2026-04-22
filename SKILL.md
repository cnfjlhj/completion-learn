---
name: completion-learn
description: Use when the user explicitly asks for /learn-complete or a post-task debrief after work is finished. Extract what should remain after a long task across self, collaboration, and tool. Never auto-trigger mid-task.
---

# Completion Learn

## Overview

Use this skill for an explicit completion debrief. The goal is to extract what should remain after a finished task across self, collaboration, and tool.

If the user only says `/learn-complete`, interpret it as "help me see what should remain after this task."

Default mode is `three-axis evolution`:
- `Self`
- `Collaboration`
- `Tool`

Prefer a short debrief with durable residue over abstract richness.
Treat `task completed` and `capability gained` as separate judgments.

## Rules

- Require explicit invocation. Never slide into this mode during normal execution or mid-task updates.
- Only run when the task is complete enough for an honest retrospective. If completion is unclear, say so and stop.
- If the user gives a focus like `debugging`, `workflow`, or `collaboration`, treat it as the primary lens.
- Prefer the smallest useful output shape from `references/output-structure.md`.
- Focus on what should remain from the long interaction instead of replaying the session.
- Before writing the axes, privately judge the residue level:
  - `mostly assisted performance`
  - `partial internalization`
  - `durable capability gain`
- Keep that residue judgment internal by default. Do not add a fourth visible section unless the user asks for deeper explanation or the distinction is the main lesson.
- Inside `Self`, inspect the user's side of the interaction: attention, phrasing, emotion, ownership, and judgment habits.
- Inside `Collaboration`, inspect what interaction pattern between the user and AI should become default.
- Map mistakes to one or two labels from `references/mistake-patterns.md`.
- In default mode, keep the priority order `Self > Collaboration > Tool`.
- End with one durable rule and one next deliberate practice.
- Make `next deliberate practice` a reduced-support test, not generic advice. It should check whether the claimed residue actually remains when one layer of help is removed.
- If the residue is `mostly assisted performance`, keep the practice narrow and ask the user to do one small step alone before using the tool.
- If the residue is `partial internalization`, make the practice user-first and tool-second on the same bottleneck.
- If the residue is `durable capability gain`, move the practice to a nearby transfer task instead of repeating the exact same one.
- Inside the `Tool` axis, keep `skill sedimentation` separate from `skill evolution / optimize`.
- If the current skill boundary is right but weak, route to `skill-optimizer`.
- If the boundary itself should change or a second complementary skill is needed, route to `skill-creator`.
- If confidence is low, stop at recommendation instead of chaining more skill work.

## When to Use

Use when:

- the user invokes `/learn-complete`
- the user asks for a post-task retrospective, completion debrief, or "what should remain from this task?"
- the user wants to know whether the finished workflow should optimize an existing skill or become a new one

Do not use when:

- the task is still underway
- the user wants a checkpoint, status update, or implementation work
- the main need is debugging, editing, or normal summarization without reflection

Typical asks:

- `/learn-complete`
- `/learn-complete debugging`
- `顺便看一下，这次该优化已有 skill 还是新建一个`

## Workflow

1. Confirm completion and pick the primary lens.
2. Choose `Light`, `Standard`, or `Deep` from `references/output-structure.md`.
3. Judge whether the outcome was mostly assisted, partially internalized, or a durable capability gain.
4. Extract the strongest residue worth keeping, the main mistake pattern, and the missing guardrail.
5. Convert that into `Self`, `Collaboration`, and `Tool` sedimentation without changing the visible three-axis shape.
6. End with one durable rule, one next deliberate practice, and one tool-evolution judgment.
7. Make sure the practice step matches the residue judgment by reducing support or forcing transfer.
8. Route to `skill-optimizer`, `skill-creator`, or stop at recommendation.

## Resource Map

- `references/improvement-axes.md`, `references/self-improvement.md`, `references/collaboration-evolution.md` -> default three-axis rubric
- `references/focus-lenses.md`, `references/question-bank.md` -> choose the learning lens and deepen it
- `references/mistake-patterns.md`, `references/output-structure.md`, `references/sample-output.md` -> shape the output and keep it concrete
- `references/skill-sedimentation.md`, `references/skill-evolution.md`, `references/tool-evolution-routing.md` -> decide whether to optimize, extend, add, or stop
- `references/examples.md` -> representative user phrasings
