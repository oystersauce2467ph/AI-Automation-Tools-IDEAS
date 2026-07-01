---
inclusion: always
---

# Memory Steering Rule

This repository maintains a persistent chat-history log at `MEMORY.md` (repo root).

## Always do the following

1. **At the start of every session**, read `MEMORY.md` to recall prior context. When the user references anything from past chats, answer using this file.
2. **Keep it current as we chat.** After any meaningful exchange — a decision, a request, a completed action, or a new follow-up — append or update the relevant dated entry in `MEMORY.md`. Do not wait to be reminded; treat memory updates as part of completing each task.
3. **Update the Quick Index table** at the top whenever a new dated entry is added.
4. **Use the entry template** at the bottom of `MEMORY.md` for consistency (Topic / What was discussed / Decisions made / Actions taken / Open items).
5. **Group by day.** Add turns under the existing entry for today's date; only create a new dated section when the date changes.
6. **Persist changes.** When appropriate, commit and push `MEMORY.md` so the history survives across sessions.

The goal: our conversation history for this repo should always be up to date without the user having to ask.
