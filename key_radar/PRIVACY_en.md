# KeyRadar Privacy Policy

**Effective date:** 2026-06-02 (draft)
**Version:** 0.5 (Mac App Store payments, local license metadata, vault identity clarified, pre-legal-review)

> v0.5 (2026-06-03): User-created vault password removed. Vault identity clarified (local organization and monitoring store, not a secure safe). Automatic verification is limited to while the app is running. Aligned with policy v0.9.4.

## One-line summary
KeyRadar does not transmit your **API keys, vault contents, project files, or workspace contents** to the operator (HAIB) or to payment infrastructure. Mac App Store payments are processed by Apple; KeyRadar stores only local license metadata needed to unlock the app.

## 1. Scope
This policy describes how the KeyRadar desktop app handles your data. The privacy practices of third-party providers you use (OpenAI, Anthropic, etc.) are governed by their own policies — KeyRadar does not control them.

## 2. Information the operator collects directly
**None.** HAIB does not operate its own server to collect, transmit, or store:
- User-identifying information (name, email, IP address, etc.)
- API keys
- Vault contents
- Project files, source code, prompts
- Usage statistics
- Telemetry or analytics
- Crash reports (no automatic submission)
- Behavior patterns

## 3. Information stored on your device
The following exists only on your local device and is not transmitted externally.

3.1 **Encrypted vault (`vault.enc`)** — your registered API keys. This is a local organization and monitoring store. The vault unlock secret is stored in the macOS Keychain (signed builds) or as a plaintext file (dev/unsigned builds, disclosed as a temporary fallback). In neither case is it transmitted externally.

3.2 **Reference metadata (`refs/refs.json`)** — the mapping of which key applies to which project.

3.3 **Audit log (`audit.log`)** — a record of decrypt/supply events. Visible only to you.

3.4 **Usage snapshots (`usage_daily.json`)** — daily cache of usage data fetched from providers.

3.5 **Safe Archive (`safe_archive/`)** — copies of original `.env` files, never auto-deleted.

3.6 **`.keyradar.md` coordinate files** — placed in your project folders. They never contain key values.

3.7 **Trial and license metadata (`license_meta.json`)** — license state (`trial` / `expired` / `pro`), trial start time, and purchase information. This data is stored locally with a tamper-evident HMAC signature and is not transmitted outside your device.

3.8 **No user password** — since users do not set a separate vault password, KeyRadar has no vault password to store, transmit, or recover. Export bundle passwords are one-time passwords chosen by the user for portability and are not stored by KeyRadar.

## 4. Data related to payment, licensing, and trial
KeyRadar uses Mac App Store purchases through Apple In-App Purchase.

4.1 **At purchase** — Apple App Store payment infrastructure processes payment data, receipts, and transaction information under Apple's policies. HAIB does not receive card numbers or other payment instrument data.

4.2 **License verification** — KeyRadar receives Apple's StoreKit verification result and stores the resulting local entitlement state in `license_meta.json`.

4.3 **Free-trial data** — trial records are stored locally only as described in §3.7. KeyRadar does not track devices or accounts to enforce the trial.

4.4 **Future direct-distribution channel** — if a non-App-Store direct channel is introduced later, its payment processor and data flow will be documented before launch.

## 5. Outbound network communication
KeyRadar communicates externally only in the following cases — none of them route through any operator-controlled server.

5.1 **To providers you registered** — calls to official endpoints for key validation and usage/balance lookup.

5.2 **To Apple App Store infrastructure** — purchase, restore, and StoreKit verification flows.

5.3 **Automatic verification scope** — provider key verification and usage monitoring work only while the app is running. When you close the app, automatic verification stops.

No other outbound communication. KeyRadar does not perform analytics submission or remote logging.

## 6. Provider-side privacy
When KeyRadar makes a validation or lookup request, the relevant provider may log that request, your IP, or key-usage patterns according to their own policy. This is outside KeyRadar's control — consult each provider's privacy policy.

## 7. Deletion and portability
7.1 **Deletion:** Settings → "Erase All" removes your vault, refs, audit log, temporary supply artifacts, local license metadata, and trial records. Removal of original `.env` files from Safe Archive is asked separately. Apple-side purchase records are managed through Apple.

7.2 **Portability:** the Export function produces an encrypted copy of your vault for transfer to another device. No plaintext export is offered.

7.3 **Uninstall:** uninstalling the app may leave local data files on disk. For complete removal, run Erase All first, or manually delete the app's data directory.

## 8. Children's privacy
KeyRadar targets general developers and does not knowingly collect information about anyone under 13 (or the relevant age under local law).

## 9. Your rights (GDPR / Korean PIPA / etc.)
- **Information held by HAIB:** HAIB does not hold personal data on its own servers.
- **Information held by Apple:** purchase and transaction information is managed through Apple.
- **Information held by providers:** exercise your rights directly with each provider.
- **Local data:** fully under your control.

## 10. Breach notification
Because HAIB does not directly hold user data, the structural risk of an operator-side breach is limited. If a security vulnerability is found in KeyRadar itself, it will be disclosed and patched through the project repository.

## 11. Changes to this policy
This policy may change, and updates will be announced in the app or the project repository. We will update this policy before introducing telemetry, crash reporting, HAIB-operated servers, or a new payment channel.

## 12. Contact and Data Protection Officer
Privacy questions are received at the contact below.

**Operator**
- Business name: HAIB (sole proprietorship, Republic of Korea)
- Business registration number: 461-13-02936
- Address: 310 Gaepo-ro, Gangnam-gu, Seoul, Republic of Korea

**Data Protection Officer**
- Name: Jaehoon Jung (정재훈), concurrently serving as the representative
- Contact: support@hai-b.ai

Please send rights requests to the contact above. Most requests will be redirected to local-data management, Apple-side purchase management, or the relevant provider.

---

**Note:** This policy is written to honestly reflect KeyRadar's structure: local-first user data, Apple-handled Mac App Store payments, and no operator-controlled data server. Conformity with GDPR/CCPA/Korean PIPA standard formats requires legal counsel.
