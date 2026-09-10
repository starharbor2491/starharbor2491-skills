# starharbor2491-skills

Public instruction files anyone can download and paste into an agent.

Each `.md` file in each folder is the whole brief: you pick the job folder (`conversation`, `coding`, `research`, `writing`, or `shared` for the rule list with no job add-on), you pick the filename your tool already looks for (`AGENTS.md`, `CLAUDE.md`, `GEMINI.md`, `CURSOR.md`, `COPILOT.md`), you download that one file, you paste or drop it where the tool reads instructions, and you stop there, because nothing in this repo is an import, an `@` path, or a pointer at another file.

An agent that receives one of these files has only that file and the current thread: there is no private conversation behind the repo, and the human is whoever is speaking now.

Root copies of `AGENTS.md`, `CLAUDE.md`, `GEMINI.md`, `CURSOR.md`, and `COPILOT.md` are the conversation file again, so a clone of the repo root still gives a tool something usable without opening a subfolder.

`.github/copilot-instructions.md` is the coding file, because Copilot in this repo would be looking at instruction markdown rather than an application.
