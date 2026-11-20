SPDX-FileCopyrightText: 2026 LeeJSwit
SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0

# Security Policy

> Applies to L1 / L2 / L3 code and distributions on the `closure` branch.  
> Chinese: [SECURITY.md](SECURITY.md) (authoritative)

## 1. Supported Versions

Security fixes are provided only for the latest `0.1.x` release.  
Older versions, deleted branches, personal modifications, and third-party forks are not supported.

L3 has not been released; the L3 target page does not contain runnable code before 0.3.0.

## 2. Reporting a Vulnerability

Use GitHub private vulnerability reporting:

```text
https://github.com/LeeJSwit-HCN/arknights-mower/security/advisories/new
```

If that entry is unavailable, contact the maintainer through the GitHub profile. Do not open a public issue first.

Please include:

- affected version or commit;
- reproduction steps;
- impact;
- the minimum necessary logs or screenshots;
- your contact information (optional).

Do not submit:

- Skland tokens, API keys, account passwords;
- real account identifiers, UIDs, or phone numbers;
- unredacted `config/conf.yml`, logs, or screenshots;
- other people's data or account information.

## 3. What Is Not a Security Vulnerability

The following are not security vulnerabilities in this project:

- game account warnings, bans, freezes, or data deletion caused by using this project;
- game terms of service, platform rules, or official enforcement;
- malware, viruses, or spyware on the user's computer, phone, or emulator;
- a user posting tokens, API keys, configuration, logs, or screenshots in a public repository, issue, chat, or cloud storage;
- improper local permissions, shared accounts, weak passwords, or device loss;
- vulnerabilities or data breaches in third-party services (Skland, MAA, DeepSeek, GitHub, etc.);
- vulnerabilities in upstream mower code (report them upstream);
- social engineering, phishing, or impersonation of the maintainer;
- disputes arising from a user's breach of the license or terms of service;
- missing features, performance issues, compatibility issues, or usage questions.

## 4. Known Design: Plaintext Local Credentials

Skland tokens/credentials are stored in plaintext in local configuration (such as `config/conf.yml`). This is a known design for compatibility with upstream mower, not a newly introduced vulnerability.

Therefore:

- credential security depends on the user's device, operating system, and file permissions;
- token leakage caused by an compromised computer, shared configuration, or leaked logs/screenshots is the user's responsibility;
- this project does not proxy Skland login, collect tokens, or operate credential servers;
- if credentials may have leaked, change the Skland password, log in again, and delete the relevant configuration and logs immediately.

## 5. Maintainer Response Expectations

This is a personal hobby project, not a commercial product.

- no 24-hour response, SLA, or fixed remediation deadline;
- no bug bounty;
- response time may be delayed by work, personal life, or other maintenance;
- the maintainer will make a best effort to confirm, fix, and coordinate disclosure, but does not guarantee a fix;
- serious issues are prioritized;
- the maintainer may close reports that are not security issues and explain why.

## 6. Scope

This policy covers closure-added L1 / L2 / L3 code, scripts, packaging configuration, and related documentation.

Out of scope:

- `arknights_mower/` upstream code;
- third-party dependencies, MAA, ADB, emulators, Skland, model services;
- the user's own configuration, accounts, devices, network, and logs;
- the game client, game servers, and game accounts.

## 7. Coordinated Disclosure

Please allow reasonable time for confirmation and remediation, and do not publish full exploitation details before a fix is available.

To the extent feasible, the maintainer will:

- confirm the issue;
- assess impact;
- prepare a fix;
- credit the reporter in release notes if desired;
- coordinate public disclosure with the reporter.

Test in good faith. Do not access other people's accounts, data, or devices, and do not disrupt service availability.  
This policy is not legal advice and does not grant any legal immunity.
