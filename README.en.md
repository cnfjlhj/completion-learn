<p align="center">
  <img src="docs/figs/hero-banner.svg" width="100%" alt="completion-learn" />
</p>

<p align="center">
  <strong><code>completion-learn</code> · a completion-only three-layer sedimentation skill: after a task is done, what remains?</strong>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT License" /></a>&nbsp;&nbsp;
  <a href="README.md">中文</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="docs/three-axis-evolution.en.md">Design Note</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="SKILL.md">Skill Definition</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="references">References</a>
</p>

---

`completion-learn` is not a recap template and not a prompt dump. It asks a different question after a finished task, especially after a long human-AI exchange: **what should remain?** And just as importantly: **is task completion the same thing as capability retained?**

- `Self`: what should remain from the human side of the interaction, including attention, phrasing, emotional handling, and judgment habits
- `Collaboration`: what should remain as the better default human-AI loop
- `Tool`: what in the tool stack or skill system deserves sedimentation, optimization, or explicit routing

> **Self → Collaboration → Tool**

The order is deliberate: extract what should remain on the human side first, then the collaboration layer, and only then the tooling layer.

## One-Minute Demo

Input:

```text
/learn-complete debugging
```

Typical output shape:

```text
Top lesson
You: Keep
You: Stop
Collaboration: Improve
Tool: Improve
Durable rule
Next drill
Skill sedimentation
```

The goal is not a richer summary. The goal is to leave behind something durable after the task ends.

The visible shape still stays three-axis by default. It does not introduce a noisy fourth section. But internally it now makes a restrained judgment:

- `mostly assisted performance`
- `partial internalization`
- `durable capability gain`

That judgment stays implicit unless the user asks for more depth. Its main job is to avoid confusing "we got it done" with "the capability now remains."

## What Problem It Solves

Most long tasks or long conversations end with one of two weak leftovers:

- a polished summary that expires quickly
- a tool wishlist that keeps pushing you toward more automation

`completion-learn` instead asks:

- what from the human input process is worth keeping?
- what collaboration pattern should become the default?
- what weakness or repeatable workflow in the tool layer is worth turning into system change?

## The Three Axes

|  | Self | Collaboration | Tool |
|:---:|---|---|---|
| **Core question** | What on the human side deserves sedimentation? | What human-AI loop deserves to remain? | What tool/skill changes deserve system entry? |
| **Output** | Keep · Stop · Practice · Rule | Pattern · Clarity · Ownership | Sediment · Optimize · Route |

## Quick Start

```bash
git clone https://github.com/cnfjlhj/completion-learn.git

# Codex
cp -r completion-learn ~/.codex/skills/

# Claude Code
cp -r completion-learn ~/.claude/skills/
```

After installation, use the entrypoint that fits your environment:

```text
# Claude Code
/learn-complete

/learn-complete debugging
/learn-complete collaboration
/learn-complete recommendation only, do not edit skill files

# Codex / other skill-based agents
Use the completion-learn skill for a post-task debrief.
Use completion-learn, focus on debugging.
```

## Who It's For

- Heavy AI-tool users who notice they're observing themselves less over time
- Anyone who does not want a long task to end with only the result and no residue
- People looking for a stable sedimentation order: **self first, then collaboration, then tools**

## What Makes It Different

- completion-only: it activates only after the work is actually done
- residue-first: it asks what remains after the task instead of asking for a nicer summary
- completion != capability gain: it separates task completion from retained capability
- self first: it looks at the human input process before discussing collaboration or tooling
- next drill is not generic advice: it should be a reduced-support test or a nearby transfer task
- diagnostic tool axis: it does not assume "make a new skill"; it first asks whether to sediment, optimize, or stop

## What The Current Version Tightens

- **Same visible structure**: still `Self → Collaboration → Tool`
- **More honest internal judgment**: it no longer treats successful completion as proof that the capability remains
- **Stronger practice design**: `Next drill` is meant to remove one layer of support and test whether the lesson actually stuck

That is the boundary this update tries to keep: **stronger, without becoming louder.**

## When Not To Use

- the task is still in progress and you only need a checkpoint
- you actually need more debugging or implementation
- you only want a feel-good summary

## Tool Axis Design

Most debriefs only ask "should this become a skill?" `completion-learn` asks two things:

- Is this workflow **worth** sedimenting at all?
- If yes, should you **create** a new skill or **optimize** an existing one?

Diagnosis before routing — avoiding premature codification of one-off patterns.

## Learn More

- **[Why self comes before tools](docs/three-axis-evolution.en.md)** — full design note
- [Skill Definition](SKILL.md) — complete skill prompt
- [References](references) — resource pack
- [Slash Command](commands/learn-complete.md) — Claude Code wrapper

## Origin

Split from [ai-collab-playbook](https://github.com/cnfjlhj/ai-collab-playbook) as a standalone skill.

## License

[MIT](LICENSE)
