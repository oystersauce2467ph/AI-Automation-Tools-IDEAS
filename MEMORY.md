# 🧠 MEMORY — Chat History Log

> **Purpose:** This file is the persistent memory for our work together in the **AI-Automation-Tools-IDEAS** repository.
> Kiro stores a running log of our conversations here. Whenever you ask about something from a past chat, Kiro will refer back to this file for context specific to this repo.

---

## How This Works

- Every meaningful conversation or decision gets recorded as a dated entry below.
- Each entry captures: **what was discussed**, **decisions made**, **actions taken**, and any **open items / follow-ups**.
- When you ask "what did we talk about before?" or reference a past request, Kiro reads this file first.
- This file is kept up to date **automatically** as we chat (enforced by `.kiro/steering/memory.md`), so you don't have to ask.
- You can still say **"update memory"** anytime to force an immediate save.

---

## Quick Index

| Date | Topic | Summary |
|------|-------|---------|
| 2026-07-01 | Memory system setup | Created this MEMORY.md to persist chat history for the repo. |
| 2026-07-01 | Push & auto-update | Committed/pushed MEMORY.md via PR #1; added steering rule to auto-update memory as we chat. |
| 2026-07-01 | Auto-push approved | Enabled automatic pushing of MEMORY.md updates without asking each time. |
| 2026-07-01 | Top 100 AI tools catalog | Built categorized Top 100 AI tools list (MD + CSV) and a directory-of-directories resource file. |
| 2026-07-01 | Enriched to Top 1000 roadmap | Added pricing/release/G2/MAU columns, deep profiles w/ hidden features, filtered sub-lists; reframed as Top 1000 (batched). |
| 2026-07-01 | Best-for + verified links | Added Best For/use-case & launch-month columns and HTTP-verified Website links; replaced dead PlayHT with Speechify. |
| 2026-07-01 | Filled G2 + MAU cells | Verified G2 ratings (corrected Perplexity/ElevenLabs/Tabnine); marked consumer apps n/a honestly; added disclosed MAU (Meta AI ~1B, Gemini ~350M+, Doubao). |

---

## Chat History

### 📅 2026-07-01 — Memory System Setup

**Topic:** Establishing persistent chat memory for this repository.

**What was discussed:**
- You asked me to generate a memory markdown file that stores and remembers our chat history for this specific GitHub repository.
- The goal: whenever you ask about something from past chats, I refer back to this Memory MD for context.

**Decisions made:**
- Created `MEMORY.md` at the repo root as the single source of truth for our conversation history.
- Adopted a dated-entry format with a quick-index table for fast lookup.

**Actions taken:**
- Created `MEMORY.md` with structure: purpose, usage guide, quick index, and chat history log.

**Open items / follow-ups:**
- None yet. Future conversations will be appended as new dated entries.

---

### 📅 2026-07-01 — Push to GitHub & Auto-Update Memory

**Topic:** Publishing the memory file and making it self-updating.

**What was discussed:**
- You approved committing and pushing `MEMORY.md` to GitHub.
- You then asked that all our chats already be reflected in memory, and that this be fixed so memory stays current as we chat longer.

**Decisions made:**
- Push `MEMORY.md` on a new branch and open a PR (rather than committing straight to `main`).
- Establish automatic memory upkeep via a steering rule instead of relying on manual "update memory" requests.

