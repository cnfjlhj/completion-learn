<p align="center">
  <img src="docs/figs/hero-banner.svg" width="100%" alt="completion-learn" />
</p>

<p align="center">
  <strong>Turn finished tasks into lasting growth — self first, tools last.</strong>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT License" /></a>&nbsp;&nbsp;
  <a href="README.md">中文</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="docs/three-axis-evolution.en.md">Design Note</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="SKILL.md">Skill Definition</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="references">References</a>
</p>

---

Most post-task reviews end up as either a polished summary or a tool wishlist. Neither makes you stronger.

`completion-learn` runs a fixed three-axis debrief after a task is done:

> **Self → Collaboration → Tool**

First, what should *you* keep, stop, or practice. Then, how should the human-tool loop change. Only then, what deserves to become a skill.

The order is deliberate — tools are seductive, and they easily crowd out the harder question: *did you actually grow?*

## The Three Axes

|  | Self | Collaboration | Tool |
|:---:|---|---|---|
| **Core question** | What to keep, stop, practice? | What should the default loop be? | What deserves sedimentation? |
| **Output** | Keep · Stop · Practice · Rule | Pattern · Clarity · Ownership | Sediment · Optimize · Route |

## Quick Start

```bash
# Codex
cp -r completion-learn ~/.codex/skills/

# Claude Code
cp -r completion-learn ~/.claude/skills/
```

After a task is done:

```
/learn-complete
```

Focus variants:

```
/learn-complete debugging
/learn-complete collaboration
/learn-complete recommendation only, do not edit skill files
```

## Who It's For

- Heavy AI-tool users who notice they're observing themselves less over time
- Anyone who wants each task to compound into the next advantage
- People looking for a stable learning loop: **grow yourself first, then collaboration, then tools**

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
