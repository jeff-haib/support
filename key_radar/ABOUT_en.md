# About KeyRadar

> This document is informational, not legal. For legally binding terms see [Terms of Service](./TERMS_en.md); for personal-data handling see the [Privacy Policy](./PRIVACY_en.md).
> **Version 0.3** (operator information confirmed + finalized prices/period)

## One-line summary
KeyRadar collects the API keys that AI coding tools scatter across your machine, then watches and records how they're used. It does not block.

## Why it exists
AI coding agents (Cursor, Claude Code, Copilot, and others) create `.env` files, ask for keys, or generate new ones project by project. The result is API keys spread across your PC. It becomes hard to know which key lives where, which keys still work, and which key suddenly started burning cost last week.

KeyRadar is a desktop tool that **collects those scattered keys locally**, **shows their state and usage at a glance**, and **flags anomalies**.

## What it does
- Scans folders you pick for `.env`-style files and shows candidates.
- Moves only the keys you approve into a locally encrypted vault.
- Never hard-deletes originals — keeps them in Safe Archive.
- Leaves a `.keyradar.md` coordinate file at the original path containing only references, no secrets.
- Shows the state of each key (alive / dead / requires admin key) and a usage trend.
- Detects anomalies like rapid burn and surfaces them.

## What it does not do (honest limits)
- **No cloud sync of your data.** Your API keys, vault contents, and project files are never transmitted to the operator's servers.
- **No accounts or signup.** Core key-management features work without an account. (Paid-license activation does involve Polar — see [Privacy](./PRIVACY_en.md).)
- **It does not block usage.** KeyRadar is a turnstile, not a gate — it *records* who did what, but does not control who is allowed (that belongs to the OS and to you).
- **It cannot stop billing.** What happens inside a provider's payment system is outside its API and outside KeyRadar's reach. Its job is to alert you to rapid burn quickly enough that you can revoke or cap from the provider's console yourself.
- **No backdoor recovery.** If you forget your master password, your vault cannot be opened. This is evidence that the lock is real — and also a real risk. We strongly recommend creating an encrypted export backup at the moment you set the password.

## Free trial and purchase
- **3-day free trial** — full features for 3 days after install. Trial records are stored only on your device (fully local). If KeyRadar detects traces of a prior installation on the same device, the trial is shortened to 1 day (abuse mitigation). This detection is not perfect and may be bypassed by OS reinstall or device change — stated honestly here.
- **One-time purchase** — not a subscription. A single purchase issues a license key and entitles you to updates for a defined period (see [Terms](./TERMS_en.md)).
- **Activation on up to 2 devices** — your license key may be activated on at most 2 devices. You can deactivate and re-register devices yourself through the Polar Customer Portal.
- **Payment processing** — Polar (merchant of record) handles payment and license issuance.

## Security model summary
- **At rest:** always encrypted. Plaintext keys never sit on disk.
- **In use:** decrypted briefly in memory at the moment a key is needed.
- **At supply (the weak link):** plaintext exists briefly. We minimize the exposure window with automatic `.gitignore`, timeout deletion, crash cleanup, and a full audit log.
- **In transit (between your PCs):** the vault is duplicated while still encrypted. We do not produce plaintext USB exports.

## The unattended-automation limit (important)
Modern AI agents run when you are not at the keyboard. To avoid blocking that automation, KeyRadar must allow the lock to open automatically (in Always-open mode, or during a session while session-lock is unlocked). **In that state, KeyRadar's encryption protects against off-device leakage but not against things that already have access to your machine.** We do not hide this limit — keeping it secret would be the dangerous choice.

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
