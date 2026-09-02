# Clarify and Build (Clarify & Build Protocol)

An Antigravity & Agentic IDE Skill that unifies autonomous codebase fact-finding, dynamic decision tree traversal, sequential one-at-a-time A-D questioning, and concise execution-ready build prompt synthesis.

## Overview

When designing features, refactoring architecture, or clarifying specifications, developers often suffer from two extremes:
1. **The Over-Questioning Trap:** Agents asking endless open-ended questions, overwhelming the user with decision fatigue.
2. **The Assumption Trap:** Agents jumping into code prematurely based on unverified assumptions, causing massive rework and diff churn.

`clarify-and-build` provides a streamlined, zero-overhead alignment loop:
- **Silent Fact-Finding (AI Owns Facts):** The agent autonomously inspects existing files, types, routes, and tokens. It never burdens the user with trivia that can be grepped.
- **Sequential Dynamic Alignment (User Owns Decisions):** Open architectural decisions are queried strictly **ONE AT A TIME** with structured **A-D options** and an explicit agent recommendation (**"My pick"**).
- **Dynamic Tree Pruning:** Each user answer immediately reshapes the decision tree, pruning irrelevant downstream branches and preventing useless questions.
- **Build Prompt Synthesis:** Settled decisions are instantly compiled into a concise, concrete build prompt / implementation plan ready for immediate execution.

## Origins & Synthesis

This skill is a unified synthesis and architectural evolution of two foundational skills:
* **`grilling` (Antigravity Core / Gemini):** Provides the dynamic decision tree (frontier) model and the strict invariant that codebase fact-finding is the AI's autonomous responsibility.
* **`ask-then-build` (by David Ondrej):** Provides the low-cognitive-load, sequential single-question format (A-D multiple choice + recommended pick) and single-paragraph build prompt compilation.

## Installation

### Antigravity Global Skill
Place `SKILL.md` under your global skills directory:
```bash
mkdir -p ~/.gemini/config/skills/clarify-and-build
cp SKILL.md ~/.gemini/config/skills/clarify-and-build/SKILL.md
```

### Project-Specific Skill
Place `SKILL.md` under your workspace `.agents/skills/` directory:
```bash
mkdir -p .agents/skills/clarify-and-build
cp SKILL.md .agents/skills/clarify-and-build/SKILL.md
```

## Structure
- [`SKILL.md`](SKILL.md): Authoritative operational rules, workflow phases, formatting templates, and build prompt specifications.
