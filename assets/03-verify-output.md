# Step: 03-verify-output

## Description
Perform a final verification of the rewritten text to ensure all AI slop has been successfully removed and the result is polished.

## Purpose
- Ensure no new AI patterns were introduced during the rewrite.
- Verify that the text flows naturally and maintains a consistent, human tone.
- Confirm that the final output meets the standards in [final-verification.md](../references/final-verification.md).

## Pre-stage Checkpoint
### Version Control
- None required.

## Workflow
### Process
1. Read the rewritten text from [02-rewrite-text.md](02-rewrite-text.md) aloud (metaphorically).
2. Check for any remaining:
    - Em-dash addiction (more than 2-3 per piece).
    - Bold-first bullets.
    - Unicode decorations.
    - Fractal summaries (redundant conclusions/introductions).
3. Ensure the conclusion does not use "In conclusion" or similar signposts.
4. Verify that the tone is varied and imperfect (in a human way).

### Output Format
- The final, polished "unsloped" text following [unsloped-text.md](../references/output-formats/unsloped-text.md).

## Post-stage Checkpoint
### Progress Tracking
- Update `.agents/skills-diary/unslop-ai/[<instance-name>]/checklist.md` by marking Stage 3 as completed.

### Version Control
- If requested by the user, save the final output to a specified file.

### Human in the Loop (HITL)
- Present the final version to the user.
- Ask: "This is the final unsloped version. Are you satisfied with the result?"

### Auto pilot
- If Autopilot is enabled, output the final text and terminate the skill workflow.
