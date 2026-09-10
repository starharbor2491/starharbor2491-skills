# starharbor2491-skills

Instruction files you drop into a chat tool or a project so the model answers like a person doing the work, with long grammatical sentences, few periods inside each bullet, and none of the cadence that reads as averaged internet.

## Folders

- `shared/base.md` is the rule list every folder assumes, including the ban on inventing cute names for these instructions.
- `conversation/` is for talk and replies.
- `coding/` is for patches, reviews, and programs.
- `research/` is for lookup with sources named.
- `writing/` is for drafts, edits, and page copy.

## Files in each job folder

- `AGENTS.md` is the tool-neutral file (Codex, Cursor-capable tools, Copilot coding agent, and anything else that looks for that name).
- `CLAUDE.md` is what Claude Code loads, and it pulls in `AGENTS.md` plus `shared/base.md`.
- `GEMINI.md` is what Gemini CLI looks for.
- `CURSOR.md` is a copy-shaped file for Cursor if you do not want to rely on `AGENTS.md` alone.

Root `AGENTS.md`, `CLAUDE.md`, `GEMINI.md`, and `.github/copilot-instructions.md` only tell a tool that this repository is a set of folders and that it should open the folder that matches the job.

## Use

Copy one job folder into the project you are actually working on (and copy `shared/` next to it so the relative `@` paths resolve), or paste `shared/base.md` plus that folder's `AGENTS.md` into custom instructions, and if the tool only reads a root `CLAUDE.md` then point that file at the folder with `@conversation/AGENTS.md` or the sibling path you chose.
