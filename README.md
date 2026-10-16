# Generalise a Correction Same-Day: The Instant Immunity Protocol

> **An open-source AI engineering protocol from [We Build for Good](https://webuildforgood.com)**  
> *Never make the human repeat a correction.*

---

## Overview

`generalise-correction-same-day` is an operational protocol for AI coding agents and human-AI pair programming workflows.

It solves the frustrating problem of AI amnesia: when you correct an AI model on a mistake in one file, it fixes that single line but repeats the exact same flawed assumption an hour later in another file or proposal.

This protocol mandates that whenever a correction is received, the AI immediately identifies the root belief, classifies its scope, and sweeps all in-flight drafts in the same turn.

---

## The Three Scopes

* **Universal**: Applies across all projects (e.g. brand voice, core privacy rules, critical security invariants).
* **Contextual**: Applies to one specific product or tech stack (e.g. design system rules for a specific app).
* **Local**: Applies only to the current prompt or line of code.

---

## Installation

### For Claude Code
```bash
git clone https://github.com/We-Build-For-Good/skill-generalise-correction-same-day.git ~/.claude/skills/generalise-correction-same-day
```

### For Cursor
```bash
mkdir -p .cursor/skills
git clone https://github.com/We-Build-For-Good/skill-generalise-correction-same-day.git .cursor/skills/generalise-correction-same-day
```

### For Antigravity / Open Agent Skills
```bash
mkdir -p .agents/skills
git clone https://github.com/We-Build-For-Good/skill-generalise-correction-same-day.git .agents/skills/generalise-correction-same-day
```

---

## License

MIT License. Developed and maintained by [We Build for Good](https://webuildforgood.com).
