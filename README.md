<p align="center">
  <img src="docs/figs/hero-banner.svg" width="100%" alt="completion-learn" />
</p>

<p align="center">
  <strong><code>completion-learn</code> · 一个 completion-only 的三轴沉淀 skill：任务做完以后，留下些什么</strong>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT License" /></a>&nbsp;&nbsp;
  <a href="README.en.md">English</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="docs/three-axis-evolution.md">设计理念</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="SKILL.md">Skill 定义</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="references">References</a>
</p>

---

`completion-learn` 不是 recap 模板，也不是 prompt 清单。它关心的是一轮任务，尤其是一段很长的人机对话结束以后，**到底能留下什么**，以及**这次做成了和你真的长出来了什么，到底是不是同一件事**：

- `Self`：从人的输入过程里，留下什么值得保留的觉察、表达、情绪处理和判断习惯
- `Collaboration`：从你和 AI 的协作过程里，留下什么更稳的默认模式
- `Tool`：从工具和 skill 本身里，留下什么值得沉淀、优化或分流的系统性改进

> **Self → Collaboration → Tool**

这个顺序是刻意的：先看人这边能沉淀什么，再看协作层，最后才看工具层，而不是一上来就继续堆自动化。

## 一分钟看懂

输入：

```text
/learn-complete debugging
```

输出的核心形状会类似：

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

它追求的不是“复盘得很完整”，而是“这轮结束后真的留下了东西”。

默认对外形状还是三轴，不会平白多出一个第四段。但内部会先做一个很克制的判断：

- 这次更像 `mostly assisted performance`
- 还是 `partial internalization`
- 还是 `durable capability gain`

这个判断默认不外显，它主要用来避免把“一次任务做成了”误判成“已经真正学会了”。

## 它解决什么问题

大多数长任务或长对话做完以后，最后只会剩下两种东西：

- 一份好看但很快失效的总结
- 一份继续鼓励你堆工具的待办清单

`completion-learn` 强制把问题改成：

- 这次从你自己的输入过程里，哪些东西值得留下来？
- 这次你和 AI 的协作里，哪些模式值得默认化？
- 这次工具本身暴露了什么不足，哪些流程真的值得沉淀成 skill？

## 三轴

|  | Self | Collaboration | Tool |
|:---:|---|---|---|
| **核心问题** | 从人的输入过程里，什么值得沉淀？ | 哪种人机协作模式值得留下？ | 哪些工具/skill 改进值得进入系统？ |
| **输出** | Keep · Stop · Practice · Rule | 模式 · 澄清 · Ownership | 沉淀 · 优化 · 路由 |

## 快速开始

```bash
git clone https://github.com/cnfjlhj/completion-learn.git

# Codex
cp -r completion-learn ~/.codex/skills/

# Claude Code
cp -r completion-learn ~/.claude/skills/
```

安装后，按你的环境使用：

```text
# Claude Code
/learn-complete

/learn-complete debugging
/learn-complete collaboration
/learn-complete 只做复盘建议，不改 skill 文件

# Codex / 其他基于 skill 的 agent
请用 completion-learn 做一个任务完成后的复盘。
请用 completion-learn，重点复盘 debugging。
```

## 适合谁

- 高频使用 AI 工具，但开始意识到自己越来越少观察自己
- 不想任务做完只剩结果，想把长对话里的有效部分沉淀下来
- 想要一种稳定的沉淀顺序：**先看自己，再看协作，再看工具**

## 它和普通复盘有什么不同

- completion-only：只在任务真的做完后启动，不抢中途注意力
- residue-first：它问的不是“总结一下”，而是“这轮结束后到底留下什么”
- completion != capability gain：它会把“这次完成了”和“你真的长出来了什么”分开判断
- self first：先看人的输入过程和自我观察，再谈协作和工具
- next drill 不是泛建议：默认会给一个降辅助的小测试，或一个相邻迁移任务
- tool axis 有诊断分流：不是默认“新建一个 skill”，而是先判断该沉淀、该优化、还是根本不该固化

## 新版现在更强调什么

- **外显结构不变**：还是 `Self → Collaboration → Tool`
- **内部判断更诚实**：不再默认把“任务做成”当成“能力已经留下”
- **练习更像验收**：`Next drill` 默认会减少一层帮助，先看你自己还能不能保住关键判断

这也是这次更新最想保住的边界：**更强，但不更吵。**

## 什么时候不要用

- 任务还没做完，只是想要 checkpoint
- 你真正需要的是继续 debug / 继续实现
- 你只是想要一份情绪价值型总结

## Tool 轴的特别设计

大多数复盘只问“要不要做成 skill”。`completion-learn` 会多问一步：

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
