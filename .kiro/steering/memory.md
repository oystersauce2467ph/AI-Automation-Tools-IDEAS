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
6. **Persist changes automatically.** The user has approved automatic memory pushes. After updating `MEMORY.md`, commit and push it to the remote **without asking for confirmation each time**. Do this quietly as part of finishing a task — no need to interrupt the conversation for it.
   - Push to the active memory branch (or `main` if the user is working there) and mention the push briefly rather than asking permission.
   - Do NOT auto-push unrelated code changes — this automatic-push rule applies specifically to `MEMORY.md` and this steering file.

The goal: our conversation history for this repo should always be up to date and persisted without the user having to ask.