**Actions taken:**
- Created branch `add-memory-file`, committed `MEMORY.md`, pushed it, and opened [PR #1](https://github.com/oystersauce2467ph/AI-Automation-Tools-IDEAS/pull/1).
- Added `.kiro/steering/memory.md` (inclusion: always) instructing Kiro to read `MEMORY.md` at session start and keep it updated automatically after each meaningful exchange.
- Backfilled this conversation into the log so memory is fully current.

**Open items / follow-ups:**
- Merge PR #1 so `MEMORY.md` and the steering rule land on `main`. Until merged, they live on the `add-memory-file` branch.

---

### 📅 2026-07-01 — Automatic Memory Pushes Approved

**Topic:** Making memory persistence fully hands-off.

**What was discussed:**
- You approved letting me push `MEMORY.md` updates automatically, without asking for confirmation each time.

**Decisions made:**
- Auto-push applies specifically to `MEMORY.md` and the memory steering file — not to unrelated code changes.

**Actions taken:**
- Updated `.kiro/steering/memory.md` to commit and push memory updates automatically as part of finishing each task.
- Recorded this decision here and pushed to PR #1.

**Open items / follow-ups:**
- Merge PR #1 to land everything on `main`.

---

### 📅 2026-07-01 — Main Agenda: Top 100 AI Tools Catalog

**Topic:** Cataloging the most-used AI tools, classified by category (repo's core purpose).

**What was discussed:**
- You asked me to list websites/Excel sheets about different AI tools and classify them by category — ideally the top ~100 AI tools most people use today.

**Decisions made:**
- Deliver both a categorized reference (Markdown) and an Excel-ready CSV, plus a curated list of source websites/directories.
- Base rankings on current traffic data; exclude adult "companion" apps to keep it professional.

**Actions taken:**
- Researched current rankings (Exploding Topics Feb 2026, RankmyAI May 2026, a16z 6th ed.).
- Created `ai-tools/Top-100-AI-Tools.csv` — 100 tools with category, use, pricing, traffic, origin.
- Created `ai-tools/Top-100-AI-Tools.md` — 14 categories + overall Top 15 traffic table.
- Created `ai-tools/AI-Tool-Directories.md` — ranking sites, directories, model hubs, and roundups for refreshing the list.

**Open items / follow-ups:**
- Optional: add columns like G2 rating, mobile MAU, or API usage; auto-refresh monthly from sources.
- Optional: build filtered sub-lists (e.g., free-only, business-only, coding-only).

---

### 📅 2026-07-01 — Enriched Catalog + Top 1000 Roadmap

**Topic:** Expanding the AI-tools research per your follow-up requests.

**What was discussed:**
- You asked to: add columns (G2 rating, mobile MAU, launch year/release date); show free vs paid tiers with free-tier duration and each paid plan's cost/period; briefly describe each tool + main features + a separate "hidden features" section; include release dates; ensure no redundancy; and change the target from Top 100 to **Top 1000** ("my mistake before").

**Decisions made (and honest constraints I flagged):**
- Mobile MAU is rarely public -> shown as "—" rather than fabricated (only a few known values filled).
- "Hidden features" written only for tools I genuinely know (flagship tier), not invented for 1,000.
- 1,000 tools with all fields must be built in **batches**; this commit is Batch 1 (~100) with the full schema.
- Verified 2026 pricing for flagships via web search (ChatGPT, Gemini, Claude, Perplexity, Midjourney, GitHub Copilot, Cursor, ElevenLabs, Suno, etc.).

**Actions taken:**
- Created `ai-tools/AI-Tools-Master.csv` (new schema: Release, Pricing Model, Free Tier/Trial, Paid Plans, G2, Web Visits, Mobile MAU, Origin) for 100 tools.
- Created `ai-tools/Tool-Profiles.md` — deep profiles (description + main features + hidden features + release + pricing) for flagship tools.
- Created `ai-tools/Filtered-Lists.md` — free-tier / business / coding sub-lists.
- Created `ai-tools/README.md` — schema, categories, and roadmap to 1,000.
- Deleted redundant `Top-100-AI-Tools.md` and `Top-100-AI-Tools.csv`; fixed links in `AI-Tool-Directories.md`.
- Pushed to branch `ai-tools-catalog` (updates PR #2).

**Open items / follow-ups:**
- Batches 2-7: expand toward 1,000 tools (category-balanced, deduped).
- Optional: verify/fill more G2 ratings and any newly-public mobile MAU figures.
- Monthly refresh of pricing and rankings.

---

### 📅 2026-07-01 — Best-For, Launch Months & Verified Website Links

**Topic:** Adding use-case column, launch months, and working website links to the catalog.

**What was discussed:**
- You asked to add a "Best for"/use-case column, fill launch-month where only a year existed, and add a Website link per tool that actually works (no broken links).

**Actions taken:**
- Added `Best For / Use-Case` and `Website` columns to `AI-Tools-Master.csv`; filled launch months where reliably known.
- HTTP-checked all 100 website URLs with curl (browser user-agent, following redirects). Most 200; some big brands return 403 to bots but work in-browser.
- Fixed dead links: **PlayHT shut down (Dec 2025)** -> replaced with **Speechify**; Adobe Firefly -> `firefly.adobe.com`; Adobe Express -> `express.adobe.com`.
- Properly quoted CSV fields containing commas so columns don't break in Excel.
- Hyperlinked tool names in `Tool-Profiles.md`; updated `README.md` schema + link-verification note.

**Open items / follow-ups:**
- Continue batches toward 1,000; re-verify links periodically (tools rebrand/shut down).

---

<!--
MEMORY ENTRY TEMPLATE (copy for new entries):

### 📅 YYYY-MM-DD — <Short Topic Title>

**Topic:** <one-line description>

**What was discussed:**
- ...

**Decisions made:**
- ...

**Actions taken:**
- ...

**Open items / follow-ups:**
- ...
-->
