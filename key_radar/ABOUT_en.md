# About KeyRadar

> This document is informational, not legal. For legally binding terms see [Terms of Service](./TERMS_en.md); for personal-data handling see the [Privacy Policy](./PRIVACY_en.md).
> **Version 0.5** (2026-06-03): User-created vault password removed. Vault identity clarified (local organization and monitoring store, not a secure safe). Automatic verification is limited to while the app is running. Aligned with policy v0.9.4.

## One-line summary
KeyRadar collects the API keys that AI coding tools scatter across your machine, then watches and records how they're used. It does not block.

## Why it exists
AI coding agents (Cursor, Claude Code, Copilot, and others) create `.env` files, ask for keys, or generate new ones project by project. The result is API keys spread across your PC. It becomes hard to know which key lives where, which keys still work, and which key suddenly started burning cost last week.

KeyRadar is a desktop tool that **collects those scattered keys locally**, **shows their state and usage at a glance**, and **flags anomalies**. KeyRadar is an *AI provider API operations dashboard*. It helps you discover, manage, verify, and monitor API keys scattered across AI services-all locally. It is not a password manager or vault replacement.

## What it does
- Scans folders you pick for `.env`-style files and shows candidates.
- Moves only the keys you approve into a locally encrypted vault.
- Never hard-deletes originals — keeps them in Safe Archive.
- Leaves a `.keyradar.md` coordinate file at the original path containing only references, no secrets.
- Shows the state of each key (alive / dead / requires admin key) and a usage trend.
- Detects anomalies like rapid burn and surfaces them.

## What it does not do (honest limits)
- **No cloud sync of your data.** Your API keys, vault contents, and project files are never transmitted to the operator's servers.
- **No KeyRadar account or signup.** Core key-management features work without a KeyRadar account. Mac App Store purchases are handled through Apple In-App Purchase.
- **It does not block usage.** KeyRadar is a turnstile, not a gate — it *records* who did what, but does not control who is allowed.
- **It cannot stop billing.** What happens inside a provider's payment system is outside its API and outside KeyRadar's reach. Its job is to alert you to rapid burn quickly enough that you can revoke or cap from the provider's console yourself.
- **Not a password manager.** The vault is a local organization and monitoring store. It is automatically available while the app is running and automatically locked when the app closes.

## Pricing
| Plan | Price |
|---|---|
| Lifetime (one-time) | $34.99 |
| Monthly subscription | $3.99 / month |
| Annual subscription | $29.99 / year |

A 3-day free trial starts automatically on first launch.

## Trial and purchase
- **Trial** — all features are available for 3 days from first launch.
- **Expired** — after the trial ends without purchase, vault access is blocked and menus are covered by a dimmed overlay. Registered key data remains on disk and is restored immediately after purchase.
- **Pro** — after purchase, all core features are available without restriction.
- **Payment processing** — Mac App Store purchases are processed by Apple In-App Purchase. Refunds and cancellations follow Apple App Store policies.

## Security model summary
- **At rest:** always encrypted. Plaintext keys never sit on disk.
- **In use:** decrypted briefly in memory at the moment a key is needed.
- **At supply (the weak link):** plaintext exists briefly. We minimize the exposure window with automatic `.gitignore`, timeout deletion, crash cleanup, and a full audit log.
- **In transit (between your PCs):** the vault is duplicated while still encrypted. We do not produce plaintext USB exports.

## The while-app-is-running limit (important)
Automatic verification and monitoring work only while the app is running. KeyRadar v1 does not provide a background resident process or LaunchAgent. When you close the app, automatic verification stops. We do not hide this limit.

## License and scope of responsibility
KeyRadar is a tool you use at your own discretion and risk. KeyRadar does not promise to block billing, prevent payment, or guarantee 100% prevention of key leakage. See [Terms of Service](./TERMS_en.md) for the full limitation of liability.

## Who built it
KeyRadar started from a real experience of overbilling and key sprawl while using AI development tools.

**Operator information**
- Business name: HAIB (sole proprietorship, registered in the Republic of Korea)
- Representative: Jaehoon Jung (정재훈)
- Business registration number: 461-13-02936
- Address: 310 Gaepo-ro, Gangnam-gu, Seoul, Republic of Korea
- Contact: support@hai-b.ai

## Contact and contributions
Issues and proposals go through the project repository. For security reports, use the dedicated channel described in the repository's SECURITY.md.
