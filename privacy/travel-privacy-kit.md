# Travel Privacy Kit

Last reviewed: `[YYYY-MM-DD]`. Buy nothing without a use case. Needs and local rules vary; `Needs verification` for destination-specific laws. Don't put itineraries in this repo.

## Tier 1: Baseline

| Item | Threat addressed | Benefit | Limitation | Cost/effort | Use when |
|---|---|---|---|---|---|
| Updated phone/laptop | Known exploits | Patches | Doesn't fix user error | Low | Always |
| Strong PIN/passphrase, short auto-lock | Theft, shoulder surfing | Blocks casual access | Can be observed or coerced | Low | Always |
| Password manager + MFA | Account takeover | Unique credentials | Needs tested recovery | Low | Always |
| Minimal local data | Loss/theft/inspection | Less to lose | Less convenient offline | Low–Medium | Always; remove unneeded apps/files |
| Secure, tested backups | Loss, damage | Recoverability | Must be restored to be proven | Medium | Before every trip |

## Tier 2: Useful add-ons

| Item | Threat addressed | Benefit | Limitation | Cost/effort | Use when |
|---|---|---|---|---|---|
| Hardware security key (and a spare kept separately) | Phishing, lost authenticator | Phishing-resistant MFA | Can be lost; needs registered backup | Medium | Tier 0/1 accounts |
| Privacy screen | Shoulder surfing | Visual privacy | Narrow angle, no other protection | Low | Frequent public working |
| Reputable charger/cable | Unknown or faulty power sources | Avoids public ports | Doesn't protect other risks | Low | Public charging likely |
| Document pouch | Loss/theft of papers | Organised and secure | Physical security only | Low | Carrying physical documents (keep copies off this repo) |
| USB data blocker | Data/"juice jacking" over USB | Blocks data pins | Doesn't protect against every charging-related risk (e.g., a faulty charger, a malicious power source); not needed with own charger | Low | Charging from unknown ports without own adapter |

## Tier 3: Advanced / conditional

| Item | Threat addressed | Benefit | Limitation | Cost/effort | Use when |
|---|---|---|---|---|---|
| Separate travel device/profile | Device inspection, loss of main device | Less data exposed | Cost, upkeep, more to secure | High | A defined high-risk destination or event |
| Faraday pouch | Remote tracking/relay of a specific device/key fob | Blocks radio signals | Mostly niche; blocks calls; use case rarely exists for phones | Low–Medium | Only with a defined use case (e.g., keyless car fob) |
| VPN | Untrusted network, local network snooping | Encrypts traffic between you and the VPN | **Does not make you anonymous**; the VPN provider sees traffic metadata; doesn't stop phishing or malware | Low–Medium | Specific need such as untrusted Wi-Fi or region-specific issue; HTTPS already covers most web traffic |

## Pre-trip checklist

- [ ] Updates and backup done
- [ ] Recovery codes/spare key accessible without the travel device
- [ ] Find-my-device decision confirmed ([device-loss](../devices/device-loss-and-theft.md))
- [ ] Location sharing and posting plans: post after leaving
- [ ] Know [lost-device playbook](../incident-response/lost-or-stolen-device.md) steps
- [ ] Local emergency numbers: `[LOCAL EMERGENCY NUMBER]`
