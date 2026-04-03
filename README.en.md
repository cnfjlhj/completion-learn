<p align="center">
  <img src="docs/figs/hero-banner.svg" width="100%" alt="completion-learn" />
</p>

<p align="center">
  <a href="docs/three-axis-evolution.en.md"><strong>Read the design note</strong></a> · <a href="SKILL.md">SKILL</a> · <a href="references">References</a> · <a href="commands/learn-complete.md">Command Wrapper</a> · <a href="README.md">中文</a>
</p>

---

`completion-learn` is a completion-only learning skill. It is designed for the moment after the work is genuinely done, when the next value is not more execution but better judgment, better collaboration patterns, and better tool evolution.

The default mode is a fixed three-axis debrief:

1. improve the user
2. improve user-tool collaboration
3. improve the tool stack

That order is deliberate. Too many retrospectives jump straight into prompts, scripts, or automation. `completion-learn` starts with attention, judgment, ownership, and self-noticing first, then moves to collaboration, and only then to tools.

> Public-facing label: `Three-Axis Growth Debrief`
>
> One-line pitch: turn a finished task into stronger judgment with a three-axis review: `self -> collaboration -> tool`.

## How To Describe This Repo

If you want to share this repository with someone else, the shortest accurate description is:

> a completion-only learning skill that improves the user first, collaboration second, and tools third, while deciding whether a workflow should become a skill or whether an existing skill should simply be improved.

## What It Does

- turns a finished task into reusable rules instead of a nicer recap
- keeps the visible priority order as `self -> collaboration -> tool`
- treats tool evolution as both `skill sedimentation` and `existing skill optimization`
- routes high-confidence tool decisions into `skill-optimizer` or `skill-creator` instead of forcing the wrong next step

## Repository Contents

- [`SKILL.md`](SKILL.md): the public skill definition
- [`references/`](references): the resource pack behind the three-axis debrief
- [`commands/learn-complete.md`](commands/learn-complete.md): an optional Claude Code slash-command wrapper
- [`docs/three-axis-evolution.en.md`](docs/three-axis-evolution.en.md): the design note behind the skill
- [`docs/figs/hero-banner.svg`](docs/figs/hero-banner.svg): repository banner

## Quick Start

For Codex, place this repository at:

```bash
~/.codex/skills/completion-learn
```

For Claude Code, sync the same directory to:

```bash
~/.claude/skills/completion-learn
```

If you want a direct slash command, also install:

```bash
commands/learn-complete.md
```

into your Claude Code commands directory.

## Default Usage

```text
/learn-complete
```

This means:

> the task is done; help me become better from it.

Supported focus variants:

```text
/learn-complete debugging
/learn-complete workflow
/learn-complete collaboration
```

Recommendation-only mode:

```text
/learn-complete recommendation only, do not edit skill files
```

If you want a more public-friendly label, you can refer to the repo as:

```text
Three-Axis Growth Debrief
```

while keeping the internal skill id as:

```text
completion-learn
```

This keeps local compatibility intact while making the public story easier to spread.

## Tool-Evolution Routing

`completion-learn` is intentionally diagnostic first.

- If the existing skill boundary is still right but the skill is weak, route to `skill-optimizer`.
- If the boundary should expand or a complementary skill should exist, route to `skill-creator`.
- If confidence is low, stop at the recommendation instead of forcing edits.

## Background

This repository is split out from [`ai-collab-playbook`](https://github.com/cnfjlhj/ai-collab-playbook). The standalone version exists because completion debriefing, self-improvement, and skill evolution deserve a clean public home instead of being buried as a small subsection in a larger workflow repo.

## License

Released under the [`MIT`](LICENSE) license.
