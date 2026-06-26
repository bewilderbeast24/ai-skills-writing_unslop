# unslop-ai

A professional-grade AI skill designed to transform predictable, AI-generated text into natural, human-like prose. `unslop-ai` systematically identifies and removes "slop"—the ornate vocabulary, repetitive sentence structures, and manufactured drama typical of Large Language Models.

## Overview

Modern AI often produces text that feels "off"—it's too polished, uses specific over-used words like "delve" or "tapestry," and relies on rhetorical crutches like "It's not just X, it's Y." `unslop-ai` provides a structured workflow to analyze these patterns and rewrite them using established human writing principles.

## Installation

To use this skill in any AI agent framework that supports `.agents/skills/` directories:

```bash
git clone https://github.com/bewilderbeast24/ai-skills-unslop_ai unslop-ai
```

## Core Features

- **Systematic Detection**: Identifies over 40 specific AI tropes across word choice, sentence structure, and tone.
- **Principled Rewriting**: Applies core human writing principles: specificity, directness, and structural variety.
- **Three-Stage Workflow**: Ensures quality through a rigorous Analysis -> Rewrite -> Polish sequence.
- **Operational Flexibility**: Supports both Human-In-The-Loop (HITL) for collaborative editing and Autopilot for automated processing.

## How It Works

The skill operates in three distinct phases:

### 1. Text Analysis
The agent scans the target text against a comprehensive [Slop Checklist](references/slop-checklist.md). It identifies "magic adverbs," overused vocabulary (e.g., "leverage," "robust"), and structural issues like negative parallelism or dramatic countdowns.

### 2. Unsloping Rewrite
Using the analysis report, the agent performs a surgical rewrite. It replaces abstractions with concrete details, varies sentence length, and removes manufactured suspense, following the [Writing Principles](references/writing-principles.md).

### 3. Final Polish
The rewritten text is validated against the original intent to ensure no meaning was lost while confirming that all AI-typical patterns have been eliminated.

## Usage

Once installed, you can invoke the skill by name. The skill expects a block of text as input.

### Execution Modes

- **Human-In-The-Loop (Default)**: The agent pauses after each stage, presenting its findings or drafts for your approval.
- **Autopilot**: The agent proceeds through all stages automatically. To enable, specify "Run on autopilot" in your request.

## Directory Structure

- `assets/`: Contains the specific prompts and instructions for each workflow stage.
- `references/`: The knowledge base of the skill, including slop checklists and writing principles.
- `SKILL.md`: The technical definition of the skill and its workflow.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
