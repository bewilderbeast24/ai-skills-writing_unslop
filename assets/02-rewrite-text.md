# Step: 02-rewrite-text

## Description
Rewrite the input text to eliminate the identified AI slop and replace it with natural, human-like language.

## Purpose
- Remove magic adverbs and overused AI vocabulary.
- Restructure sentences to avoid predictable AI patterns (e.g., negative parallelism, rhetorical questions).
- Flatten grandiose tone into direct, honest prose.
- Ensure the core message remains intact while the "slop" is removed.

## Pre-stage Checkpoint
### Version Control
- None required.

## Workflow
### Process
1. Use the analysis from [01-analyze-text.md](01-analyze-text.md) as a guide.
2. Replace overused words with simpler, more precise alternatives (e.g., "is" instead of "serves as").
3. Break up repetitive sentence structures (anaphora, tricolons).
4. Remove "filler" transitions (e.g., "It's worth noting").
5. Convert "Listicles in a Trench Coat" into genuine continuous prose.
6. Reword analogies to be specific and non-patronizing.
7. Tone down grandiose claims to match the actual significance of the topic.
8. Apply the principles in [writing-principles.md](../references/writing-principles.md).

### Output Format
- A draft of the "unsloped" text following [unsloped-text.md](../references/output-formats/unsloped-text.md).

## Post-stage Checkpoint
### Progress Tracking
- Update `.agents/skills-diary/unslop-ai/[<instance-name>]/checklist.md` by marking Stage 2 as completed.

### Version Control
- None required.

### Human in the Loop (HITL)
- Present the rewritten draft to the user.
- Ask: "Here is the first unsloped draft. Does this capture the original intent while feeling more human? Any specific sections you'd like me to adjust further?"

### Auto pilot
- If Autopilot is enabled, proceed directly to [03-verify-output.md](03-verify-output.md).
