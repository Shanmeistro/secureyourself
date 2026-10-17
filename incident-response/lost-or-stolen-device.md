# Lost or Stolen Device

[← Incident response index](README.md)

## 1. Trigger
A phone, laptop, tablet, key, or authenticator is missing.

## 2. Immediate priorities
1. Personal safety: do not confront a thief.
2. Protect accounts; the device may hold sessions and MFA.
3. Decide lock vs wipe.

## 3. First 15 minutes
1. Use find-my-device from a trusted device (only if previously enabled; `Needs verification`).
2. Enable lost mode/lock; display a contact message without personal details.
3. Change Tier 0 passwords (email, password manager, identity provider); sign out the lost device.
4. Call the carrier to suspend the SIM.

## 4. First 24 hours
1. Revoke sessions and tokens for the device across accounts.
2. Move MFA to a spare method; use recovery codes if the authenticator was on the device ([recovery](../identity-and-accounts/recovery-and-lockout.md)).
3. Decide on remote wipe (see [trade-off](../devices/device-loss-and-theft.md)).
4. Notify employer if it is work-related.
5. Report theft to police and request a report number if needed for insurance.

## 5. Recovery and verification
- Device removed from account lists and passkeys revoked
- New device set up from backup
- Check financial accounts for unusual activity
- Monitor for 30 days

## 6. Evidence to preserve
- Time/place last seen, device model alias
- Police report number
- Screenshots of location status (off-repo)

## 7. Who to contact
- Carrier; device vendor support; police
- Employer IT (work devices)
- Insurance or card providers if relevant

## 8. What not to do
- Don't go to retrieve it alone or confront anyone
- Don't wait to change keystone passwords
- Don't assume lock screen is enough
- Don't remote-wipe before checking if you need location evidence (if safe)

## 9. After-action review
Was the device encrypted, locked, and backed up? Were recovery codes reachable? Update [devices](../devices/iphone-ios.md) docs.
