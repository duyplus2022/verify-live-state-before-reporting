---
name: verify-live-state-before-reporting
description: Stop your agent from reporting "done", "live", or "broken" based on indirect signals. A verification discipline for AI agents: check the expected state first, verify on the live surface itself, and report only what was actually checked. Use before any status report, completion claim, failure alert, or re-run of a step that "already failed".
---

# Verify Live State Before Reporting (Lite)

Agents fail their users most often not by doing the work wrong, but by *reporting* it wrong: declaring a post live because the upload call returned success, declaring a machine broken because it did not answer, declaring access fine because it worked yesterday. This lite edition installs the core discipline. The full skill — free on Agensi, link at the bottom — adds the complete red-flag list, a worked example, and the reporting templates.

## Step 1 — Know the expected state before you judge

- Read the schedule, rule, or record that governs the thing you are checking. A machine with a known power window that is off *inside* that window is on schedule, not down.
- Name anything the user already disabled, parked, or switched off on purpose, and treat its silence as expected instead of raising it as a failure.
- Look up what you already recorded before asking the user anything. Do not make the user repeat themselves.

## Step 2 — Verify on the live surface

- Open the live URL, dashboard, channel, document, or posted item itself before saying it is live, up, or finished.
- Treat a saved credential, a successful API/upload response, or a session that worked earlier as a lead only — confirm the *current* session still reaches the live surface.
- Before re-doing anything reported as failed, check the destination first: the "failed" post may already be live, and re-running creates a duplicate.
- A single odd sighting is not a conclusion. A slow or blank page can look exactly like a logged-out state. Reload, wait for the full load, and check a second independent place (the profile page, the account menu) before concluding.

## Step 3 — Report only what you verified

- State the check you ran and what it showed: "I opened the published page and the video is public" — not "the upload succeeded, so it should be live".
- When a step is unverified, say so plainly and name the next check that would verify it.
- If a live check contradicts something you reported earlier, correct it in the same turn and name what the earlier claim got wrong.

## The one-line version

Expected state first, live surface second, report third — and never let an indirect signal speak for the thing itself.

## Full version

The complete skill is **free** on Agensi (worked example, full red-flag list, reporting templates): https://www.agensi.io/users/duylam
