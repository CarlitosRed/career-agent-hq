# Context rules (copied in spirit from advance-po-reader notes, 2026-10-12)

1. One chat, one job, short life. A finished chat leaves a closing note in `OFFICE-STATE.md` and is retired.
2. Files hold the truth. A decision not written in `decisions.md` does not exist.
3. Raw dumps (voice, pasted CVs, job posts) go to `raw/` verbatim, never edited. Agents read the brief, not the dump.
4. Heavy reading (Codex memory, long repos, job boards) goes to a sub-agent that returns a short conclusion plus an evidence file.
5. Read only the section the step needs.
6. Checkpoint at ~60% context or when Carlos says "checkpoint": write `audits/handoff-<chat>-<date>.md` (open tasks, what was not checked, decisions not yet saved, next three actions), reply with the path only.
7. Codex is the memory and build agent; Claude is PM, reviewer and glue. Handoffs between them go only through files here.
8. Every explanation to Carlos comes with a visual; lead with the answer.

## Resume prompt (first message of any fresh chat)
"Read C:\Users\carlo\dev\career-agent-hq\OFFICE-STATE.md and CONTEXT-RULES.md, then AGENTS.md. You are <chat name>."
