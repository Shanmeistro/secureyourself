# Personal Threat Model

Last reviewed: `[YYYY-MM-DD]` · Owner: `[ME]` · Status: `In progress`

> Generic seed content only. No personal details. Every "Existing control" is a **claim to verify** until marked `Implemented` with non-sensitive evidence.

## 1. Assets and why they matter

See [assets-and-impact.md](assets-and-impact.md). Highest value: primary email (reset hub for everything else), password manager, MFA/recovery methods, financial/government accounts, and personal photos/documents.

## 2. Adversaries and capabilities

Described plainly; see [adversaries-and-scenarios.md](adversaries-and-scenarios.md).

- **Opportunistic criminals:** mass phishing, credential stuffing, SIM-swap attempts, scams. Low skill, high volume.
- **Targeted scammers / extortionists:** social engineering, impersonation, sextortion. Motivated by money.
- **Known individuals** (ex-partner, acquaintance): may know personal details or have had device/account access.
- **Device thieves:** physical access to an unlocked or weakly locked device.
- **Malicious or compromised apps/services:** over-broad permissions, breaches at third parties.

## 3. Entry points and trust boundaries

| Entry point | Trust boundary |
|---|---|
| Email, SMS, messaging links | Untrusted sender → my attention |
| Public Wi-Fi, USB charging | Untrusted network/port → my device |
| App stores, browser extensions | Third-party code → my device/data |
| Account recovery flows | Support staff / phone carrier → my accounts |
| SSO providers | One provider → many accounts |
| Cloud backups | Provider → my data |
| Shared/borrowed devices | Other people → my sessions |

## 4. Scenario register

| Scenario | Asset at risk | Likelihood | Impact | Existing control | Gap | Next action | Status |
|---|---|---|---|---|---|---|---|
| Phishing captures primary email password | Primary email | Medium | High | Unique password, MFA (`Needs verification`) | Phishing-resistant MFA not confirmed | Evaluate hardware key for critical accounts | `Needs verification` |
| Credential stuffing from third-party breach | Any account | Medium | Medium | Password manager (`Needs verification`) | Reuse not audited | Run password-manager health report | `Not reviewed` |
| SIM swap / number takeover | SMS-based MFA and recovery | Low–Medium | High | `Needs verification` | SMS may be a recovery path | Prefer app/hardware MFA; set carrier port-out lock | `Not reviewed` |
| Lost or stolen unlocked phone | Device, accounts, photos | Medium | High | Screen lock (`Needs verification`) | Auto-lock and remote-wipe unconfirmed | Verify lock, encryption, find-my-device | `Needs verification` |
| Lockout (lost phone with only authenticator) | Account access | Medium | High | Recovery codes in `[OFFLINE STORAGE]` (`Needs verification`) | Recovery path untested | Test recovery order once | `Not reviewed` |
| Password manager master credential compromised or forgotten | All accounts | Low | Very high | `[RECOVERY METHOD STORED OFF-REPO]` | Emergency access not confirmed | Document and test recovery | `Not reviewed` |
| Malicious app / excessive permissions | Device data | Low–Medium | Medium | Store-only installs (`Needs verification`) | No periodic app review | Quarterly app and permission review | `Not reviewed` |
| Sextortion or intimate-image threat | Personal safety, photos | Low–Medium | High | [Playbook](../incident-response/sextortion.md) | Dating-app habits unreviewed | Review [dating-app safety](../communications/social-and-dating-apps.md) | `In progress` |
| Impersonation / fake profiles | Reputation | Low–Medium | Medium | [Playbook](../incident-response/harassment-and-impersonation.md) | Public footprint unchecked | Run [footprint review](../privacy/public-footprint.md) | `Not reviewed` |
| Insecure public Wi-Fi / USB charging while travelling | Device, sessions | Low | Medium | [Travel kit](../privacy/travel-privacy-kit.md) | Practices not confirmed | Adopt baseline kit | `In progress` |
| Secret accidentally committed to this repo | Credentials | Low | High | [SECURITY.md](../SECURITY.md), `.gitignore` | Staged-diff habit | Check diffs before commit | `Implemented` |
| Backup unavailable or unrecoverable | Photos, documents | Low–Medium | High | Backups (`Needs verification`) | Restore never tested | Test a restore | `Not reviewed` |

Likelihood/impact scale: Low / Medium / High. Likelihoods are rough judgements, not measurements.

## 5. Residual risk

After controls, residual risk is highest for: phishing against a tired or rushed user, loss of recovery methods, and targeted social engineering of a carrier or provider. Re-rate after each review.

## 6. Mitigations ranked by impact and effort

| Rank | Mitigation | Impact | Effort |
|---|---|---|---|
| 1 | Unique password per account via a password manager | High | Low |
| 2 | MFA on email, password manager, financial accounts; prefer app/hardware over SMS | High | Low–Medium |
| 3 | Tested recovery plan (offline recovery codes, second recovery path) | High | Medium |
| 4 | Screen lock, encryption, updates on all devices | High | Low |
| 5 | Tested backups | High | Medium |
| 6 | Hardware security keys (two) for critical accounts | High | Medium (cost) |
| 7 | Quarterly review of sessions, apps, forwarding rules | Medium | Low |
| 8 | Public footprint review | Medium | Low |
| 9 | Separate travel profile/device | Low–Medium | High |

## 7. Out of scope

- Nation-state or well-resourced targeted surveillance
- Compromise of hardware supply chains or firmware
- Legal compulsion and border-search strategy (seek specific advice if relevant)
- Physical home security and personal protection beyond emergency guidance
- Threats to other people's accounts/devices (family, employer systems beyond my own accounts)

## 8. Review triggers

Review this model when: new device; relocation; job change; account compromise or near miss; travel; major platform change (OS, password manager, email provider); end of a relationship that involved shared accounts/devices.
