---
name: completion-learn
description: Explicit post-task learning debrief for finished work and /learn-complete requests. Returns a short three-axis retrospective across self, collaboration, and tool. Never auto-trigger mid-task.
---

# Completion Learn

## Overview

Use this skill for an explicit completion debrief. The goal is not a nicer summary. The goal is to turn a finished task into reusable judgment, one next deliberate-practice move, and a clear call on whether any workflow or skill should evolve.

If the user only says `/learn-complete`, interpret it as "help me get better after this task" without requiring extra framing.

Default mode is `three-axis evolution`:
- `Self`
- `Collaboration`
- `Tool`

Prefer a short debrief that changes the next task over a richer one that stays abstract.

## Rules

- Require explicit invocation. Never slide into this mode during normal execution or mid-task updates.
- Only run when the task is complete enough for an honest retrospective. If completion is unclear, say so and stop.
- If the user gives a focus like `debugging`, `workflow`, or `collaboration`, treat it as the primary lens. Otherwise use `references/improvement-axes.md`.
- Prefer the smallest useful output shape from `references/output-structure.md`.
- Focus on reusable judgment, mistake patterns, guardrails, and next behavior change instead of replaying the session.
- Map mistakes to one or two labels from `references/mistake-patterns.md`.
- In default mode, keep the priority order `Self > Collaboration > Tool`.
- End with one durable rule and one next deliberate practice.
- Inside the `Tool` axis, keep `skill sedimentation` separate from `skill evolution / optimize`.
- If the current skill boundary is right but weak, route to `skill-optimizer`.
- If the boundary itself should change or a second complementary skill is needed, route to `skill-creator`.
- If confidence is low, stop at recommendation instead of chaining more skill work.

## When to Use

Use when:

- the user invokes `/learn-complete`
- the user asks for a post-task retrospective, completion debrief, or "what should I remember from this task?"
- the user wants to know whether the finished workflow should optimize an existing skill or become a new one

Do not use when:

- the task is still underway
- the user wants a checkpoint, status update, or implementation work
- the main need is debugging, editing, or normal summarization without reflection

Typical asks:

- `/learn-complete`
- `/learn-complete debugging`
- `这次任务做完了，帮我复盘最该保留的经验`
- `顺便看一下，这次该优化已有 skill 还是新建一个`

## Workflow

1. Confirm completion and pick the primary lens.
2. Choose `Light`, `Standard`, or `Deep` from `references/output-structure.md`.
3. Extract the repeatable win, the main mistake pattern, and the missing guardrail.
4. Convert that into `Self`, `Collaboration`, and `Tool` changes.
5. End with one durable rule, one next deliberate practice, and one tool-evolution judgment.
6. Route to `skill-optimizer`, `skill-creator`, or stop at recommendation.

## Resource Map

- `references/improvement-axes.md`, `references/self-improvement.md`, `references/collaboration-evolution.md` -> default three-axis rubric
- `references/focus-lenses.md`, `references/question-bank.md` -> choose the learning lens and deepen it
- `references/mistake-patterns.md`, `references/output-structure.md`, `references/sample-output.md` -> shape the output and keep it concrete
- `references/skill-sedimentation.md`, `references/skill-evolution.md`, `references/tool-evolution-routing.md` -> decide whether to optimize, extend, add, or stop
- `references/examples.md` -> representative user phrasings
