# Security Policy for This Repository

This repository is private and documentation-only. Its main risk is **accidentally storing sensitive data**.

## What must never be committed

- Passwords, passphrases, PINs, recovery codes, backup codes, seed phrases
- API keys, access tokens, private keys, certificates, session cookies
- Scans or photos of passports, permits, IDs, bank cards
- Full phone numbers, home address, exact travel itineraries
- Unredacted account identifiers, email addresses or usernames
- Intimate images or content of any kind (including as evidence; store evidence off-repo)
- Exports from password managers, authenticators or devices

Use placeholders and categories instead (for example `[ACCOUNT ALIAS]`).

## If sensitive information is accidentally committed

> Deleting a file in a later commit does **not** remove it from Git history.

1. **Revoke or rotate first.** Treat the value as compromised: change the password, revoke the token or key, regenerate recovery codes. Do this before cleaning up.
2. **Stop pushing** more commits until you have a plan.
3. **Remove from history if appropriate.** Rewrite history with a supported tool (for example `git filter-repo`), then force-push. If the repo was never pushed, rewriting locally may be enough.
4. **Check forks, clones and caches.** Review forks, other local clones, CI logs, pull requests, and any hosting-provider cached views. Ask the host to purge cached data where relevant.
5. **Review access.** Check who has or had access to the repository, and review account activity for the affected credentials.
6. **Record it.** Write a redacted entry using [templates/incident-log-redacted.md](templates/incident-log-redacted.md) (no secret values).

Rewriting history is not a substitute for step 1.

## Reporting issues with this repo

This is a personal repository; raise a private note or issue without including any sensitive value.
