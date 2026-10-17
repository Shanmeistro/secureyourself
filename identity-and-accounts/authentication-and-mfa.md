# Authentication and MFA

Last reviewed: `[YYYY-MM-DD]`. No MFA method is assumed to be configured; verify each.

## Password-manager operating rules

1. Every account gets a **unique** generated password; reuse is a finding.
2. Master credential: long passphrase, used only for `[PASSWORD MANAGER]`, never stored in this repo or in plain notes.
3. Enable MFA on the password manager itself.
4. Know how to recover it ([recovery](recovery-and-lockout.md)); test once.
5. Autofill only on exact domain matches; a manager that refuses to fill on a look-alike site is a phishing signal.
6. Don't store recovery codes in the same place as the thing they recover (see below).
7. Review the manager's health report (weak, reused, breached) monthly.
8. Least privilege: share items only through the manager's sharing features, and remove sharing when done.

## MFA strategy (ranked by strength)

| Method | Phishing-resistant? | Notes |
|---|---|---|
| Hardware security key (FIDO2/passkey) | Yes | Register at least two; keep one in a separate location |
| Passkeys on device | Yes | Check how they sync/recover; `Needs verification` |
| Authenticator app (TOTP) | No (codes can be phished) | Know how it is backed up or transferred |
| Push approval | Partly | Beware prompt fatigue; never approve unexpected prompts |
| SMS/voice code | No | Weakest; vulnerable to SIM swap. Use only if nothing else is offered |

Policy: Tier 0 and Tier 1 accounts ([categories](account-categories.md)) use the strongest method offered. Status for each: `Needs verification`.

## Recovery codes: location category only

Record **where category**, never the code. Examples of categories: `[PASSWORD MANAGER SECURE NOTE]`, `[PRINTED, HOME SAFE]`, `[PRINTED, TRUSTED PERSON]`. Don't keep the only copy inside the account it protects.

## Periodic account review checklist

For each Tier 0/1 account:

- [ ] Active sessions/devices: sign out ones I don't recognise
- [ ] Connected apps / OAuth grants: remove unused
- [ ] App passwords: remove unused
- [ ] Email forwarding rules and filters: none unexpected
- [ ] Recovery email/phone: current and still mine
- [ ] MFA methods: current, spare method exists
- [ ] Security alerts enabled
- [ ] Recent security events: anything unexplained → [account compromise playbook](../incident-response/account-compromise.md)
