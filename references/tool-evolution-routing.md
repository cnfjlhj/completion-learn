# Tool Evolution Routing

Use this note after the tool-improvement axis has already produced a candidate.

The question here is no longer "is there a tool lesson?" It is "what should happen next?"

## Routing Outcomes

- `Stop at recommendation`
- `Route to skill-optimizer`
- `Route to skill-creator`

## Route To `skill-optimizer`

Use when:
- the current skill boundary is still correct
- the weakness is in triggers, references, workflow, examples, routing quality, or under/over-trigger behavior
- you need a read-first audit before deciding the exact rewrite

Typical signs:
- the skill exists but underperforms
- the skill is too vague, too bloated, or misroutes
- transcript evidence is needed before editing

## Route To `skill-creator`

Use when:
- a skill boundary should expand
- a new complementary skill should be added
- the structure of `SKILL.md`, `references/`, or route definition itself needs revision

Typical signs:
- there is a stable new lane not covered by the current skill
- the current skill is overloaded and needs a cleaner boundary
- the audit already made the rewrite direction clear enough

## Stop At Recommendation

Use when:
- confidence is low
- the pattern only occurred once
- there is no stable skill boundary yet
- the cost of editing skills is higher than the likely reuse

## Confidence Rule

Only chain automatically when:
- the current session already authorizes autonomous improvement
- the candidate is concrete
- the smallest next change is obvious

Otherwise stop at the recommendation.

