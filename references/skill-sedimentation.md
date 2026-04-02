# Skill Sedimentation Audit

Use this checklist only inside an explicit `completion-learn` debrief.

## Goal

Decide whether a completed workflow should remain a one-off lesson, extend an existing skill, or become a new skill.

## Questions

1. Did a stable workflow repeat at least twice inside the task?
2. Would the same workflow likely recur across future tasks or sessions?
3. Can the boundary be explained in 1-2 sentences without hand-waving?
4. Does an existing skill already sit near that boundary?
5. Is there a concrete verifier, script, checklist, or artifact that makes the workflow reliable?
6. Would turning it into a skill reduce future ambiguity, context cost, or operator error?

## Decision Rule

- Prefer `no new skill` when the pattern was interesting but still too situational.
- Prefer `extend existing skill` when the new behavior is adjacent to an existing trigger boundary.
- Prefer `new skill` only when the workflow is stable, reusable, and clearly distinct.

## Output Shape

Keep the audit short:

- `Candidate`: one sentence
- `Why it repeats`: one sentence
- `Best home`: existing skill or new skill
- `Boundary`: the narrowest stable trigger description
- `Next action`: recommend only, unless the user explicitly asks to edit skills

