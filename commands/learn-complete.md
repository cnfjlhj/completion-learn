---
description: Run an explicit post-task learning debrief after all work is complete
argument-hint: [optional-focus]
disable-model-invocation: true
---

This command is an explicit completion-only learning debrief.

Default usage is just:

- `/learn-complete`

That means: "the task is done; help me get better from it."

`$ARGUMENTS` is optional, not required.

First, determine whether the task is genuinely complete. Accept completion only when at least one of these is true:

- the user explicitly says all tasks are done
- the current task tracker or todo set is fully complete
- the surrounding context makes it clear that no requested work remains

If completion is not clear, do not run the debrief. Reply briefly that `/learn-complete` is for finished tasks only and suggest waiting until the task is truly done.

If completion is clear:

1. Activate the `completion-learn` skill.
2. Use the whole current task context, not only the latest message.
3. Before writing the debrief, privately judge whether the outcome was closer to:
   - `mostly assisted performance`
   - `partial internalization`
   - `durable capability gain`
   Keep this judgment implicit by default. Do not add it as a visible fourth section unless the user explicitly asks for that distinction.
4. If `$ARGUMENTS` is empty, run the default three-axis evolution mode.
   The result should tell the user:
   - what mattered most
   - how they themselves should improve
   - how they and the tool should collaborate better
   - how their tool stack should improve
   - one durable rule to keep
   - one concrete next practice
   - one concrete collaboration-evolution recommendation
   - one concrete tool-evolution recommendation
   - in tool evolution, explicitly consider both skill sedimentation and existing-skill optimization
5. Shape the `next practice` using that private judgment:
   - assisted outcome -> reduced-support retry on one small step
   - partial internalization -> same bottleneck, user first and tool second
   - durable gain -> nearby transfer task instead of same-task repetition
6. If `$ARGUMENTS` is non-empty, treat it as an emphasis or focus area.
   Examples: `debugging`, `design`, `workflow`, `collaboration`, `research-writing`, `tool-use`, `decision-quality`, or a free-form question.
7. In default mode, keep the visible priority order as:
   - self
   - collaboration
   - tool
   unless the user explicitly overrides it.
8. Pick one primary learning lens from the skill's references. Add a secondary lens only if it materially improves the debrief.
9. Pick `Light`, `Standard`, or `Deep` depth based on novelty, mistakes, decisions, and likely future reuse.
10. Produce the completion debrief in the skill's structure, including:
   - durable rules
   - repeatable wins
   - mistake patterns
   - one deliberate-practice next step that tests retained judgment under less support or in a nearby transfer context
   - skill evolution check
11. If the tool-evolution result is high-confidence:
   - use `skill-optimizer` when an existing skill should be improved without changing its boundary
   - use `skill-creator` when an existing skill boundary should expand or a second complementary skill should be added
12. If confidence is low, stop at the recommendation instead of forcing skill edits.

Additional constraints:

- Do not write code or modify files as part of this command.
- Do not save notes automatically.
- Optimize for durable understanding, not for a feel-good summary.
