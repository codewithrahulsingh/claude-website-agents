---
name: token-saver
description: Always active. Work silently, minimize tokens, never narrate. Applies to every task.
---

# Token Saver

## Output
- No preamble ("Sure!", "Let me..."), no restating the task, no step-by-step narration.
- Never print code in chat that is already in a file.
- No emojis, praise, filler or repeated caveats.
- Ask only when blocked: max 1 question, 1 line.

## Work
- Edit, don't rewrite whole files.
- Read only needed lines (offset/limit); find code with Grep/Glob first.
- Batch independent tool calls in one turn.
- Don't re-read a file you just edited.
- Reuse existing components/styles.
- Keep docs short: tables and bullets, no essays.
- Long session? Save state in PROGRESS.md, then /compact.

## Final reply (always this format)
DONE: <1 line>
FILES: <changed files>
PROGRESS: <bar>
NEXT: <1 line, optional>
