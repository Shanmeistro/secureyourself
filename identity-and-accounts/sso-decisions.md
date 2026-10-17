# SSO Decisions ("Sign in with Google / Apple / GitHub")

Last reviewed: `[YYYY-MM-DD]`. Use [templates/decision-record.md](../templates/decision-record.md) for each decision.

## Trade-offs

| Benefit | Cost (blast radius) |
|---|---|
| Fewer passwords; strong MFA on one provider | If the provider account is lost or compromised, every linked service is affected |
| Less credential exposure to small sites | Provider can suspend account → lockout everywhere |
| Fine-grained revocation of app access | Tracking/data sharing by the provider; Apple "hide my email" aliases complicate recovery |

## Selective-use policy (draft; `Needs verification`)

| Use SSO for | Avoid SSO for |
|---|---|
| Low-tier convenience services | Financial, government, password manager, primary email |
| Developer tooling tied to one identity (e.g., GitHub for code services) | Services I'd need if the provider locked me out |

Rules:
1. SSO provider accounts are Tier 0 and get hardware-key MFA and tested recovery.
2. Keep a **password-based fallback** (email + unique password) for important services where offered.
3. Review connected apps quarterly ([checklist](authentication-and-mfa.md#periodic-account-review-checklist)).
4. Avoid a single vendor ecosystem dependency: keep at least one non-provider route to each keystone account.

## Decisions log

| Service category | Decision | Date | Revisit trigger | Status |
|---|---|---|---|---|
| `[CATEGORY]` | `[SSO / password]` | `[DATE]` | provider change, incident | `Not reviewed` |
