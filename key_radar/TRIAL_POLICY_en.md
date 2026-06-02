# KeyRadar Trial Policy v0.5

> v0.5 (2026-06-03): User-created vault password removed. Vault identity clarified (local organization and monitoring store, not a secure safe). Automatic verification is limited to while the app is running. Aligned with policy v0.9.4.

This document supplements [Terms of Service](./TERMS_en.md). The Terms prevail in case of conflict.

## 1. Trial Period

A *3-day* free trial automatically starts on first launch. Users do not need to opt in to start the trial.

## 2. Trial Access

During the trial, all features are accessible identically to a Pro license holder.

## 3. After Trial Expiration

If 3 days pass without a license purchase:
- The app transitions to the Expired state.
- Vault access is blocked, and all menus are covered by a dimmed overlay.
- Registered key data remains on disk. Access is restored immediately upon license purchase.
- Only the purchase button (top-right of the topbar) remains active.

## 4. Trial Bypass Prevention

KeyRadar stores the trial start time in a local file (`license_meta.json`) with HMAC signature. The file is tamper-evident, but a user who completely deletes the vault directory and reinstalls the app can restart the trial.

This is an intentional policy:
- No device identifier tracking (privacy minimization policy alignment)
- No additional permissions like iCloud required
- Operates entirely within the App Sandbox

The 3-day trial length itself creates an unreasonable friction cost for reinstall-based bypass attempts.

## 5. Trial Notifications

The following notifications are shown:
- On first launch: "Your 3-day free trial has started" modal
- 1 day before expiration: Toast notification
- At expiration: Purchase modal automatically displayed
