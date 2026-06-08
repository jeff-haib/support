# Privacy Policy — HAIB Scrap Relay

_Last updated: 2026-06-01_

HAIB Scrap Relay ("the Extension," "we," "us") is a browser extension that helps you scrap, annotate, and relay content across AI tools. This policy explains what we do — and more importantly, what we do **not** do — with your data.

The short version: **we don't collect anything.** Everything stays on your device.

---

## 1. What We Collect

**Nothing on our servers.** We do not operate a server that collects, receives, or stores your data. We have no analytics backend, no tracking infrastructure, and no user database.

Specifically, the Extension does **not** collect, transmit, or store on any server controlled by us:

- The content you scrap (text, code, links, files, images)
- Your annotations or composed prompts
- Your browsing history
- Your IP address or device identifiers
- Cookies
- Usage analytics or telemetry
- Crash reports (no automatic transmission)

---

## 2. Where Your Data Lives

All data created or captured by the Extension is stored **locally on your own device**, in two places:

- **Browser storage** (IndexedDB and extension storage) — for in-app data (scraps, annotations, groups, settings).
- **Your local disk** — each scrap is automatically saved as an HTML file in `Downloads/ScrapRelay/` so the file is yours to keep, move, or delete as you wish.

- Your scraps, annotations, groups, and settings never leave your device. They are not sent to any server we operate.
- We cannot see, access, or recover your data. It is yours alone.
- If you uninstall the Extension, the in-app data stored by the browser is removed by the browser. Files already saved to your Downloads folder remain on disk — you can keep or delete them yourself.

---

## 3. When Data Leaves Your Device

There are only a few cases, and each happens **only on your explicit action**:

1. **Relay** — When you choose to relay content, the Extension inserts text into the input field of an AI page (Claude, ChatGPT, or Gemini) that you have open. The content goes to that AI provider under their own terms — not to us.

2. **Local file saves** — When you capture a scrap, the Extension automatically saves an HTML copy to your local Downloads folder (`Downloads/ScrapRelay/`). The file stays on your device. Nothing is uploaded.

3. **Pro license (if you purchase Pro)** — License activation and validation send your license key to our payment provider, **Polar** (see Section 5). This does not include any of your scrap content.

We do **not** auto-submit anything to AI providers. You always review and send manually.

---

## 4. Permissions We Use, and Why

- **storage** — to save your scraps, annotations, and settings locally.
- **sidePanel** — to display the main interface.
- **activeTab / scripting** — to capture content and insert relayed prompts, only when you click to do so.
- **tabs** — to detect whether a supported AI tab is open before relaying (we only read tab URLs to match supported domains; no history is collected).
- **contextMenus** — to provide right-click "Scrap" / "Annotate" options.
- **downloads** — to save each scrap as an HTML file to your local Downloads folder (`Downloads/ScrapRelay/`). Saving happens automatically when you capture, so the file stays on your disk for you to keep, move, or delete.

The Extension accesses only these AI sites: **Claude (claude.ai), ChatGPT (chatgpt.com / chat.openai.com), and Gemini (gemini.google.com).** It never requests access to all websites.

---

## 5. Third-Party Services

**Polar** (payments and license keys — Pro only)
If you purchase Pro, payment is processed by Polar, which acts as the **Merchant of Record**. Polar handles the transaction, billing, tax, and refunds. Your payment information is handled by Polar, not by us. License activation sends only your license key (not your content) to Polar for verification. Polar's handling of your data is governed by Polar's own privacy policy at polar.sh.

**Chrome Web Store / Microsoft Edge Add-ons** (distribution)
The Extension is distributed through these stores. Any data they collect (such as install counts or reviews) is governed by Google's and Microsoft's respective policies, not by us.

We use no other third-party services. No advertising networks, no trackers.

---

## 6. What We Do NOT Do

- We do not sell, rent, or share your data (we don't have it).
- We do not analyze or train on your content.
- We do not show advertisements.
- We do not automatically send anything to AI providers.
- We do not track your activity across sites.

---

## 7. Your Control

- All your data is on your device, under your control.
- You can export your data at any time (Markdown, JSON, and more).
- You can delete any or all of it at any time.
- Uninstalling the Extension removes its local data.

---

## 8. Children

The Extension is a general productivity tool not directed at children and does not knowingly collect any information from anyone, including children.

---

## 9. Changes to This Policy

We may update this policy as the Extension evolves. Material changes will be reflected in the "Last updated" date and, where appropriate, noted in the Extension's "What's new" section.

---

## 10. Contact

Questions about this policy or the Extension?

**Operator:** HAIB
**Representative & Data Protection Officer:** Jaehoon Jung
**Business Registration No.:** 461-13-02936
**Address:** 310 Gaepo-ro, Gangnam-gu, Seoul, Republic of Korea
**Email:** support@hai-b.ai

---

_HAIB Scrap Relay is an independent tool and is not affiliated with, endorsed by, or sponsored by Anthropic, OpenAI, or Google._
