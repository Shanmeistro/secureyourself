# Assets and Impact Register

Categories and aliases only. **No real email addresses, phone numbers, account IDs, or document numbers.**

Last reviewed: `[YYYY-MM-DD]`

| Category | Alias | Why it matters | Impact if lost/compromised | Impact scale | Controls documented in | Status |
|---|---|---|---|---|---|---|
| Primary email and identity providers | `[ACCOUNT ALIAS: PRIMARY EMAIL]` | Reset hub for most accounts | Cascading takeover | High | [email](../communications/email.md), [recovery](../identity-and-accounts/recovery-and-lockout.md) | `Needs verification` |
| Password manager | `[PASSWORD MANAGER]` | Holds nearly all credentials | Total credential exposure or lockout | High | [authentication](../identity-and-accounts/authentication-and-mfa.md) | `Needs verification` |
| MFA and recovery methods | `[MFA METHODS]`, `[RECOVERY METHOD STORED OFF-REPO]` | Last line of defence and last resort | Takeover or permanent lockout | High | [recovery](../identity-and-accounts/recovery-and-lockout.md) | `Needs verification` |
| Financial and government accounts | `[ACCOUNT ALIAS: FINANCE]` | Money, identity | Fraud, identity theft | High | [account categories](../identity-and-accounts/account-categories.md) | `Not reviewed` |
| Work accounts/devices | `[WORK ACCOUNT ALIAS]` | Employer data, livelihood | Disciplinary, data breach | Medium–High | [devices](../devices/linux-and-computers.md) | `Not reviewed` |
| Personal devices | `[DEVICE ALIAS]` | Hold sessions, data, 2FA apps | Account access, privacy loss | High | [devices/](../devices/iphone-ios.md) | `Needs verification` |
| Messaging and social accounts | `[MESSAGING ALIAS]` | Impersonation, scams of contacts | Reputation, harassment | Medium | [communications/](../communications/messaging-and-whatsapp.md) | `Not reviewed` |
| Personal photos/documents | `[PHOTO/DOC STORE ALIAS]` | Irreplaceable, private | Loss, extortion | High | [backup](../devices/device-loss-and-theft.md) | `Needs verification` |
| Professional reputation and public profiles | `[PUBLIC PROFILE ALIAS]` | Career, trust | Impersonation, doxxing | Medium | [public footprint](../privacy/public-footprint.md) | `Not reviewed` |

See the [threat model](personal-threat-model.md).
