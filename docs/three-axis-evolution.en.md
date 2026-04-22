# Why tool changes should not be the first move after a finished task

> Completion is not the end of the task — it is the entry point to the sedimentation loop.

For heavy AI-tool users, the moment a task is done is usually the moment where the most valuable residue is either captured or wasted. This is especially true after a long human-AI exchange: the context is still fresh, the input process is still visible, and the emotional or judgmental drift has not yet faded. You can turn that into something durable — or let it dissolve into "anyway, it's done."

The problem is that most post-task reflection degrades into one of two weak forms:

1. A nicer recap that nobody acts on
2. A tool-first wishlist with no human growth inside it

`completion-learn` fixes this by locking the default question into three layers: **Self → Collaboration → Tool**.

---

## Self: why the human comes first

The main failure mode for many AI-heavy workflows is not lack of tools. It is loss of attention, weaker self-noticing, degraded phrasing, emotional drift, and outsourced judgment.

You may know more commands, more prompts, more skills — but if you stop asking yourself:

- How did I phrase the task, and where did I amplify confusion?
- Did emotion distort the way I interacted with the model?
- Did I outsource a judgment that should have stayed with me?
- What from the human input process is actually worth keeping?

— then more tools just means more drift.

The Self axis exists to reverse that. It looks at the human side of the interaction: attention, phrasing, emotional handling, ownership, and judgment habits.

It still demands four concrete outputs: **Keep · Stop · Practice next · Durable rule**. On purpose. What lasts is not abstraction, but these retained moves.

## Collaboration: why the operating loop comes second

The Collaboration axis is not generic teamwork advice. It is about one specific question: what operating loop between you and the AI deserves to remain as the default?

- What interaction pattern should become default?
- What should be clarified earlier next time?
- How much visibility is enough — not overloaded, not blind?
- Where should ownership stay with you, and where should the tool act?

Many painful tasks come from unstable collaboration patterns, not from weak humans or weak tools in isolation. A better operating loop found in one task often outlasts any local prompt tweak because it is exactly the kind of thing that should remain.

## Tool: why it comes last

Not because tools do not matter, but because they are seductive. The moment you start a debrief, the natural impulse is: *should I add another script? Another command? Another automation?* That impulse can hide the more important question of what should remain on the human or collaboration side.

Those are valid questions. But if they arrive before the first two axes are done, the result is a larger tool stack instead of a stronger operator.

The Tool axis covers two things, both with restraint:

1. **Skill sedimentation** — is this workflow worth turning into a skill at all?
2. **Existing skill optimization** — if yes, should you create something new or improve what already exists?

This layer also includes what the AI or tool stack itself revealed as weak during the task. Diagnosis first. If confidence is low, stop at the recommendation instead of writing anything into the system.

## Completion is not the same as capability gain

This is the main reinforcement in the current version of `completion-learn`.

After an AI-heavy task, the easiest mistake is not "forgetting to debrief." The easier mistake is **confusing completion with internalization**. A successful outcome may mean very different things:

- the tool mostly scaffolded the result
- part of the judgment stuck, but support still mattered
- a durable, transferable capability actually formed

All three can look like "the task got done." They should not produce the same next step.

The more stable loop now looks like:

```text
task done
  → (internal) capability residue judgment
  → self
  → collaboration
  → tool
```

That internal judgment serves two purposes:

1. avoid mistaking one successful run for retained skill
2. make `Next deliberate practice` behave more like a check than a suggestion

It is intentionally kept implicit by default. Turning it into a visible fourth axis would make the skill louder without making it better. The goal here is not more theory on the surface. It is more honesty inside the debrief.

### How practice should change

If the outcome was closer to:

- `mostly assisted performance`
  the next practice should be very small and start with one independent step before the tool helps
- `partial internalization`
  the next practice should stay on the same bottleneck, but run human-first and tool-second
- `durable capability gain`
  the next practice should move to a nearby transfer task instead of mechanically repeating the same one

This looks like a small change, but it is the real test of whether a learning skill works. A good debrief does not merely say something insightful. It designs the next attempt so the retained judgment can actually be checked.

---

## Diagnosis before routing

`completion-learn` does not assume "a new skill should be created." It diagnoses first, then routes:

- Boundary still correct but skill is weak → `skill-optimizer`
- Boundary should expand or a complementary skill is needed → `skill-creator`
- Evidence insufficient → stop at recommendation

This prevents a common failure: one intense task finishes, emotions and context are running hot, and a one-off pattern gets prematurely hard-coded into the tool system.

## The long-term sedimentation loop

If you work with AI tools over time, the intended sedimentation loop is:

```
task done
  → (internal) residue judgment:  mostly assisted, partial internalization, or durable gain
  → self:                        what should remain from the human input process
  → collaboration:               what default human-AI loop should remain
  → tool:                        what system change deserves sedimentation or optimization
```

The point of this order is not completeness — it is **drift prevention**. It stops the debrief from sliding into tool obsession, and it also prevents a different mistake: treating one completed task as proof that the capability now remains.

## When not to use it

`completion-learn` is completion-only. Do not use it when:

- The task is still in progress
- You only need a checkpoint
- The real need is more implementation or debugging
- What you want is emotional closure, not reusable learning

It fits exactly one moment: **the task is done enough to be honest about what happened.**

---

The real question after a finished task is not whether it succeeded. It is what actually remains after it ends.
