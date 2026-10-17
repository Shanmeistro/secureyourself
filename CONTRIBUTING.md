# Contributing

- **Small, reviewable changes.** One topic per commit or pull request.
- **No sensitive data.** See [SECURITY.md](SECURITY.md). When in doubt, leave it out.
- **Check staged diffs before committing:** `git status` then `git diff --staged`. `.gitignore` is not a safety net.
- **Prefer generic examples** and placeholders such as `[ACCOUNT ALIAS]`.
- **Update review dates** (and the status) whenever a procedure changes.
- **Mark unknowns** as `Needs verification` rather than assuming a setting is enabled.
- **No automation that changes real accounts or devices.** Do not add scripts that access or alter them.
- Every control should map to a plausible threat, impact or recovery need; avoid security theatre.
