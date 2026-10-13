# Hermes Agent (Nous Research) installation - local or offline

Hermes is an open-source, local-first agent that keeps MEMORY.md and USER.md, reads SOUL.md for persona and loads skills in the open Agent Skills format. MINE's skills are already in that format. Docs: hermes-agent.nousresearch.com/docs (confirm exact paths and commands there; they change by version).

1. Install Hermes and run its setup (`hermes setup`). For fully offline use, point it at a local model server such as Ollama and choose a local Hermes model. Turn off or replace any web search provider you do not want online.
2. SOUL.md: use core/SOUL.md from this kit as the persona file.
3. MEMORY.md: Hermes injects it into every session and limits it to about 2,200 characters. Use core/HERMES_MEMORY.md (compact, under the limit). The long core/MEMORY.md is too big for this slot; keep it as a reference document.
4. USER.md: fill in core/HERMES_USER.md (about 1,375 characters max) about the person using the agent.
5. Skills: copy the skills/ folders (mine-mine, mine-grade, mine-refine, mine-forge, mine-move, plus creator skills) into Hermes' skills location, or use its /learn command on the folder.
6. Put the playbook PDF where the agent can read it (a local folder). Say: "Read START_PROMPT.md and report which files you accessed."
7. Run TEST_PROMPTS.md. Record real capabilities in core/CAPABILITIES.md.

Offline notes: the agent can only read files you give it. Anything that needs the web (links, search, docs) will not work offline. Hermes can write its own skills; review them before you trust them. Require approval before it sends, posts, pays or runs commands.
