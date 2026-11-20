SPDX-FileCopyrightText: 2026 LeeJSwit
SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0

# arknights-mower (closure branch)

A personally maintained fork of [Arknights® Mower](https://github.com/ArkMowers/arknights-mower), based on the upstream `alpha` snapshot `f7b1a70` (v4.1.6-alpha.15). Only the `closure` branch is maintained. This is an unofficial version; it does not represent the upstream maintainers and does not provide official support.

> This is a docs-only baseline commit: documentation and licenses only. L1/L2 code and runnable packages will be provided with the closure v0.1.0 code release.
>
> Chinese: [README.md](README.md)

## Relationship with Upstream

- Upstream `alpha` changes are reviewed manually before merging; this branch does not follow upstream automatically and is currently behind several upstream commits.
- Closure 0.1.0 disables the inherited auto-updater when the code is released, so it cannot be overwritten by upstream releases, nightlies, or source branches. Closure will provide its own updater later.
- No pull requests are submitted upstream. Upstream files and modifications to them remain MIT-licensed.

## Project Positioning

This is a personal study and research project. It studies automated testing and scheduling algorithms for the open-source arknights-mower project in virtual-device and simulation environments.

- It does not modify the game client, read game memory, intercept network traffic, or modify game files.
- These technical characteristics are implementation notes only; they do not constitute authorization from Hypergryph®.
- It does not authorize or provide tutorials or support for connecting the project to a real game environment.
- Use of the project for violating game terms of service, commercial boosting, account farming, hosting, or other commercial purposes is prohibited.
- It is not affiliated with Hypergryph, Yostar, or ArkMowers.

## Before Use

- This is an unofficial, personally maintained fork. It does not represent the upstream maintainers or Hypergryph.
- Upstream files and modifications to them are MIT-licensed. New files added by this fork are PolyForm Noncommercial 1.0.0. **No commercial license is offered or accepted.**
- Automated operations may violate game terms of service and lead to account penalties. Account, device, and data risks are borne by the user.
- See [`USER-NOTICE.en.md`](USER-NOTICE.en.md) for the complete terms, data and privacy information, and confirmation process.
- See [`SECURITY.en.md`](SECURITY.en.md) for vulnerability reporting and cases that are not security vulnerabilities.

## Scope

| Layer | Location | Description |
|---|---|---|
| L1 base simulation | `ui/src/riic/riic-sim/` | TypeScript physics engine and v2 numeric model; HTTP bridge under `bridge/` |
| L2 headless mower execution | `sim_bridge/`, `sim_api_bridge.py` | Virtual clock drives mower business logic; `/sim/*` is registered by `server.py` |
| L3 scheduling optimization | Not released | Automatic schedule search, in development |

## Architecture

The layered technical documentation starts at [`architecture/README.md`](architecture/README.md):

- [L1 simulation](architecture/l1-simulation.md): deterministic base world; usage, quick start, reliability argument, and scope;
- [L2 execution](architecture/l2-execution.md): running mower business without a device; quick start, replay diff, business regression, and the three CI gates;
- [L3 target](architecture/l3-target.md): goals and boundaries of the scheduling optimization layer (in development, not pushed).

L2 documentation §7.6 also describes mower-sim, a command-line replay workbench for mower business-core developers. The first release provides only the command-line replay tool; the mower-sim frontend and full workbench are planned for later versions.

The empirical numbers in the documentation come from local developer calibration. Test and acceptance data are not published with the repository.

## Development

New closure documentation does not provide user-facing installation, configuration, or real-game integration tutorials. Documentation inherited from upstream remains as upstream provided it and does not represent closure's positioning or views. Development and testing conventions are in [`CONTRIBUTING.en.md`](CONTRIBUTING.en.md).

## License and Use

- Upstream files and modifications to them: MIT (`LICENSE`); new files added by this fork: PolyForm Noncommercial 1.0.0 (`LICENSE-CLOSURE`), with scope described in `NOTICE`.
- The current versions of `README.md` / `README.en.md` are independent closure rewrites and are PolyForm; the original upstream README at `f7b1a70` remains MIT.
- Whether a new closure file is covered by PolyForm is determined by the SPDX identifier in its header. A new file that omits the identifier is still treated as a new file. `LICENSE-CLOSURE` is the license text and `CLOSURE-VERSION` is version-only data; neither is judged by the header rule.
- Any noncommercial purpose is permitted (scope: `LICENSE-CLOSURE`). **No commercial license is offered or accepted.** Commercial use, including boosting, account farming, hosting, or paid interfaces, is outside the license.
- PolyForm does not restrict commercial use of MIT-covered upstream files.
- A Release package should be distributed under the mixed MIT + PolyForm Noncommercial 1.0.0 license: upstream portions remain MIT and closure-added portions are PolyForm. Distributions must include `LICENSE`, `LICENSE-CLOSURE`, `NOTICE`, and `USER-NOTICE.md`.
- Read [`USER-NOTICE.en.md`](USER-NOTICE.en.md) before use.

## Disclaimer

- This is a personal study and research project. It is noncommercial, does not offer or accept commercial licenses, and does not participate in or authorize boosting, account farming, hosting, paid services, or paid cooperation.
- The developer does not provide any paid service and will stop distribution if a rights holder objects.
- The copyright in *Arknights* and its assets belongs to Hypergryph. Use of this tool may violate the game's terms of service; account and data risks are borne by the user.
- Stability and compatibility are not guaranteed, and the developer is not liable for the consequences of use.
