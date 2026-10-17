# iPhone / iOS

Last reviewed: `[YYYY-MM-DD]` · Settings below are **targets, not confirmed**; each is `Needs verification` until checked. Menu names change between versions; confirm against the vendor's current documentation.

## iOS notes (reviewed `[DATE]`)

- Lockdown-style hardening is out of scope unless a specific threat justifies it.
- Check Settings for: passcode, Face/Touch ID, automatic updates, Find My, backup, app privacy report.
- If using iCloud backup, confirm what is covered and whether extra encryption is enabled (`Needs verification`).

## Common checklist

| Area | Target | Status |
|---|---|---|
| Screen lock and auto-lock | Strong PIN/passphrase (6+ digits at minimum; longer on desktop); auto-lock ≤ 1–2 min; biometrics optional | `Needs verification` |
| Updates | OS and apps update automatically; apply critical patches within days; retire devices that no longer get updates | `Needs verification` |
| Encryption and backup | Full-disk/device encryption on; encrypted backup tested via a restore | `Needs verification` |
| Find-my-device / remote wipe | Trade-off: helps recovery and wipe, but ties device to a cloud account and shares location with the provider. Decision: `[ENABLE/DISABLE]` | `Needs verification` |
| App permissions / installed apps | Review quarterly; remove unused; deny location, contacts, microphone unless needed | `Not reviewed` |
| Work/personal separation | Separate profiles/accounts; know what work MDM can see or wipe; don't enrol a personal device without understanding that | `Needs verification` |
| Public Wi-Fi | Prefer mobile data/hotspot for sensitive tasks; HTTPS everywhere; no sensitive logins on captive portals | `Not reviewed` |
| USB charging | Use own charger/cable or power-only; decline "trust this computer"/data prompts | `Not reviewed` |
| Lost-device response | Follow [lost-or-stolen playbook](../incident-response/lost-or-stolen-device.md) | `Implemented` (doc only) |
| Disposal / secure reset | Back up, sign out of accounts, remove from find-my, factory reset, verify wiped; see [device loss](device-loss-and-theft.md) | `Not reviewed` |

See also: [threat model](../threat-model/personal-threat-model.md).
