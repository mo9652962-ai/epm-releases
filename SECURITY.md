# Security Policy

## Supported Versions

| Channel | Naming        | Supported          |
| ------- | ------------- | ------------------ |
| Stable  | `v1.x.x`      | :white_check_mark: |
| Beta    | `v2.0.0-beta.x` | :white_check_mark: |

## Security Model & Boundaries

This repository is the **release distribution channel** for 墨题 · 英语刷题机
(an Electron desktop app). It contains only built installers and update
metadata — **no source code**.

1. **No Source Code:** Only release artifacts (installers, blockmaps, update
   manifests) are published here. Source lives in the
   [main repository](https://github.com/mo9652962-ai/english-multiple-choice-practice-machine).

2. **No Credential Storage:** No signing keys, tokens, or certificates are
   committed to this repository. Windows code-signing credentials are injected
   at build time from environment variables in CI and never persisted.

3. **Update Integrity:** Updates are distributed via `electron-updater` with
   checksum verification against the release manifest.

4. **Local-First Application:** The application itself runs fully offline by
   default and contains zero telemetry. See the main repository's `PRIVACY.md`.

## Reporting a Vulnerability

- Please **do not** create a public GitHub Issue.
- Submit details privately via GitHub Private Vulnerability Reporting.
- We will acknowledge receipt within 48 hours and provide a fix release within 7 days.
