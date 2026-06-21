# Step: 01-analyze-text

## Description
Analyze the provided input text to identify common AI "slop" patterns, including specific word choices, sentence structures, and tonal issues.

## Purpose
- Identify specific instances of AI tropes.
- Categorize the types of slop present (e.g., word choice, sentence structure, tone).
- Create a roadmap for the rewriting stage.

## Pre-stage Checkpoint
### Version Control
- Ensure you have the original text clearly identified.
- No git commands are strictly necessary for text analysis unless the text is stored in a file you intend to track.

## Workflow
### Process
1. Read the input text thoroughly.
2. Cross-reference the text with the [slop-checklist.md](../references/slop-checklist.md).
3. Identify occurrences of:
    - Magic adverbs (e.g., "quietly", "deeply").
    - Overused AI vocabulary (e.g., "delve", "leverage", "robust").
    - Ornate nouns (e.g., "tapestry", "landscape").
    - Negative parallelism ("It's not X -- it's Y").
    - Rhetorical questions ("The result? Devastating.").
    - Listicles in prose.
    - Grandiose stakes inflation.
4. List the identified patterns and their locations in the text.

### Output Format
- Follow the structure in [analysis-report.md](../references/output-formats/analysis-report.md).
- Ensure specific examples from the text are included for each category.

## Post-stage Checkpoint
### Progress Tracking
- Update `.agents/skills-diary/unslop-ai/[<instance-name>]/checklist.md` by marking Stage 1 as completed.

### Version Control
- None required for this analysis step.

### Human in the Loop (HITL)
- Present the analysis summary to the user.
- Ask: "Would you like me to proceed with the rewrite based on this analysis, or should I look for other specific patterns?"

### Auto pilot
- If Autopilot is enabled, proceed directly to [02-rewrite-text.md](02-rewrite-text.md).
