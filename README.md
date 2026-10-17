# Personal Security Repository

> **⚠️ Never commit secrets or sensitive personal data.**
> No passwords, recovery codes, seed phrases, API keys, private keys, ID/permit scans, full phone numbers, home address, exact travel itineraries, or unredacted account identifiers. Use placeholders such as `[PASSWORD MANAGER]`, `[ACCOUNT ALIAS]`, `[RECOVERY METHOD STORED OFF-REPO]`. See [SECURITY.md](SECURITY.md).

## Purpose and scope

A **private-by-default**, documentation-first repository describing my security architecture, threat model, recovery procedures and periodic reviews across Apple, Android, Linux, online accounts, communications and travel.

- It documents **controls and procedures**. It is **not proof that any control is enabled**. Anything unconfirmed is marked `Needs verification`.
- It contains no scripts that access or alter real accounts or devices.
- Keep this repository private. Do not publish personal security details.

## How to navigate

| Need | Go to |
|---|---|
| Why do I do any of this? | [threat-model/](threat-model/README.md) → [personal-threat-model.md](threat-model/personal-threat-model.md) |
| What am I protecting? | [assets-and-impact.md](threat-model/assets-and-impact.md) |
| Accounts, MFA, recovery | [identity-and-accounts/](identity-and-accounts/account-categories.md) |
| Phones and computers | [devices/](devices/iphone-ios.md) |
| Email, messaging, social, dating | [communications/](communications/email.md) |
| **Something has gone wrong** | [incident-response/](incident-response/README.md) |
| Travel and public footprint | [privacy/](privacy/travel-privacy-kit.md) |
| Periodic reviews | [reviews/2026-q4-review.md](reviews/2026-q4-review.md), [templates/](templates/periodic-review.md) |

## Status legend

| Status | Meaning |
|---|---|
| `Not reviewed` | Not yet looked at |
| `In progress` | Work under way |
| `Implemented` | Confirmed in place (with non-sensitive evidence) |
| `Needs verification` | Believed true or planned, but not confirmed |
| `Retired` | No longer applicable |

## Monthly review checklist (about 15 minutes)

- [ ] Install pending OS and app updates on all devices.
- [ ] Confirm password-manager and backup access works (without writing anything secret down here).
- [ ] Review new sign-ins, sessions and security alerts on primary email and identity providers.
- [ ] Check no new forwarding rules or connected apps on primary email.
- [ ] Confirm recovery methods are still reachable (phone number, backup email, hardware key location).
- [ ] Review open items in the [threat model](threat-model/personal-threat-model.md) and update statuses.
- [ ] Run `git diff` / secret-pattern search to confirm nothing sensitive is in the repo.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).
