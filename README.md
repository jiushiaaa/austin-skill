<h1 align="center">austin.skill</h1>

<p align="center">奥斯汀 · J. L. Austin</p>

**中文** · [English](README.en.md)

<blockquote>
<p align="center">“日常语言并不是最后的定论。”<br>— 奥斯汀 · <a href="https://sites.ualberta.ca/~francisp/NewPhil448/AustinPlea56.pdf">〈为借口辩护〉</a></p>
</blockquote>

[![MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) [![Agent Skills](https://img.shields.io/badge/Agent_Skills-Standard-blue.svg)](https://agentskills.io/) [![Made with nvwa-skill](https://img.shields.io/badge/Made_with-nvwa--skill-orange.svg)](https://github.com/alchaincyf/nuwa-skill)

**将言语行为与日常语言辨析整理为思想分析 Skill，让 AI 分清一句话说了什么、做了什么，以及失信、误解与失效究竟发生在哪一层。**

---

## 效果示例

以下为说明用法而编写的示例，展示分析思路；不是哲学家原话或实测对话记录。

### 1. 他说“我保证”，后来承认当时根本不想兑现，那还算承诺吗？

> 不真诚与未作出承诺是两回事。先看语境中承诺是否成立，再看诚意和履行；当时没有兑现意图，可能恰好是这项承诺的缺陷，而不是承诺从未发生。

### 2. “我没看见警告”和“那条规定不合理”，有区别吗？

> 前一句通常涉及行动者知道什么，后一句质疑规则或行为评价。它们需要不同证据，也可能同时出现；不能把两者统称为找借口，更不能仅凭一句解释就宣布免责。

## 蒸馏了什么

| 思想方法 | 能帮助分析什么 |
|---|---|
| 言语行为 | 分开言说内容、施行行为与实际效果。 |
| 失效与不真诚 | 检查资格、程序、诚意与履行，不把所有失败合并。 |
| 借口与辩护 | 追问理由是在改变行为评价，还是减轻行为者的责任。 |

这些方法来自已定位的原作选段，不代表全集蒸馏。具体依据与适用范围见 [SKILL.md](SKILL.md) 和 [提炼说明](EXTRACTION.md)。

## 安装

本 skill 基于开放的 [Agent Skills](https://agentskills.io/) 协议，可在任何 skills-compatible 的 AI agent runtime 中运行（Claude Code、Codex、Cursor、OpenClaw、Hermes Agent、CodeBuddy、Workbuddy、Gemini CLI、OpenCode 等 50+ runtime）。

### 方式一：一行命令

```bash
npx skills add jiushiaaa/austin-skill
```

[Skills CLI](https://github.com/vercel-labs/skills) 可检测受支持的 agent；指定 runtime 时添加 `-a codex`、`-a claude-code` 或 `-a cursor`，全局安装添加 `-g`。这里说明协议与安装器的兼容生态，不代表本项目逐一实测了全部 runtime。

### 方式二：手动安装

克隆仓库后，将完整目录放入 runtime 的 skills 目录，保留 `SKILL.md` 及相对引用。安装目录命名为 `austin-perspective`，与入口元数据一致。常见路径为 Codex 的 `~/.agents/skills/`、Claude Code 的 `~/.claude/skills/`、Cursor 的 `~/.cursor/skills/`；以所用 runtime 当前文档为准。

```bash
git clone https://github.com/jiushiaaa/austin-skill.git
```

### 方式三：作为参考资料

不支持自动加载时，可把 `SKILL.md` 连同当前问题需要的引用文件交给 agent。README 与使用说明提供中英双语，研究底稿保留原语言。

## 使用方式

- **中性思想模式（默认）：**“用奥斯汀的思想分析这个问题，区分原作观点与当代应用。”
- **人物表达模式（可选）：**明确提出“开启人物表达模式”。这是注明性质的模拟，不是作者本人发言。

文游创作默认只取思想，文风另行决定。详见 [双语使用说明](USAGE.md)。

## 调研来源

《如何以言行事》选段；〈为借口辩护〉；相关日常语言分析材料。

- [原作来源、版本与实际阅读范围](references/research/source-catalog.md)
- [方法提炼与证据](EXTRACTION.md)
- 开篇名言出处：<a href="https://sites.ualberta.ca/~francisp/NewPhil448/AustinPlea56.pdf">〈为借口辩护〉</a>，日常语言方法讨论段（节选）。中文引文为本仓库译文；非英语原作的英文引文亦为本仓库译文。

## 仓库结构

主要文件：

```text
├── SKILL.md  # Skill 入口与分析方法
├── README.md / README.en.md  # 中英文介绍
├── USAGE.md  # 双语使用说明
├── EXTRACTION.md  # 方法提炼与证据
├── references/  # 研究笔记与可选人物表达模式
└── LICENSE  # MIT 许可
```

## 构建工具

使用 [nvwa-skill](https://github.com/alchaincyf/nuwa-skill) 构建。

项目原创材料采用 [MIT](LICENSE)，所引原著与译本保留各自权利。详见 [来源说明](ATTRIBUTION.md)。

## 更多 Skill

更多人物 Skill 请查看 [Philosophy Skills 合集](https://github.com/jiushiaaa/Philosophy-Skills)。
