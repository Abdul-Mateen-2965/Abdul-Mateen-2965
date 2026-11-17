# Prompt library

Two saved prompts. Copy the prompt, fill in the [brackets], send.

Files these prompts use (branch `claude/fable-5-2-setup-wixsca`):
- Playbook: https://github.com/Abdul-Mateen-2965/Abdul-Mateen-2965/blob/claude/fable-5-2-setup-wixsca/.claude/skills/fable-playbook/SKILL.md
- Rules: https://github.com/Abdul-Mateen-2965/Abdul-Mateen-2965/blob/claude/fable-5-2-setup-wixsca/CLAUDE.md

## Working style

### 1. Playbook
**When to use:** any task with more than one step, on any model, especially CV, job application or LinkedIn work.

**In Claude Code (file is already loaded):**
```
Use the fable-playbook skill for this task: [your task]. Before you start, tell me which steps of the playbook you are following.
```

**In the Claude app (no skill loaded):** open the Playbook link above, copy the whole file, then send:
```
Here is my playbook: [paste SKILL.md here]

Follow it for this task: [your task]. Before you start, write the Phase 1 plan in at most 10 lines and wait for my yes. Do one step at a time.
```

**A good answer looks like:** a plan of at most 10 lines starting with "Done means:", then one step at a time with a wait for your yes, and a final report that starts with the outcome and shows the proof.

### 2. My rules
**When to use:** the start of any new chat, so Claude follows your corrections from the first message.

**In Claude Code:** nothing to paste. `CLAUDE.md` loads by itself in this repo. To check it, send:
```
List my rules from CLAUDE.md in one line each, then do this task: [your task]
```

**In the Claude app:** open the Rules link above, copy the whole file, then send:
```
These are my rules. Follow all of them for this whole chat: [paste CLAUDE.md here]

First reply with a numbered one-line summary of the rules you will follow, then start on: [your task]
```

**A good answer looks like:** a numbered list of 15 one-line rules first, then the task done one step at a time, with no Power BI, no freelance suggestions, nothing removed and the Riyadh line kept.
