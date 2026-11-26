# Verify Live State Before Reporting — Lite (Free)

**Stop your AI agent from reporting "done", "live", or "broken" based on indirect signals.**

An agent skill (SKILL.md) for Claude Code, Cursor, and other AI agents that run real operations — posting, deploying, importing, messaging — and then have to tell a human what actually happened.

## Why this exists

The most expensive agent failures are reporting failures:

- "The video failed to post, please sign in again" — the account was never signed out; a slow page just looked like a login screen, and the "failed" video was already public. A re-post would have created a duplicate.
- "The server is down" — it was off inside its own scheduled power window.
- "Import completed" — the success message came from the tool, not from checking the data that actually landed.

Each one costs the user time, trust, or a duplicate they have to clean up.

## The discipline (3 steps)

1. **Expected state first** — check the schedule/rule/record before judging any signal.
2. **Live surface second** — open the thing itself; a success response, a saved session, or yesterday's access is a lead, not proof. One odd sighting is never a conclusion: reload, wait, check a second independent place.
3. **Report third** — state the check you ran and what it showed; say plainly what is still unverified.

## What's in this repo

- `SKILL.md` — the lite skill: the 3-step protocol in installable form. Copy it into your agent's skills folder and it applies the discipline before any status claim.

## Full version — free on Agensi

The complete skill adds the full red-flag list (rationalizations to refuse), a worked example, and reporting templates. It is **free**:

→ **https://www.agensi.io/users/duylam** (store: Duy Lam — look for "Verify Live State Before Reporting")

From the same store, for agents doing higher-stakes work: Safe Retention Cleanup (deletion guardrails), Multi-Account Browser Profiles (anti cross-posting), Live Database Import Guardrail (pre-flight import checks).

## Keywords

claude-code-skill · cursor-rules · ai-agent-skills · mcp-skills · agent-reliability · verification

## License

MIT — see `LICENSE`. The full version on Agensi is a separate listing (free).
