# Ripple Capture Privacy Policy

**Effective date:** 2026-07-19 (draft)
**Version:** 0.1 (Mac App Store payments, local-only captures, no operator server, pre-legal-review)

## One-line summary
Ripple Capture does not transmit your **recordings, screenshots, GIFs, or screen content** to the operator (HAIB) or to payment infrastructure. All captures are processed locally on your device. Mac App Store payments are processed by Apple; Ripple Capture stores only local license metadata needed to unlock the app.

## 1. Scope
This policy describes how the Ripple Capture desktop app handles your data.

## 2. Information the operator collects directly
**None.** HAIB does not operate its own server to collect, transmit, or store:
- User-identifying information (name, email, IP address, etc.)
- Recordings, screenshots, GIFs, or other capture output
- Screen content or capture regions
- Usage statistics
- Telemetry or analytics
- Crash reports (no automatic submission)
- Behavior patterns

## 3. Information stored on your device
The following exists only on your local device and is not transmitted externally.

3.1 **Capture output (video, image, GIF)** — saved only as local files in a folder you choose (default `~/Movies/Ripple`). They are never uploaded or sent to the operator or any third party, and the operator cannot access them.

3.2 **App preferences** — accent color, language, cursor-effect strengths, chosen save folder, etc. Stored locally via macOS standard storage (UserDefaults) and app-scoped security bookmarks.

3.3 **Recent items (history)** — name/path references to recent capture files. Kept locally only; original files are not duplicated.

3.4 **Trial and license metadata** — license state (`trial` / `expired` / `pro`, etc.), trial start time, and purchase information. Stored locally and not transmitted outside your device.

## 4. Payments, license, and trial data
Ripple Capture processes Mac App Store purchases through Apple.

4.1 **At purchase** — Apple's App Store payment infrastructure handles payment details, receipts, and transaction information under Apple's policies. HAIB does not receive payment-instrument details such as card numbers.

4.2 **License verification** — Ripple Capture receives Apple StoreKit verification results and stores only the resulting local entitlement state.

4.3 **Free trial data** — Trial records are stored locally only, per §3.4. Ripple Capture does not track your device or account on a server to enforce the trial.

## 5. macOS permissions
Ripple Capture may request the following permissions to perform its function; these are used for real-time local processing only.

5.1 **Screen Recording** — used to record/capture the screen. Captured content is saved only as local files (§3.1) and is not transmitted externally.

5.2 **Accessibility (optional)** — detects click events to draw a ripple effect at the cursor position. It **does not capture keystrokes, input content, or the content of what you click**; it uses only coordinates, in real time, for effect rendering. Recording works without this permission; only the click-ripple effect is disabled.

## 6. Outbound communication
Ripple Capture communicates externally only with **Apple App Store infrastructure (purchase, restore, StoreKit verification)**. There is no other external communication — no usage-statistics transmission, remote logging, or operator server calls.

## 7. Deletion and transfer
7.1 **Deletion:** Capture output is managed and deleted by you in Finder. App preferences are removed on uninstall or by standard macOS means. Apple-side purchase records are managed through Apple.

7.2 **Uninstall:** Removing the app leaves the capture files you saved in their folder intact (to protect your content). Delete those files directly for complete removal.

## 8. Children's privacy
Ripple Capture is intended for general users and does not knowingly collect personal information from children under 13 (or as defined by applicable law).

## 9. Your rights (GDPR / Korea PIPA, etc.)
- **Information held by HAIB:** HAIB holds no personal information on its own servers.
- **Information held by Apple:** Purchase and transaction information is managed through Apple.
- **Local data:** Managed directly by you.

## 10. Security incident notification
Because HAIB does not directly hold user information, the risk of a data breach on HAIB's side is structurally limited. If a security vulnerability is found in Ripple Capture itself, we will announce it through the project repository and distribute a patch.

## 11. Changes to this policy
This policy may change; changes will be announced through the app or repository. In particular, we will update this policy before introducing any telemetry, crash reporting, HAIB-operated server, or new payment channel.

## 12. Contact and Data Protection Officer
For privacy inquiries, contact:

**Operator**
- Business name: HAIB (sole proprietor)
- Business registration no.: 461-13-02936
- Address: 310 Gaepo-ro, Gangnam-gu, Seoul, Republic of Korea

**Data Protection Officer**
- Name: Jaehoon Jung (also representative)
- Contact: support@hai-b.ai

Please submit rights requests to the contact above. Most requests are directed to local data management or Apple-side purchase management.

---

**Note:** This policy honestly reflects Ripple Capture's structure: local-only captures, Mac App Store payments handled by Apple, and no operator data server. Conformance to GDPR/CCPA/Korea PIPA standard templates requires review by a lawyer.
