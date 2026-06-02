# KeyRadar Terms of Service

**Effective date:** 2026-06-02 (draft)
**Version:** 0.5 (vault identity clarified, Mac App Store channel, 3-state license model, pre-legal-review)

> v0.5 (2026-06-03): User-created vault password removed. Vault identity clarified (local organization and monitoring store, not a secure safe). Automatic verification is limited to while the app is running. Aligned with policy v0.9.4.

## 1. Acceptance
By installing or running KeyRadar you are deemed to accept these Terms. If you do not accept them, do not use KeyRadar.

## 2. Nature of the service
KeyRadar is desktop software that runs entirely on your local device. The operator (HAIB, the "Operator") does not run its own server and has no ability to access your API keys, vault contents, project files, or workspace contents.

Mac App Store purchases are processed through Apple In-App Purchase. See the [Privacy Policy](./PRIVACY_en.md) for the data flow.

**Operator information**
- Business name: HAIB (sole proprietorship, registered in the Republic of Korea)
- Representative: Jaehoon Jung (정재훈)
- Business registration number: 461-13-02936
- Address: 310 Gaepo-ro, Gangnam-gu, Seoul, Republic of Korea
- Contact: support@hai-b.ai

## 3. Free trial
3.1 **Trial period — 3 days.** KeyRadar provides all features free of charge for 3 days from first launch.

3.2 **Automatic start.** The trial starts automatically on first launch. You do not need to opt in.

3.3 **Storage of trial records.** The trial start time and license state are stored locally in `license_meta.json` and are not transmitted to the Operator.

3.4 **Limits of trial enforcement.** This trial mechanism is local and tamper-evident, not server-enforced. It may be bypassed if a user completely deletes the vault directory and reinstalls the app. The short 3-day period is an intentional friction-based deterrent. You agree not to intentionally circumvent the trial limits.

3.5 **After trial expiration.** Once the trial ends without purchase, the app transitions to the Expired state described in §5.

## §4. Pricing and Payment

KeyRadar offers three plans:

| Plan | Price | Updates |
|---|---|---|
| Lifetime (one-time) | $34.99 | 2 years from purchase |
| Monthly subscription | $3.99 / month | During subscription |
| Annual subscription | $29.99 / year | During subscription |

All plans grant identical access to core features. Some extension features (plugins) may be sold separately or as separate subscriptions.

Payments are processed through the Mac App Store via Apple In-App Purchase. Refunds and cancellations follow Apple App Store policies.

## §5. License States

KeyRadar uses three license states:

(1) **Trial**: A 3-day trial automatically starts on first launch. All features are fully accessible during this period.

(2) **Expired**: The trial has ended and no license has been purchased. Existing key data remains on disk but is inaccessible until a license is purchased, at which point access is restored.

(3) **Pro**: A license has been purchased. All features are accessible without restriction.

## §6. Update Policy

**Lifetime purchase**: Updates are included for 2 years from purchase date. Major versions released after 2 years are outside the included update period and can require an upgrade price.

**Subscriptions (monthly/annual)**: All updates are included during the active subscription period. When the subscription ends, updates stop, and the installation transitions to the Expired state defined in §5.

**Plugins**: Some extension features (plugins) are sold separately or via separate subscriptions. The core app remains fully functional without plugins.

## §7. Vault and Key Storage

KeyRadar stores API keys in a local vault.
- The vault is automatically available while the app is running.
- The vault is automatically locked when the app closes.
- No separate vault password.
- The vault is not intended as a password manager or secure safe; it is a *local organization and monitoring* utility.

## 8. Your responsibilities
You agree to the following.

8.1 **Export files.** Export bundles and their passwords are yours to manage. Loss or leakage of a bundle or its password is your responsibility.

8.2 **The API keys themselves.** API keys are credentials issued to you by each provider (OpenAI, Anthropic, etc.) under that provider's own terms. You are responsible for all use, cost, and consequences arising from those keys.

8.3 **Lawful use.** You will use KeyRadar only for lawful purposes and will not use it in any manner that infringes the rights of others or violates applicable law.

8.4 **No trial abuse.** You will not intentionally circumvent the trial limits as described in §3.4.

## 9. What KeyRadar does NOT promise (scope of limitation)
The following are explicitly not promised.

9.1 **No promise to block billing or prevent payment.** KeyRadar detects and alerts on rapid-burn usage, but it cannot prevent actions inside a provider's payment system.

9.2 **No promise of complete leakage prevention.** While the app is running and the vault is automatically available, any process with access to the machine may also reach the key. KeyRadar does not control that.

9.3 **No agent control.** KeyRadar does not decide which apps or agents may use a key. That decision belongs to the OS and to you.

9.4 **No guarantee of provider-change adaptation.** If a provider changes its API, billing model, or policy, parts of KeyRadar may stop working.

9.5 **No 24/7 monitoring guarantee.** KeyRadar is a desktop app. Its monitoring and logging stop when your machine is off or the app is closed.

9.6 **No guarantee of App Store or StoreKit availability.** Purchases and restore operations depend on Apple's systems. The Operator is not responsible for temporary inability to purchase, restore, or validate due to Apple service availability, without denying any reasonable mitigation duty the Operator may have.

## 10. Limitation of liability
To the maximum extent permitted by applicable law, the Operator (HAIB) and its contributors are not liable for:

10.1 API charges or payments incurred while using KeyRadar.

10.2 Any damages arising from key leakage, loss, or misuse.

10.3 Indirect or consequential damages from errors, interruptions, or non-functioning features of KeyRadar.

10.4 Loss or leakage of export bundles or export passwords, and any consequences thereof.

10.5 Temporary inability to purchase, restore, or validate Pro status due to Apple service availability.

## 11. Disclaimer of warranties
KeyRadar is provided **"AS IS"** and **"AS AVAILABLE"** without warranties of any kind, express or implied, including but not limited to merchantability, fitness for a particular purpose, and non-infringement.

## 12. License (software use)
Use of the KeyRadar software is governed by the separate license file (LICENSE) and these Terms.

## 13. Changes to these Terms
These Terms may change. Material changes will be announced in-app or in the project repository. Continued use after a change constitutes acceptance of the changed Terms.

## 14. Governing law and disputes
These Terms are governed by the laws of the Republic of Korea. Disputes arising from these Terms shall be brought before competent courts in the Republic of Korea. (For global distribution, jurisdiction needs legal review.)

## 15. Contact
Questions about these Terms are received through the project repository or at support@hai-b.ai.

---

**Items deferred for later passes**
- §13 jurisdiction wording for global distribution — pending legal review
- Final form of the LICENSE file — pending decision (commercial / open-source)

**Recommended legal-review points:** Consumer-protection law in KR / EU / California, GDPR applicability, enforceability of liability limitations, and App Store policy consistency.
