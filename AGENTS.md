# Project instructions

This repository is the durable project memory for a credit-card channel, merchant settlement, and multi-level agent commission system.

## Continuity protocol

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

