# Device Loss and Theft (Preparation)

Response steps are in the [lost-or-stolen device playbook](../incident-response/lost-or-stolen-device.md). This page covers preparation.

## Prepare in advance

- [ ] Device list by alias only (`[DEVICE ALIAS]`), with whether each holds an authenticator or passkeys
- [ ] Find-my-device decision recorded (see [iOS](iphone-ios.md), [Android](android.md), [Linux](linux-and-computers.md))
- [ ] Lock-screen contact message that does not reveal personal details (`Needs verification`)
- [ ] Recovery codes / spare hardware key available without the lost device ([recovery](../identity-and-accounts/recovery-and-lockout.md))
- [ ] Carrier contact route known (stored in `[PASSWORD MANAGER]`, not here)
- [ ] Backups tested

## Decision: remote wipe

Wipe protects data but removes tracking and evidence of location, and is irreversible. Wipe when the device is confidently gone and sensitive data is not otherwise protected by encryption and a strong lock.

## Disposal / secure reset

1. Back up and verify the restore.
2. Sign out of cloud accounts and remove from find-my/device lists.
3. Remove SIM and SD cards.
4. Factory reset (encrypted devices: reset destroys keys).
5. Verify the device is at setup screen; then sell/recycle.
6. Remove it from the account device lists.
