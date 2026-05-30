# KeyRadar Terms of Service

**Effective date:** 2026-05-30 (draft)
**Version:** 0.3 (operator info confirmed + finalized values, pre-legal-review)

> ⚠️ Pre-legal-review draft. Have qualified counsel in your jurisdictions review it before public release.

## 1. Acceptance
By installing or running KeyRadar you are deemed to accept these Terms. If you do not accept them, do not use KeyRadar.

## 2. Nature of the service
KeyRadar is desktop software that runs entirely on your local device. The operator (HAIB, the "Operator") does not run its own server and has no ability to access your API keys, vault contents, project files, or workspace contents.

Paid-license activation and validation are performed via the payment processor Polar. See the [Privacy Policy](./PRIVACY_en.md) for the data flow.

**Operator information**
- Business name: HAIB (sole proprietorship, registered in the Republic of Korea)
- Representative: Jaehoon Jung (정재훈)
- Business registration number: 461-13-02936
- Address: 310 Gaepo-ro, Gangnam-gu, Seoul, Republic of Korea
- Contact: support@hai-b.ai

Because Polar (merchant of record) handles checkout, billing, tax compliance, and the consumer-facing seller role, the Operator does not separately file as a Korean 통신판매업자 (mail-order distance-selling business). (※ This clause will be updated if the sales structure changes.)

## 3. Free trial
3.1 **Trial period — 3 days.** KeyRadar provides all features free of charge for 3 days after installation.

3.2 **1 day if prior install is detected.** If traces of a prior KeyRadar installation are detected on the same device, the trial is shortened to 1 day. This is an abuse-mitigation measure.

3.3 **Storage of trial records.** The trial start date and prior-install markers are **stored locally on your device only** and are not transmitted externally.

3.4 **Limits of trial enforcement.** This trial-limit mechanism is based on local markers and is not perfect. It may be bypassed by OS reinstall, device change, or user-account change. You agree not to intentionally circumvent these measures in order to obtain repeated trials.

3.5 **After trial expiration.** Once the trial ends, some features may be restricted, and a license purchase is required to continue using them.

## 4. License and activation
4.1 **One-time purchase (primary launch model).** KeyRadar is primarily offered as a USD $24.99 one-time purchase (not an auto-renewing subscription). A monthly subscription at USD $3.99/month may also be offered as an alternative pricing option; if enabled, access to paid features continues while the subscription remains active. Unless explicitly enabled at checkout, the initial launch model is the one-time purchase.

4.2 **License key issuance.** After payment completes, Polar issues a license key.

4.3 **Activation limit — 2 devices.** A license key may be activated on up to **2 devices**. This limit is enforced via Polar's activation-limit feature.

4.4 **Device changes and deactivation.** When you need to deactivate an instance (device replacement, retirement, transfer), you can deactivate activation instances directly through the Polar Customer Portal. No separate operator approval is required.

4.5 **No transfer or sharing of license keys.** A license key is issued to the individual purchaser and may not be shared, transferred, or resold to third parties. Violations may result in license revocation by the Operator.

4.6 **Validation.** KeyRadar validates the license against Polar's endpoint at app startup (and periodically). If a license is revoked (refund, cancellation, etc.), paid features will be disabled.

## 5. Update entitlement
5.1 **Update period — 2 years.** A one-time purchase includes the right to receive updates for 2 years from the date the license is issued.

5.2 **After the update period.** After the update period ends, you may continue to use the features available at the time of purchase. To receive further updates, a new license purchase or a separate renewal policy (e.g., renewal discount) may apply.

## 6. Refunds
6.1 **Refund policy.** Refund requests must be submitted within **7 days** of purchase, via the Polar Customer Portal or the contact listed in these Terms.

6.2 **Refund processor.** Refunds are processed by Polar (merchant of record). The Operator approves refunds within Polar's policy.

6.3 **License upon refund.** After a refund, the license is revoked and paid features are disabled on all activated devices.

## 7. Your responsibilities
You agree to the following.

7.1 **Master password.** KeyRadar does not provide master-password recovery. If you forget it, there is no way to recover the keys stored in the vault. Password management and creating an export backup are entirely your responsibility.

7.2 **Export files.** Export bundles and their passwords are yours to manage. Loss or leakage of a bundle or its password is your responsibility.

7.3 **The API keys themselves.** API keys are credentials issued to you by each provider (OpenAI, Anthropic, etc.) under that provider's own terms. You are responsible for all use, cost, and consequences arising from those keys.

7.4 **Lawful use.** You will use KeyRadar only for lawful purposes and will not use it in any manner that infringes the rights of others or violates applicable law.

7.5 **No trial abuse.** You will not intentionally circumvent the trial limits as described in §3.4.

## 8. What KeyRadar does NOT promise (scope of limitation)

The following are **explicitly not promised.**

8.1 **No promise to block billing or prevent payment.** KeyRadar detects and alerts on rapid-burn usage, but it cannot prevent actions inside a provider's payment system (threshold charges, split retries, automatic settlement).

8.2 **No promise of complete leakage prevention.** In unattended-automation modes, while the lock is open automatically, any process with access to the machine may also reach the key. KeyRadar does not control that.

8.3 **No agent control.** KeyRadar does not decide which apps or agents may use a key. That decision belongs to the OS and to you.

8.4 **No guarantee of provider-change adaptation.** If a provider changes its API, billing model, or policy, parts of KeyRadar may stop working.

8.5 **No 24/7 uptime guarantee.** KeyRadar is a desktop app. Its monitoring and logging stop when your machine is off, locked, or the app is closed.

8.6 **No guarantee of Polar service availability.** License activation and validation depend on Polar's service. The Operator is not responsible for temporary inability to activate or validate due to Polar outages or policy changes (without denying any reasonable mitigation duty the Operator may have).

## 9. Limitation of liability
To the maximum extent permitted by applicable law, the Operator (HAIB) and its contributors are not liable for:

9.1 API charges or payments incurred while using KeyRadar.

9.2 Any damages arising from key leakage, loss, or misuse.

9.3 Indirect or consequential damages from errors, interruptions, or non-functioning features of KeyRadar.

9.4 Inability to access the vault due to lost master password, and any consequences thereof.

9.5 Temporary inability to activate or validate licenses due to Polar service issues.

## 10. Disclaimer of warranties
KeyRadar is provided **"AS IS"** and **"AS AVAILABLE"** without warranties of any kind, express or implied, including but not limited to merchantability, fitness for a particular purpose, and non-infringement.

## 11. License (software use)
Use of the KeyRadar software is governed by the separate license file (LICENSE) and these Terms. The license key follows a one-purchase-one-user (up to 2 devices) principle; third-party sharing or resale is prohibited (§4.5).

## 12. Changes to these Terms
These Terms may change. Material changes will be announced in-app or in the project repository. Continued use after a change constitutes acceptance of the changed Terms.

## 13. Governing law and disputes
These Terms are governed by the laws of the Republic of Korea. Disputes arising from these Terms shall be brought before competent courts in the Republic of Korea. (※ For global distribution, jurisdiction needs adjustment — confirm with counsel.)

## 14. Contact
Questions about these Terms are received through the project repository or at support@hai-b.ai.

---

**Items deferred for later passes**
- §13 jurisdiction wording for global distribution — pending legal review
- Final form of the LICENSE file — pending decision (commercial / open-source)

**Recommended legal-review points:** (a) Consumer-protection law in KR / EU / California, (b) GDPR applicability, (c) enforceability of §9 limitation, (d) scope of the §2 distance-selling-registration exemption under Korean law, (e) consistency between these Terms and Polar's merchant-of-record terms.
