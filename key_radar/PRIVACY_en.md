# KeyRadar Privacy Policy

**Effective date:** 2026-05-30 (draft)
**Version:** 0.3 (operator info confirmed, pre-legal-review)

## One-line summary
KeyRadar does not transmit your **API keys, vault contents, project files, or workspace contents** to the operator (HAIB) or to the payment processor (Polar). However, minimal license-related information is processed for paid-license activation and trial management (see §4).

## 1. Scope
This policy describes how the KeyRadar desktop app handles your data. The privacy practices of third-party providers you use (OpenAI, Anthropic, etc.) are governed by their own policies — KeyRadar does not control them.

## 2. Information the operator collects directly
**None.** HAIB does not operate its own server to collect, transmit, or store:
- User-identifying information (name, email, IP address, etc.) — except for information that Polar holds as part of the payment flow described in §4.
- API keys
- Vault contents
- Project files, source code, prompts
- Usage statistics
- Telemetry or analytics
- Crash reports (no automatic submission)
- Behavior patterns

## 3. Information stored on your device
The following exists only on your local device and is not transmitted externally.

3.1 **Encrypted vault (`vault.enc`)** — your registered API keys, stored under strong encryption (e.g., ChaCha20-Poly1305).

3.2 **Reference metadata (`refs/refs.json`)** — the mapping of which key applies to which project.

3.3 **Audit log (`audit.log`)** — a record of decrypt/supply events (who, when, which key). Visible only to you.

3.4 **Usage snapshots (`usage_daily.json`)** — daily cache of usage data fetched from providers.

3.5 **Safe Archive (`safe_archive/`)** — copies of original `.env` files (never auto-deleted).

3.6 **`.keyradar.md` coordinate files** — placed in your project folders. **They never contain key values** — only vault reference IDs and "managed by KeyRadar" metadata.

3.7 **Free-trial records** — trial start date and local markers used to detect a prior install on the same device. Not transmitted to the operator. (Bypassable via OS reinstall or device change — not a perfect abuse mitigation, stated honestly.)

3.8 **License key and activation status cache** — local cache of the license key you entered and the latest validation result. The key text itself is sent to Polar during activation and validation (§4).

## 4. Data related to payment, licensing, and free trial (handled by Polar)
For paid-license activation and validation, the following data is **processed by Polar (merchant of record)**. HAIB's own servers do not participate in this flow.

4.1 **At purchase (handled by Polar)**
- Payment information (card, billing address, etc.) — collected and held by Polar. HAIB does not receive card numbers or other payment instrument data.
- Buyer email — held by Polar. HAIB may view limited information (such as buyer email and license status) through the Polar dashboard for operational purposes (license issuance verification, customer support), but does not replicate or store this information in any HAIB-operated database.
- Transaction ID, receipts — held by Polar.

4.2 **At license activation / validation (KeyRadar calls Polar API)** — KeyRadar transmits the following to Polar's license endpoints:
- License key text
- Activation label (e.g., "MacBook Pro" — user-visible identifier)
- Activation metadata: a hashed device identifier for device-counting. (Polar may independently observe data such as IP at the connection level.)

4.3 **License information held by Polar**
- License key status (valid / expired / revoked)
- List of activation instances (label, meta, created_at)
- Validation count and last-validation timestamp
- Activation limit (up to 2 devices), expiration, etc.

4.4 **User self-management of licenses**
- Users can view and deactivate activation instances directly through the Polar Customer Portal.
- Refund and subscription-cancellation requests are handled through the Polar Portal.

4.5 **Free-trial data**
- Free-trial records are stored **locally only** as described in §3.7, and are not transmitted to operator servers.
- Detection of prior install on the same device is based on local markers and is not perfect.

4.6 **Polar's own privacy practices**
- Polar's handling of personal data is governed by Polar's policy (https://polar.sh). KeyRadar does not control Polar's processing.

4.7 **Commitment to update on future changes**
- At present, KeyRadar does not operate its own license or trial server. If HAIB later introduces an own-operated license server or trial verification server, this policy will be updated *before* such introduction and users will be notified.

## 5. Outbound network communication
KeyRadar communicates externally only in the following cases — none of them route through any operator-controlled server.

5.1 **To providers you registered** — calls to official endpoints for key validation and usage/balance lookup.

5.2 **To Polar** — calls to Polar's license endpoints for activation and validation as described in §4.

No other outbound communication. KeyRadar does not perform automatic updates, analytics submission, or remote logging.

## 6. Provider-side privacy
When KeyRadar makes a validation or lookup request, the relevant provider may log that request, your IP, or key-usage patterns according to their own policy. This is outside KeyRadar's control — consult each provider's privacy policy.

## 7. Deletion and portability
7.1 **Deletion:** Settings → "Erase All" removes your vault, refs, audit log, temporary supply artifacts, local license cache, and trial records. Removal of original `.env` files from Safe Archive is asked separately. Polar-side data (payment receipts, license records) is managed directly through the Polar Customer Portal.

7.2 **Portability (to another device):** the Export function produces an encrypted copy of your vault for transfer to another device. No plaintext export is offered.

7.3 **Uninstall:** uninstalling the app may leave local data files on disk. For complete removal, run Erase All first, or manually delete the app's data directory.

## 8. Children's privacy
KeyRadar targets general developers and does not knowingly collect information about anyone under 13 (or the relevant age under local law).

## 9. Your rights (GDPR / Korean PIPA / etc.)
- **Information held by HAIB:** HAIB does not hold personal data on its own servers, so no data subject to access, correction, deletion, portability, or processing-restriction requests exists on the HAIB side.
- **Information held by Polar:** Payment and licensing information described in §4 can be managed directly through the Polar Customer Portal. Rights requests may need to be directed to Polar.
- **Information held by providers:** Exercise your rights directly with each provider.
- **Local data:** Fully under your control.

## 10. Breach notification
Because HAIB does not directly hold user data, the structural risk of an operator-side breach is limited. However, if a security vulnerability is found in KeyRadar itself, it will be disclosed and patched through the project repository. Polar-side incidents follow Polar's own notification policy.

## 11. Changes to this policy
This policy may change, and updates will be announced in the app or the project repository. We will update this policy immediately if any of the following are introduced — telemetry/automatic updates/crash reporting, HAIB-operated servers, or change of payment processor.

## 12. Contact and Data Protection Officer
Privacy questions are received at the contact below.

**Operator**
- Business name: HAIB (sole proprietorship, Republic of Korea)
- Business registration number: 461-13-02936
- Address: 310 Gaepo-ro, Gangnam-gu, Seoul, Republic of Korea

**Data Protection Officer**
- Name: Jaehoon Jung (정재훈), concurrently serving as the representative
- Contact: support@hai-b.ai

Please send rights requests to the contact above. Note that, as stated in §9, because the Operator holds no personal data on its own servers, most requests will be redirected to local-data management or to processing through the Polar Customer Portal.

---

**Note:** This policy is written to honestly reflect KeyRadar's structure: "minimize direct collection by the operator, payment and licensing handled via Polar." Conformity with GDPR/CCPA/Korean PIPA standard formats and review of Polar's data-processing addendum (DPA) require legal counsel.
