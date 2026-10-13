# Crimewallets — agent guidance

This repository contains a static list of public Solana wallet addresses and
alternative export formats. It does not contain private keys or a trading
runtime. Preserve the README's caution about attribution and false positives.

## Workflow

- On a VPS with /srv/shared/docs/AGENTS.md, read that master and STATUS.md first.
- Use your own clone and worktree. Branches are codex/<topic> or claude/<topic>.
- Keep main clean and integrate changes through a reviewed pull request.
- Use conventional commits and a Co-Authored-By trailer naming the acting agent.
- Keep credentials and runtime data outside the repository.
- For the coexistence pilot, change documentation only; preserve wallet lists,
  their ordering and export formats, the image, and the existing README.

## Validation and handoff

Run git diff --check. For future data changes, validate the affected format,
counts and consistency between exports; do not infer misconduct from a match.
Every modifying session writes docs/handoff/YYYY/MM/<UTC>-<agent>-<session>.md
with branch, checkout, commit, changes, validation and pending publication.
On the shared VPS also record a coordination event and read other open sessions.
