SPDX-FileCopyrightText: 2026 LeeJSwit
SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0

# Closure Branch User License and Risk Acknowledgement

**Document version:** 1.0  
**Document date:** 2026-11-20  
**Applies to:** closure v0.1.0 (planned tag `closure-v0.1.0`; upstream baseline v4.1.6-alpha.15 / `f7b1a70`)  
**Nature of this document:** license explanation, risk disclosure, and user acknowledgement. It does not replace [LICENSE](LICENSE) / [LICENSE-CLOSURE](LICENSE-CLOSURE); if there is a conflict, the license terms prevail.  
**Chinese version:** [USER-NOTICE.md](USER-NOTICE.md) (authoritative)

## Summary

This is an **unofficial, personally maintained** fork of mower. It is not affiliated with Hypergryph®, Yostar, ArkMowers, or their maintainers.

Upstream files are provided under **MIT**; closure-added files are provided under **PolyForm Noncommercial 1.0.0**. The added portions permit noncommercial purposes only. **No commercial license is offered or accepted.**

Using this project or its output in a real game environment may violate the game's terms of service and lead to account penalties. Account, device, and data risks are borne by the user.

## 1. Project Nature and Definitions

- **This project:** the `closure` branch and its distributions (source, documentation, scripts, and binaries). L3 is in development and has not been pushed; plan generation and export are not provided before 0.3.0.
- **Upstream:** [ArkMowers/arknights-mower](https://github.com/ArkMowers/arknights-mower) (MIT). This project is derived from snapshot `f7b1a70` (v4.1.6-alpha.15) and does not automatically follow upstream.
- **Game:** *Arknights®*; rights belong to Hypergryph, Yostar, and other rights holders.
- **You:** the natural person using this project.

This is a personal study and research project. It is unofficial and noncommercial, with no official support, SLA, or guarantee of stability or compatibility. The current version does not generate revenue through this project.

## 2. License Structure

### 2.1 Mixed License

| Scope | License | Notes |
|---|---|---|
| Upstream files and modifications | MIT ([LICENSE](LICENSE)) | Original files remain the original authors' copyright; modifications belong to the modifier |
| Current `README.md` / `README.en.md` | PolyForm Noncommercial 1.0.0 | Independent closure rewrites; the original upstream README remains MIT |
| Closure-added files (relative to `f7b1a70`) | PolyForm Noncommercial 1.0.0 ([LICENSE-CLOSURE](LICENSE-CLOSURE)) | Determined by the SPDX identifier in the file header |
| Game assets and data | Hypergryph copyright | See Section 6 and [NOTICE](NOTICE) |

**Determination rule:** closure-added code, documentation, and templates are under PolyForm Noncommercial 1.0.0. New files should carry `SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0`; a new file that omits the identifier is still treated as a new file. Upstream files and modifications are under MIT; the current versions of `README.md` / `README.en.md` are independent closure rewrites under PolyForm, while the original upstream README remains MIT. `LICENSE-CLOSURE` is the license text and `CLOSURE-VERSION` is version-only data; neither is judged by the header rule. Pure data files follow [NOTICE](NOTICE). This explanation is not a license contract and does not change the license terms.

### 2.2 Key Points of PolyForm Noncommercial 1.0.0

- Any **noncommercial purpose** is permitted, including personal study, research, experiment, testing, private entertainment, and hobby projects.
- Use with an anticipated commercial application is not permitted.
- This is not an OSI-approved open source license; it is source-available.
- The MIT-covered upstream portion is not restricted by this license and remains usable under MIT.

**This is a copyright license, not a Hypergryph game-use license.** It does not authorize, and should not be read as permitting, running the game or using game services in violation of the *Hypergryph Network Game License and Service Agreement*.

### 2.3 Permitted and Prohibited Use

PolyForm permits noncommercial use of the code itself: copying, modifying, and creating derivative works for personal study, research, and internal noncommercial evaluation and testing; redistributing under the MIT/PolyForm conditions while retaining `LICENSE`, `LICENSE-CLOSURE`, `NOTICE`, and `USER-NOTICE.md` and the file headers; and viewing, auditing, and modifying published source.

PolyForm does not authorize running the game on a real game account, real client, or real device, and does not provide related support. Whether to connect the project to a real game environment is the user's own decision and risk. The developer does not authorize, recommend, or instruct such use.

Commercial use includes, without limitation: paid boosting, account farming, hosting, and paid interfaces; selling or paid distribution; subscription, advertising, or donation monetization; use by a for-profit entity in production; providing functionality to third parties as a service; and assisting with any of the above.

**Commercial license:** this repository does not offer commercial licenses and does not accept commercial license requests. The uses above are not authorized; stop using the project for them. This restriction applies only to PolyForm-covered new files; MIT-covered upstream files remain usable commercially under MIT. The commercial restriction is a copyright license term and does not change the Hypergryph agreement's restrictions on third-party tools, auxiliary programs, or related methods.

### 2.4 License Boundary

PolyForm Noncommercial 1.0.0 restricts commercial purposes but does not restrict commercial use of MIT-covered upstream files. See [NOTICE](NOTICE) for the complete boundary. No copyright license constitutes Hypergryph's authorization for game software, game services, game data, or game assets.

### 2.5 Developer Position

I do not participate in or authorize any profit-making operation of this project or its derivatives, and I do not accept donations, sponsorship, advertising, or paid cooperation. This is a personal statement, not a modification of `LICENSE` / `LICENSE-CLOSURE`; MIT-covered upstream files remain usable under MIT, and I have no authority to restrict them.

## 3. Risks of Use

### 3.1 Use Boundary and Account Risks

This project is a simulation, testing, and scheduling research project built around arknights-mower. It does not provide game client modification, memory reading, network interception, or real-game integration tutorials. If you use the project or its output in a real game environment, you must determine and comply with the applicable game terms yourself; account, device, and data risks are yours. Do not use the project for commercial boosting, hosting, or other purposes that violate the terms of service.

### 3.2 Device and Data Risks

The project reads and writes configuration, databases, logs, caches, and screenshots. Device, emulator, ADB, system update, permission, or human errors may cause data loss or device abnormalities. Back up `config/`, `data.db`, and schedules yourself. The developer is not liable for data loss, device damage, or system instability.

### 3.3 Third-Party Service Risks

Skland check-in, MAA, Penguin Logistics / Yituliu reporting, the AI assistant, and similar features may connect to third-party services. Availability, terms, and data processing are determined by those providers, and the developer is not liable for them. Read and comply with their terms.

## 4. No Warranty and Limitation of Liability

The project is provided **"AS IS"**, without any express or implied warranty, including merchantability, fitness for a particular purpose, non-infringement, or freedom from errors.

**To the maximum extent permitted by applicable law**, the developer is not liable for account penalties, data loss, device damage, loss of income, third-party claims, or indirect, incidental, special, or punitive damages. This limitation does not exclude liability that cannot be excluded by law (such as intentional misconduct or gross negligence); any provision held unenforceable shall be limited to the extent permitted by law, and the remaining provisions remain in effect.

If you do not agree with this notice, stop using the project and delete it.

## 5. Data and Privacy

### 5.1 No Upload by Default

The current version does not upload schedules, operator data, runtime logs, accounts, passwords, phone numbers, or device identifiers to developer servers, and does not actively collect or store IP addresses. Core functionality runs locally; this project is not a cloud service. GitHub and third-party services will see your IP address when contacted.

### 5.2 AI Assistant and Network Requests

The AI assistant is optional. When enabled, your prompts, necessary schedule/operator/runtime context, and your API key are sent to the model service you choose (such as DeepSeek or a custom OpenAI-compatible endpoint). Its terms and privacy policy are the provider's responsibility; read them before enabling. When the AI assistant is not used, this content is not actively uploaded. When you explicitly request feedback submission, the assistant sends the content you confirm and necessary logs/screenshots to the developer group's email via `submit_issue`; it does not use a developer-operated server.

Update checks contact GitHub; Skland, MAA, and other third-party requests also expose your IP to those parties. The developer does not operate servers that collect this data.

### 5.3 Skland Credentials and Local Configuration

Skland automatic check-in is an optional local feature. Skland login credentials (token/credential, which may include account identifiers) are stored **in plaintext** in local configuration (for example, `config/conf.yml`) and are not uploaded to developer servers. The developer does not proxy check-ins or collect credentials. Do not submit or share configuration, logs, or screenshots containing credentials (public repositories, issues, chats, cloud storage, etc.). If credentials have leaked, change the Skland password and log in again immediately.

### 5.4 Optional Data Collection (if offered in the future)

If offered in the future, collection will be off by default and require separate opt-in consent under a separate data-collection notice. Only de-identified aggregate data will be uploaded; schedules, operator data, raw logs, accounts, and device identifiers will not be uploaded. Collection can be paused or deleted at any time, and refusal will not affect use.

## 6. Third-Party Components and Game Assets

Upstream mower is provided under MIT. Python/Node dependencies, MAA, ADB, emulators, and similar components are provided under their respective licenses. Rights in *Arknights* assets and game data (including game-derived content in data files) belong to Hypergryph. Public wikis, public upstream data, and public calculators do not constitute Hypergryph's authorization for game data or assets. This project claims rights only in its organization, field selection, and arrangement (see [NOTICE](NOTICE)) and does not grant trademark, logo, or official-endorsement rights. If a rights holder objects, the developer will stop distribution and remove the relevant assets or data where feasible.

## 7. Minors

This project is not directed at minors. Users aged 18 or older may use it independently. Users aged 14 to 17 must obtain guardian consent before reading and deciding whether to use it. Users under 14 may not use it. The current version does not collect minors' data; if data collection is enabled in the future, separate guardian consent will be required. Guardians who discover unauthorized use by a minor should stop the use and delete the project.

## 8. Acknowledgement and Acceptance Records

On first entering a closure feature, the frontend displays the acknowledgement page for this notice. The user must confirm each item and check all boxes before continuing. Acceptance records the document version, content hash, time, and language. This gate takes effect with the v0.1.0 code release; the current docs-only commit only describes the rules.

The confirmation items include: unofficial status and license structure; account, device, and data risks; data and privacy; noncommercial use; and age confirmation. The gate applies only to closure-added features and does not affect the upstream MIT core. If the user declines, only closure features are disabled; the Mower core remains usable.

## 9. Changes, Termination, and Rights Objections

This notice is updated with closure versions. Material changes are noted in release notes and require re-confirmation under Section 8. If you do not agree, stop using closure features.

Use in violation of `LICENSE-CLOSURE` is handled under that license; stop using the project and delete copies immediately. If a rights holder (Hypergryph, Yostar, or an upstream maintainer) objects, the developer will stop distribution and cooperate, and you should stop using the project.

## 10. Contact

- Rights objections and compliance questions: GitHub [@LeeJSwit-HCN](https://github.com/LeeJSwit-HCN).
- Security issues and vulnerabilities: contact privately through GitHub; do not post credentials or vulnerability details in public issues.
- Commercial licensing: not offered and not accepted by this repository.

## Statement

This notice explains the license and discloses risks. It is not legal advice; consult a professional for specific legal questions.

This English translation is provided for reference. If the Chinese and English versions differ, the Chinese version prevails.
