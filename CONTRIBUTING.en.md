SPDX-FileCopyrightText: 2026 LeeJSwit
SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0

# Contributing Guide

> Chinese: [CONTRIBUTING.md](CONTRIBUTING.md) (authoritative)  
> This English translation is provided for reference. If the Chinese and English versions differ, the Chinese version prevails.

## 1. Sign the CLA First

Every code PR must first accept [CLA.md](CLA.md) ([English](CLA.en.md)). A PR without CLA acceptance does not enter merge review.

The maintainer must configure the repository secret `CLA_SIGNATURES_TOKEN` (contents: write). This is repository configuration and is not part of the CLA text.

Do not report security vulnerabilities in a public issue; report them privately according to [`SECURITY.en.md`](SECURITY.en.md).

The CLA covers only:

```text
L1: ui/src/riic/riic-sim/, ui/src/riic/sim/
L2: sim_bridge/, sim_api_bridge.py
L3: sim_bridge/autoschedule/, ui/src/riic/autoschedule/
other closure-added code directories expressly approved by the maintainer
```

## 2. Do Not Modify the Mower Core

The following do not accept external PRs:

```text
arknights_mower/
server.py
webview_ui.py
webui_zip.spec
ui/package.json
ui/package-lock.json
ui/.gitignore
ui/src/pages/Plan.vue
```

Submit changes to the mower core to the upstream project.  
The `closure` branch does not accept "while I was here, I also changed upstream" PRs.

## 3. Only L1/L2/L3 Code Is Accepted

- L1: simulation entities, skills, mood, production, orders, drones, power;
- L2: virtual clock, seams, headless execution, services, caches, regression;
- L3: scheduling optimization, candidate evaluation, and search (certification-related capabilities are not offered before 0.3.0);
- Documentation fixes may be submitted separately, but must not include commercial, boosting, or hosting functionality.

Not accepted:

- commercial-use features;
- boosting, account farming, hosting, paid interfaces;
- real-game integration tutorials;
- game memory modification, network interception, or client cracking;
- real account data, logs, screenshots, credentials, or personal information;
- features that evade detection or bypass restrictions.

## 4. File Headers

New closure files:

```text
SPDX-FileCopyrightText: 2026 LeeJSwit
SPDX-FileCopyrightText: 2026 <Contributor>
SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0
```

Each actual contributor keeps their own copyright line. Do not merge, overwrite, or add a line for a non-contributor. A file created only by LeeJSwit lists only LeeJSwit; when another contributor actually modifies or co-creates it, add that contributor's line.

When modifying MIT files:

- preserve the original copyright and MIT notice;
- do not add a PolyForm header;
- do not remove `LICENSE`, `NOTICE`, or `USER-NOTICE.md`.

## 5. Testing

Before submitting, run at least the focused tests related to the change:

```text
L1: focused vitest tests under ui/
L2: relevant sim_bridge pytest tests
L3: corresponding L3 tests
```

Do not submit tests that require a real game account, real device, or real data.

## 6. PR Requirements

- one PR should contain one kind of change;
- describe the scope, test results, and known limitations;
- do not include `arknights_mower/` changes;
- do not include commercial or boosting-related content;
- do not include unfinished feature entry points;
- do not include real credentials or personal data;
- pass the scope guard and CLA checks.

## 7. Project Positioning

This is a personal study and research project. It studies automated testing and scheduling algorithms for the open-source arknights-mower project in virtual-device and simulation environments.

The project does not provide tutorials or support for connecting code to a real game environment. Use of the project for violating game terms of service, commercial boosting, hosting, or other commercial purposes is prohibited.

## 8. License

- upstream MIT files remain MIT;
- new closure files are under PolyForm Noncommercial 1.0.0;
- commercial license requests are not accepted;
- contributing means agreeing to [CLA.md](CLA.md).
