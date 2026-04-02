# completion-learn: why tool changes should not be the first move after a finished task

Many people treat task completion as the endpoint.

For heavy AI-tool users, that is usually the exact moment where the most valuable learning is either captured or wasted. The context is still fresh. The real bottlenecks, wrong assumptions, and useful moves are still visible. If you do not convert them into reusable rules, they disappear back into the transcript.

`completion-learn` is built around one idea:

> completion is not the end of the task; it is the entry point to the learning loop.

The problem is that most post-task reflection degrades into one of two weak forms:

1. a nicer recap
2. a tool-first wishlist with little human growth inside it

That is why the default order is fixed:

1. `self`
2. `collaboration`
3. `tool`

## Why self comes first

The main failure mode for many AI-heavy workflows is not lack of tools. It is loss of attention, weaker self-noticing, and outsourced judgment.

If each retrospective jumps straight to prompts, scripts, agents, and automation, the user may learn more setup details while becoming less capable of noticing:

- what the real bottleneck was
- which judgment should have stayed local
- what should be practiced next
- where stronger self-observation would have changed the outcome

The self axis exists to reverse that drift. It keeps the first claim on attention for:

- `Keep`
- `Stop`
- `Practice next`
- `Durable rule`

These are small outputs on purpose. The goal is not reflection theater. The goal is next-task behavior change.

## Why collaboration comes second

The collaboration axis is not generic teamwork language. It is about the operating loop between the human and the tool:

- what interaction pattern should become default
- what should be clarified earlier
- how much visibility is enough
- where ownership should stay with the human and where the tool should act

Many painful tasks come from unstable collaboration patterns rather than weak human ability or weak tools in isolation. Fixing the operating loop often pays off longer than a local prompt tweak.

## Why tool comes last

Tool evolution matters, but it is seductive. It easily crowds out the harder and more important reflections.

After a task, people naturally want to ask:

- should I add another script?
- should I turn this into a skill?
- should I add more automation?

Those are valid questions, but if they arrive too early, the result is usually a larger tool stack instead of a stronger operator.

That is why the tool axis in `completion-learn` explicitly covers both:

1. `skill sedimentation`
2. `existing skill optimization`

It does not only ask whether a workflow should become a new skill. It also asks whether the real move is to improve an existing skill instead of creating yet another one.

## Why diagnosis should come before routing

This skill is intentionally diagnostic first.

The right structure is:

1. `completion-learn` diagnoses the lesson
2. route to `skill-optimizer` when the skill boundary is still right but the skill is weak
3. route to `skill-creator` when the boundary should expand or a complementary skill should exist
4. stop at recommendation when confidence is low

Without that separation, it is too easy to overfit one intense task and prematurely hard-code it into the tool system.

## A healthier long-term loop

The intended learning loop is:

```text
task done
  -> self: how does the user become stronger
  -> collaboration: how do user and tool work better together
  -> tool: what deserves sedimentation or optimization
```

This order is not about completeness. It is about preventing drift toward tool obsession while protecting judgment, ownership, and clarity.

## When not to use it

Do not use `completion-learn`:

- when the task is still in progress
- when you only need a checkpoint
- when the real need is more implementation or debugging
- when what you want is emotional closure instead of reusable learning

It is a completion-only lane.

## Why this repository exists

This skill was split into a standalone repository because the pattern is important enough to deserve a clean public home:

- completion debriefing should be more than a closing summary
- self-improvement should not be buried under tool chatter
- collaboration patterns should be made explicit
- tool evolution should include both new-skill sedimentation and existing-skill improvement

The main question after a finished task is not only whether the task succeeded.

It is whether the user became stronger from it.

