<h1 align="center">austin.skill</h1>

<p align="center">奥斯汀 · J. L. Austin</p>

[中文](README.md) · **English**

<blockquote>
<p align="center">“Ordinary language is not the last word.”<br>— J. L. Austin · <a href="https://sites.ualberta.ca/~francisp/NewPhil448/AustinPlea56.pdf">A Plea for Excuses</a></p>
</blockquote>

[![MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) [![Agent Skills](https://img.shields.io/badge/Agent_Skills-Standard-blue.svg)](https://agentskills.io/) [![Made with nvwa-skill](https://img.shields.io/badge/Made_with-nvwa--skill-orange.svg)](https://github.com/alchaincyf/nuwa-skill)

**A thinking skill for speech acts and ordinary-language distinctions: separate what an utterance says, what it does, and where a promise, procedure, or explanation goes wrong.**

---

## Examples

Illustrative applications written for this README; these are not quotations from the philosopher or transcripts of a live run.

### 1. Someone said “I promise” but never intended to follow through. Was it a promise?

> Insincerity differs from never making a promise. Establish whether a promise was made in that setting, then examine intention and performance. The lack of intention may be a defect in the promise rather than proof that no promise occurred.

### 2. How do “I did not see the warning” and “the rule was unreasonable” differ?

> The first concerns what the agent knew; the second challenges a rule or the evaluation of an act. They require different evidence and can coexist. Neither automatically removes responsibility.

## What is distilled

| Method | What it helps examine |
|---|---|
| Speech acts | Separate utterance content, the act performed, and its effects. |
| Infelicity and insincerity | Distinguish authority, procedure, sincerity, and subsequent performance. |
| Excuses and justifications | Ask whether a reason defends an act or reduces responsibility for it. |

These are selected, source-grounded methods, not a claim to cover the complete works. See [SKILL.md](SKILL.md) and [extraction notes](EXTRACTION.md) for scope and reasoning.

## Installation

This skill follows the open [Agent Skills](https://agentskills.io/) standard and can run in any skills-compatible AI agent runtime, including Claude Code, Codex, Cursor, OpenClaw, Hermes Agent, CodeBuddy, Workbuddy, Gemini CLI, OpenCode, and the broader ecosystem of 50+ runtimes.

### 1. One command

```bash
npx skills add jiushiaaa/austin-skill
```

The [Skills CLI](https://github.com/vercel-labs/skills) can detect supported agents. To select one, append `-a codex`, `-a claude-code`, or `-a cursor`; append `-g` for a global installation. Runtime support describes the standard and installer ecosystem, not a claim that we tested every runtime.

### 2. Manual installation

Clone this repository, then copy the complete folder into your runtime's skill directory, preserving `SKILL.md` and its relative reference paths. Name the installed folder `austin-perspective` to match its metadata. Common locations include `~/.agents/skills/` (Codex), `~/.claude/skills/` (Claude Code), and `~/.cursor/skills/` (Cursor); consult your runtime's current documentation.

```bash
git clone https://github.com/jiushiaaa/austin-skill.git
```

### 3. Use as reference

If automatic skill loading is unavailable, provide `SKILL.md` together with the referenced files needed for your question. Research notes remain in their source languages; README and usage guides are bilingual.

## Usage

- **Neutral analysis (default):** “Use J. L. Austin’s ideas to analyze this question. Distinguish source claims from contemporary applications.”
- **Persona expression (optional):** explicitly request “persona expression mode.” It is an acknowledged simulation, not a statement by the philosopher.

Fiction work uses the ideas while leaving narrative voice to the writing task. See the bilingual [usage guide](USAGE.md).

## Research sources

Selections from How to Do Things with Words; A Plea for Excuses; related ordinary-language analysis.

- [Source catalogue and reading ranges](references/research/source-catalog.md)
- [Method extraction and evidence](EXTRACTION.md)
- Opening quotation: <a href="https://sites.ualberta.ca/~francisp/NewPhil448/AustinPlea56.pdf">A Plea for Excuses</a>, ordinary-language discussion. English wording is translated where the source is not English; Chinese quotations are repository translations.

## Repository structure

Main files:

```text
├── SKILL.md  # Skill entry point and analysis methods
├── README.md / README.en.md  # Chinese and English introduction
├── USAGE.md  # Bilingual usage guide
├── EXTRACTION.md  # Method extraction and evidence
├── references/  # Research notes and optional expression mode
└── LICENSE  # MIT license
```

## Built with

Built with [nvwa-skill](https://github.com/alchaincyf/nuwa-skill).

Original project material is [MIT licensed](LICENSE); quoted works and translations retain their separate rights. See [source notices](ATTRIBUTION.md).

## More skills

Explore more thinkers and writers in the [Philosophy Skills collection](https://github.com/jiushiaaa/Philosophy-Skills).
