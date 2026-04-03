<p align="center">
  <img src="docs/figs/hero-banner.svg" width="100%" alt="completion-learn" />
</p>

<p align="center">
  <strong>把"做完"变成"变强"的三轴复盘 Skill</strong>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT License" /></a>&nbsp;&nbsp;
  <a href="README.en.md">English</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="docs/three-axis-evolution.md">设计理念</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="SKILL.md">Skill 定义</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="references">References</a>
</p>

---

大多数复盘最终变成两种东西：一份好看的总结，或者一份工具清单。两者都不会让你真正变强。

`completion-learn` 在任务完成后，按固定顺序提取成长收益：

> **Self → Collaboration → Tool**

先看自己哪里该更强，再看人和工具怎么配合更顺，最后才看工具该怎么进化。

这个顺序是刻意的——工具越多，越容易忘记真正需要升级的是你自己。

## 三轴

|  | Self | Collaboration | Tool |
|:---:|---|---|---|
| **核心问题** | 我该保留、停止、练习什么？ | 默认协作模式怎么调？ | 哪些流程值得沉淀成 Skill？ |
| **输出** | Keep · Stop · Practice · Rule | 模式 · 澄清 · Ownership | 沉淀 · 优化 · 路由 |

## 快速开始

```bash
# Codex
cp -r completion-learn ~/.codex/skills/

# Claude Code
cp -r completion-learn ~/.claude/skills/
```

任务完成后运行：

```
/learn-complete
```

也支持聚焦模式：

```
/learn-complete debugging
/learn-complete collaboration
/learn-complete 只做复盘建议，不改 skill 文件
```

## 适合谁

- 高频使用 AI 工具，但开始意识到自己越来越少观察自己
- 想把每轮任务变成下一轮的优势，而不只是做完就算
- 想要一种稳定的 learn loop：**先长自己，再长协作，再长工具**

## Tool 轴的特别设计

大多数复盘只问"要不要做成 Skill"。`completion-learn` 同时问两件事：

- 这段流程**值不值得**沉淀？
- 如果值得，是**新建** Skill，还是**优化**已有的？

诊断先行，路由在后——避免把偶然问题过早固化成系统。

## 深入了解

- **[为什么先是人，不是工具](docs/three-axis-evolution.md)** — 设计理念全文
- [Skill 定义](SKILL.md) — 完整 skill prompt
- [References](references) — 三轴复盘资源包
- [Slash Command](commands/learn-complete.md) — Claude Code 命令封装

## 来源

从 [ai-collab-playbook](https://github.com/cnfjlhj/ai-collab-playbook) 独立拆分。

## License

[MIT](LICENSE)
