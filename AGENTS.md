# Project instructions

This repository is the durable project memory for a credit-card channel, merchant settlement, and multi-level agent commission system.

## Continuity protocol

- When the user sends only `讀取` (or clearly uses it as a command), treat it as the project start shortcut:
  1. Check the Git working tree. If it is clean, run `git pull --ff-only`; if it is dirty, do not pull and report the local changes first.
  2. Read `docs/START_HERE.md` and `docs/CURRENT_STATUS.md`.
  3. Read `docs/REQUIREMENTS.md`, `docs/DECISIONS.md`, and `docs/OPEN_QUESTIONS.md` when product rules, accounting, permissions, payment status, or settlement are relevant.
  4. Reply with a concise summary of current progress, confirmed decisions, unresolved items, and the next recommended action.
- When the user sends only `儲存` (or clearly uses it as a command), treat it as the project handoff shortcut:
  1. Update `docs/DECISIONS.md` only with decisions explicitly confirmed in the current conversation.
  2. Update `docs/REQUIREMENTS.md` with new requirements and `docs/OPEN_QUESTIONS.md` with unresolved matters.
  3. Update `docs/CURRENT_STATUS.md` with work completed, changed files, blockers, and the next action.
  4. Review the pending diff for secrets, full PANs, CVVs, PINs, wallet private keys, and unredacted real transaction data; do not commit them.
  5. Commit the relevant project changes with a concise message and push to `origin/main`.
  6. Report the commit ID and whether the push succeeded. If the push is rejected, preserve all local work and explain the safe next step; never force-push automatically.
- At the start of a new conversation, or when asked to continue prior work, read `docs/START_HERE.md` and `docs/CURRENT_STATUS.md` first.
- Read `docs/REQUIREMENTS.md` for product scope, `docs/DECISIONS.md` for settled choices, and `docs/OPEN_QUESTIONS.md` before making assumptions that affect accounting, permissions, payment status, or settlement.
- Treat only entries in `docs/DECISIONS.md` as confirmed. Requirements marked tentative and all open questions remain unconfirmed.
- After material product or implementation work, update `docs/CURRENT_STATUS.md`. Add to `docs/DECISIONS.md` only when the user or project stakeholders explicitly confirm a decision.
- Use Asia/Taipei dates in `YYYY-MM-DD` format for project records.
- Keep documents concise and current; update an existing source-of-truth file instead of duplicating the same fact in several places.

## Security

- Never store production secrets, wallet private keys, full PANs, CVVs, PINs, or unredacted real transaction data in the repository.
- Prefer upstream-hosted payment pages or tokens so the application does not handle raw card data.
- Do not infer authorization to change external payment, merchant, wallet, or production systems.

## Document routing

- Product scope and behavior: `docs/REQUIREMENTS.md`
- Confirmed choices and rationale: `docs/DECISIONS.md`
- Unresolved choices: `docs/OPEN_QUESTIONS.md`
- Current work and handoff: `docs/CURRENT_STATUS.md`
- Terminology: `docs/GLOSSARY.md`
- Meeting summaries: `docs/meeting-notes/`

