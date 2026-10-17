# Adversaries and Scenarios

Plain descriptions; no sensationalism. Part of the [threat model](personal-threat-model.md).

| Adversary | Typical capability | Typical goal | Most relevant controls |
|---|---|---|---|
| Mass phisher / scammer | Email/SMS/social messages, fake login pages | Credentials, payments | Password manager autofill, MFA, [phishing playbook](../incident-response/phishing-and-social-engineering.md) |
| Credential stuffer | Reused passwords from breaches | Account takeover | Unique passwords |
| Extortionist | Social engineering, screenshots, threats | Money, more material | [Sextortion playbook](../incident-response/sextortion.md) |
| Person known to me | Knowledge of habits/answers, possible past device access | Control, harassment | Change credentials from a trusted device; review sessions; [harassment playbook](../incident-response/harassment-and-impersonation.md) |
| Opportunistic thief | Physical device | Resale, account access | Lock, encryption, [lost-device playbook](../incident-response/lost-or-stolen-device.md) |
| Carrier social engineer | Convinces support to move a number | SMS codes | Carrier PIN/port lock; avoid SMS for critical MFA |
| Malicious app/extension | Over-broad permissions | Data theft | Permission review |

## Generic scenarios

1. Convincing "security alert" email leads to a fake sign-in page.
2. Phone stolen in a public place while unlocked.
3. Phone lost abroad; authenticator on it; no recovery codes accessible.
4. A new contact on a dating app pressures for intimate images, then threatens to share them.
5. Fake profile created using my public photos.
6. Public Wi-Fi captive portal or unknown charger used at an airport.
7. Credential committed to a repository by mistake.

Scenarios feed the [scenario table](personal-threat-model.md#4-scenario-register).
