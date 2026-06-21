---
name: writing-unslop
description: Use when you need to re-write AI-generated text to sound more human. It removes common "slop" patterns, ornate vocabulary, and predictable sentence structures.
---

## Skill Overview

The `unslop-ai` skill is designed to transform text that exhibits telltale signs of AI generation into natural, human-like prose. It uses a systematic approach to identify "slop" (overused AI tropes) and provides targeted rewriting instructions based on established human writing principles.

## Workflow Sequence

| Stage | Description | Workflow Asset | Input | Output |
| :--- | :--- | :--- | :--- | :--- |
| **1. Text Analysis** | Identify AI slop patterns and tropes in the target text. | [01-analyze-text.md](assets/01-analyze-text.md) | Target text | Analysis report |
| **2. Unsloping Rewrite** | Apply rewriting rules to remove slop and improve naturalness. | [02-rewrite-text.md](assets/02-rewrite-text.md) | Analysis report | Rewritten text |
| **3. Final Polish** | Verify the rewrite against human writing standards and style. | [03-verify-output.md](assets/03-verify-output.md) | Rewritten text | Final unsloped text |

## Pre-stage Checkpoint

### HITL / Autopilot 
Determine whether the user is asking for 'Execution on Autopilot' (only when specified) or 'Execution with Human In The Loop (HITL)' (default).

1. **Human in the Loop (HITL) Execution**: After each step, provide a clear handover (summary of findings/changes) and wait for user confirmation.
    
2. **Autopilot Execution**:
    - When execution on 'Autopilot' is explicitly requested, the agent will automatically proceed to the next stage after completing the current one.
    - Autopilot shall only apply to subsequent steps if requested mid-process.

## Core Operation Flow

### Progress Tracking
Before starting, ensure [checklist.md](references/checklist.md) is initialized and stored in `.agents/skills-diary/unslop-ai/[<instance-name>]/checklist.md`. After completing each stage below, you MUST update the checklist by marking the corresponding checkbox as completed (`[x]`).

### Stages

1. **Text Analysis**: Using the user provided input text, refer to [01-analyze-text.md](assets/01-analyze-text.md). Analyze the input text for specific slop patterns identified in [slop-checklist.md](references/slop-checklist.md).
2. **Unsloping Rewrite**: Using the analysis report from Stage 1, refer to [02-rewrite-text.md](assets/02-rewrite-text.md). Rewrite the text using the principles in [writing-principles.md](references/writing-principles.md).
3. **Final Polish**: Using the rewritten text from Stage 2, refer to [03-verify-output.md](assets/03-verify-output.md). Validate the rewritten text against the original intent and ensure all slop has been removed.

## Handover & Confirmation
- **No Placeholders**: All outputs must be final, ready-to-use text.
- **Verification**: The final output must pass the criteria in [final-verification.md](references/final-verification.md).
- **Handover**: Present the final "unsloped" text to the user for approval along with directory and file name in which it is saved.

## Additional Instructions

All temporary scripts generated while execution of skills (scripts which will be deleted after execution) will be written in `.agents/skills-diary/temp-scripts/<timestamp>/` as directory

