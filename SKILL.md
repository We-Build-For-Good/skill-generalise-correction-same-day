---
name: generalise-correction-same-day
description: When a human operator corrects an AI on a single product or file, immediately scan for that underlying assumption across all live proposals, drafts, and instructions in the same turn. Prevents the human from having to correct the same mistake twice. Includes scope classification (Universal, Contextual, Local).
license: MIT
metadata:
  author: We Build for Good
  version: "1.1.0"
---

# Generalise a Correction Same-Day: The Instant Immunity Protocol

The fastest way an AI collaborator loses human trust is **re-making a mistake after being corrected**.

When a human founder corrects an AI (e.g. "stop saying local-only is a benefit", "never put rings behind artwork", "do not use corporate buzzwords"), standard AI agents fix the immediate line of code and stop thinking. Hours later, the agent repeats the exact same flawed assumption on a different screen or proposal.

Having to give the same correction twice costs trust, patience, and momentum.

This protocol establishes the **Instant Immunity Rule**: when corrected once, the AI immediately asks *"Where else am I holding this belief?"* and removes it across all live drafts, specs, and prompts in the same turn.

---

## The Prime Philosophy

**A correction you have to give twice costs ten times more than one you never had to give.**

When a correction arrives:
1. Fix the immediate local line.
2. Identify the *underlying mental model or assumption* that produced the mistake.
3. Classify its scope (Universal, Contextual, or Local).
4. Sweep all in-flight drafts, specs, and system instructions to immunize the entire workspace.
5. Report the generalized rule back to the human operator in one line so they know they will never need to say it again.

---

## The Three-Tier Scope Classification

Not all corrections are universal. Blindly applying a local styling preference across an entire company is dangerous.

Every correction must be classified before sweeping:

### 1. Universal Scope (Company-Wide Invariant)
* **What it is**: Fundamental brand voice, privacy rules, safety boundaries, or non-negotiable coding hygiene (e.g. "never use em dashes", "never log customer passwords", "always check backup size").
* **Action**: Update global system instructions, add an automated grep check or linter rule, and sweep all active drafts across all repositories.

### 2. Contextual Scope (Product or Framework Specific)
* **What it is**: Specific to a single product, domain, or technology stack (e.g. "in this app, rings are always placed in front of images").
* **Action**: Codify into that specific project's `README.md`, `CLAUDE.md`, or standing rules. Do not leak into unrelated projects.

### 3. Local Scope (Session or Task Specific)
* **What it is**: A one-off aesthetic choice for a specific user request (e.g. "make this specific button purple for the demo").
* **Action**: Execute locally. Do not turn it into a permanent rule.

---

## The Sweep Procedure (Executed in the Same Turn)

When the human issues a correction:

1. **Acknowledge and Trace**: Identify the root belief.
   * *Example*: User says "Don't say our offline-first feature is about privacy; it is about reliability on trains."
   * *Root Belief*: The AI assumed offline storage is primarily a privacy feature.
2. **Scan In-Flight Memory**: Search all open drafts, pending PRs, and queued tickets for mentions of the flawed framing.
3. **Strip and Re-frame**: Update all affected documents in the same turn.
4. **Codify for Posterity**: If Universal or Contextual, append the rule to the project's standing instructions or memory ledger.
5. **Add Mechanical Verification (Where Feasible)**: If the rule is syntax or pattern based, add a simple pre-commit grep or linter rule (for example with skill-system-invariant-engine) so a repeat is caught automatically.
