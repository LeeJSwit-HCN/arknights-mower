SPDX-FileCopyrightText: 2026 LeeJSwit
SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0

# Closure Contributor License Agreement (CLA)

> Version: 1.1  
> Scope: L1 / L2 / L3 code contributions to the `closure` branch.  
> This English version is provided for reference. If the Chinese and English versions differ, the Chinese version prevails.

## 1. Scope

This CLA applies only to code contributed to the `closure` branch in the following areas:

```text
L1: ui/src/riic/riic-sim/, ui/src/riic/sim/
L2: sim_bridge/, sim_api_bridge.py
L3: sim_bridge/autoschedule/, ui/src/riic/autoschedule/
and other closure-added code directories expressly approved by the Maintainer
```

This CLA does **not** apply to:

```text
arknights_mower/
upstream-tracked server.py, webview_ui.py, webui_zip.spec,
ui/package.json, ui/package-lock.json, ui/.gitignore, ui/src/pages/Plan.vue
and other upstream files or modifications to them
```

Changes to the mower core should be submitted to the upstream project, not to the `closure` branch.

## 2. Contributor Retains Copyright

The Contributor retains copyright in the Contribution.  
This CLA does not require an assignment of copyright; it grants the Maintainer the licenses below.

## 3. License Granted to the Maintainer

The Contributor grants LeeJSwit (the "Maintainer") a:

- perpetual;
- worldwide;
- non-exclusive;
- royalty-free;
- irrevocable;

copyright license permitting the Maintainer to:

- reproduce, modify, and distribute the Contribution;
- create derivative works;
- combine the Contribution with other parts of the project;
- distribute and sublicense the Contribution under PolyForm Noncommercial 1.0.0 or a future license selected by the Maintainer;
- use the Contribution for project operation, publication, and maintenance.

This license does not restrict the Contributor's other uses of the Contribution, but the Contributor may not require the Maintainer to remove versions that have already been published.

## 4. Patent License

The Contributor grants the Maintainer a perpetual, worldwide, non-exclusive, royalty-free, irrevocable patent license covering patent claims that the Contributor owns or has the right to license and that would necessarily be infringed by use of the Contribution.

If the Contributor or the Contributor's organization asserts a patent infringement claim against the project, the patent license granted in this Section 4 terminates immediately.

## 5. Contributor Representations

The Contributor represents and warrants that:

- the Contributor has the right to submit the Contribution;
- the Contribution is original, or the Contributor has obtained all necessary third-party permissions;
- the Contribution does not contain unauthorized third-party code, game assets, account data, keys, or personal information;
- the Contribution does not contain code that the Contributor knows infringes the rights of others;
- the Contribution is not used for boosting, account farming, hosting, paid interfaces, or other commercial services;
- the Contribution complies with the scope and licensing requirements in `CONTRIBUTING.md`;
- submitting the Contribution does not breach any agreement between the Contributor and the Contributor's employer or institution; and
- if the Contribution is a work made for hire or is otherwise made in the course of employment, the Contributor has obtained the employer's express authorization.

## 6. License Files and File Headers

The Contributor agrees to:

- license new closure files under PolyForm Noncommercial 1.0.0;
- mark new file headers with the actual contributors, one line per contributor:
  ```text
  SPDX-FileCopyrightText: 2026 LeeJSwit
  SPDX-FileCopyrightText: 2026 <Contributor>
  SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0
  ```
- preserve each contributor's copyright line without merging, overwriting, or adding a line for a non-contributor;
- preserve the original MIT copyright and license notices when modifying MIT files, and not relicense MIT files under PolyForm;
- not remove `LICENSE`, `LICENSE-CLOSURE`, `NOTICE`, or `USER-NOTICE.md`.

## 7. Acceptance

A Contributor accepts this CLA by:

- replying to the CLA Assistant prompt on a Pull Request; or
- stating in the PR description: "I accept CLA.md 1.1".

A PR that has not completed acceptance will not enter merge review.

## 8. Maintainer Rights

The Maintainer may:

- reject contributions that do not comply with the scope, license, or project positioning;
- request additional proof of rights from the Contributor;
- remove contributions that violate this CLA or project rules;
- adjust the project license without violating licenses already granted;
- if a Contributor breaches this CLA, the project license, or the restrictions in `USER-NOTICE.md`, terminate, to the extent permitted by applicable law, the authorization granted to that Contributor under this CLA and stop distributing the Contributor's Contribution.

## 9. Disclaimer and Governing Law

This CLA is a licensing arrangement between the Contributor and the Maintainer. It does not alter the license of upstream MIT code and does not constitute any commitment to game publishers, platforms, or third parties.

This CLA is governed by the laws of the People's Republic of China (excluding the laws of Hong Kong, Macao, and Taiwan). Any dispute arising from or relating to this CLA shall first be resolved through friendly negotiation between the parties.
