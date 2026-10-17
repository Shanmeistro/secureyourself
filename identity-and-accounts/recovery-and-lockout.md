# Account Recovery and Lockout Prevention

Last reviewed: `[YYYY-MM-DD]`. The goal: never be locked out of keystone accounts, and never let an attacker use recovery against me.

## Recovery order (rebuild trust from the top)

1. **Phone/device access** (new SIM from carrier, or replacement device).
2. **Primary email** (Tier 0) via its recovery method.
3. **Password manager** via `[RECOVERY METHOD STORED OFF-REPO]`.
4. **MFA**: hardware key backup, recovery codes, re-enrol authenticator.
5. **Identity providers / SSO** (see [sso-decisions](sso-decisions.md)).
6. **Financial and government accounts**.
7. Everything else, using the password manager.

## Lockout prevention checklist

- [ ] Two independent MFA methods on every Tier 0/1 account
- [ ] Recovery codes generated and stored by category (not in the account they protect)
- [ ] Second hardware key registered and stored separately
- [ ] Recovery email/phone current; recovery email protected at the same level
- [ ] Trusted person or emergency-access arrangement considered (`Needs verification`)
- [ ] Carrier PIN / port-out protection set
- [ ] Recovery tested at least once a year without actually locking myself out

## Scenarios

| Scenario | First step |
|---|---|
| Lost phone with authenticator | Use recovery codes/hardware key; then [lost device playbook](../incident-response/lost-or-stolen-device.md) |
| Forgot password-manager master credential | Use its documented recovery; if none exists, this is a known gap |
| Number lost/SIM swapped | Contact carrier from a trusted device; secure email first; see [account compromise](../incident-response/account-compromise.md) |
| Hardware key lost | Use the spare; revoke the lost key; register a replacement |

## Warnings

- Recovery paths are attack paths: remove old numbers and emails.
- Don't write codes, answers or passwords in this repo.
