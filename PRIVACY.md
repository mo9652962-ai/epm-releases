# Privacy Policy

**Last Updated:** 2026-10

This repository is the **release distribution channel** for 墨题 · 英语刷题机,
a local-first offline English practice desktop app. We uphold strict local-first
and zero-telemetry data protection principles.

## 1. Local Processing & Data Ownership

- The application runs **100% locally** on the user's machine.
- Practice history, vocabulary progress, and question-bank data **never leave
  the local environment** and remain the sole property of the user.
- This repository itself contains only built installers and update metadata —
  no user data of any kind.

## 2. Network Boundaries

- **Zero Telemetry:** No analytics SDKs, tracking pixels, crash beacons, or
  phone-home routines exist in the application or in this repository.
- The only outbound requests are **update checks** — anonymous, read-only queries
  to GitHub Releases (this repository) for the latest version manifest. No
  credentials, machine identifiers, or usage data are transmitted.
- Users on restricted networks may reach the same update metadata through a
  read-only mirror (`ghproxy.net`); no data is sent there either.

## 3. Credential Handling

- No API keys, signing certificates, or secrets are stored in this repository.
- Windows code-signing credentials are injected at build time from environment
  variables in CI and are never committed or distributed.

## 4. Contact & Disclosure

For security issues or questions regarding this policy, refer to
[SECURITY.md](SECURITY.md) or open an issue at
https://github.com/mo9652962-ai/english-multiple-choice-practice-machine
