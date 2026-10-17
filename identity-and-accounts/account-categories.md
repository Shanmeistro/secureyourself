# Account Categories

Tiering decides how much protection each account gets. Use aliases only. Related: [asset register](../threat-model/assets-and-impact.md).

| Tier | Examples (categories) | Minimum controls |
|---|---|---|
| **Tier 0 – Keystone** | Primary email, password manager, identity provider (Google/Apple/Microsoft), mobile carrier | Unique strong credential, strongest MFA available (hardware key preferred), offline recovery, tested recovery path |
| **Tier 1 – Critical** | Banking, government, health, cloud storage/backups, code hosting | Unique password, MFA (app or key, not SMS where avoidable), alerts on |
| **Tier 2 – Important** | Work accounts, messaging, social, shopping | Unique password, MFA where offered |
| **Tier 3 – Low** | Forums, one-off sign-ups | Unique password; consider deleting if unused |

## Review checklist (per account or category)

Use for [connected apps, sessions and recovery review](authentication-and-mfa.md#periodic-account-review-checklist). Record outcomes in `[PASSWORD MANAGER]` or a redacted note; not here.

| Category | Alias | Tier | MFA type | Recovery path | Last review | Status |
|---|---|---|---|---|---|---|
| Primary email | `[ACCOUNT ALIAS]` | 0 | `[Needs verification]` | `[RECOVERY METHOD STORED OFF-REPO]` | `[DATE]` | `Needs verification` |
| Password manager | `[PASSWORD MANAGER]` | 0 | `[Needs verification]` | `[RECOVERY METHOD STORED OFF-REPO]` | `[DATE]` | `Needs verification` |
| Financial | `[ACCOUNT ALIAS]` | 1 | `[Needs verification]` | `[...]` | `[DATE]` | `Not reviewed` |
