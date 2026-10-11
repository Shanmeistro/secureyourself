# Account Compromise

[← Incident response index](README.md)

## 1. Trigger
- Unexpected password-reset, MFA prompt, or sign-in alert
- Messages sent that I didn't send; settings changed; locked out

## 2. Immediate priorities
1. Regain control of the **keystone** account (primary email first).
2. Cut off the attacker's sessions.
3. Protect money and other linked accounts.

## 3. First 15 minutes
1. Use a **trusted device** and network.
2. Change the password (new, unique, from `[PASSWORD MANAGER]`).
3. Sign out all sessions/devices.
4. Check/remove forwarding rules, filters, recovery email/phone, app passwords.
5. Re-check MFA methods; remove ones that aren't mine.
6. If locked out: start the provider's recovery and see [recovery](../identity-and-accounts/recovery-and-lockout.md).

## 4. First 24 hours
1. Work through other accounts in [recovery order](../identity-and-accounts/recovery-and-lockout.md).
2. Contact banks if financial accounts may be affected.
3. Scan the device for unknown apps/profiles; consider a reset if unsure.
4. Warn contacts out-of-band if impersonation is likely.
5. Review connected apps and sessions everywhere ([checklist](../identity-and-accounts/authentication-and-mfa.md#periodic-account-review-checklist)).

## 5. Recovery and verification
- Sign-in history is clean and only my devices remain
- No unknown forwarding rules/recovery methods
- Password-manager health report shows no reuse
- Monitor alerts for 30 days

## 6. Evidence to preserve
- Screenshots of alerts and sign-in history (no passwords)
- Timestamps, provider ticket numbers, redacted
- Keep the original phishing message if there was one

## 7. Who to contact
- The provider's account-recovery / security support
- Bank or card issuer for financial exposure
- Carrier if SIM swap suspected
- Employer security team if a work account is involved
- Local police/fraud reporting for financial loss or identity theft (`[LOCAL REPORTING SERVICE]`)

## 8. What not to do
- Don't reply to the attacker or pay
- Don't use the compromised device to reset others
- Don't reuse the old password or a variation
- Don't delete evidence before capturing it
- Don't trust 'recovery' offers from strangers

## 9. After-action review
Record cause, detection time, what worked, and what control failed. Update the [threat model](../threat-model/personal-threat-model.md) and status entries. Use the [incident log](../templates/incident-log-redacted.md).
