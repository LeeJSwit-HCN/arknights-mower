SPDX-FileCopyrightText: 2026 LeeJSwit
SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0

# closure 分支用户使用许可与风险确认书

**文档版本**：1.0  
**文档日期**：2026-11-20  
**适用版本**：closure v0.1.0（计划 tag `closure-v0.1.0`；上游基线 v4.1.6-alpha.15 / `f7b1a70`）  
**文档性质**：使用许可说明、风险告知与用户确认；不替代 [LICENSE](LICENSE) / [LICENSE-CLOSURE](LICENSE-CLOSURE)，冲突时以许可条款为准。  
**English version**：[USER-NOTICE.en.md](USER-NOTICE.en.md)

## 摘要

本项目是**非官方、个人维护**的 mower fork，与鹰角网络®、悠星、ArkMowers 及其维护者无隶属关系。

上游文件按 **MIT**、closure 新增文件按 **PolyForm Noncommercial 1.0.0** 提供。新增部分仅允许非商业目的，**不提供商业许可，也不接受商业许可申请**。

将本项目或其输出用于真实游戏环境，可能违反游戏服务条款并导致账号处罚；账号、设备与数据风险由使用者自行承担。

## 1. 项目性质与定义

- **本项目**：`closure` 分支及其发布物（源码、文档、脚本与二进制）。L3 正在开发、尚未推送；0.3.0 前不提供 plan 生成或导出。
- **上游**：[ArkMowers/arknights-mower](https://github.com/ArkMowers/arknights-mower)（MIT）；本项目基于快照 `f7b1a70`（v4.1.6-alpha.15）派生，不自动跟随上游。
- **游戏**：《明日方舟®》（Arknights®），权利归鹰角网络（Hypergryph®）、悠星（Yostar）等权利人。
- **您**：使用本项目的自然人。

本项目是个人学习与研究项目，非官方、非商业，无官方支持、SLA 或稳定性、兼容性保证。当前版本不通过本项目获取收入。

## 2. 许可结构

### 2.1 混合许可

| 范围 | 许可 | 说明 |
|---|---|---|
| 上游文件及其修改 | MIT（[LICENSE](LICENSE)） | 原文件版权归原作者；修改部分归修改者 |
| `README.md` / `README.en.md` 当前版本 | PolyForm Noncommercial 1.0.0 | closure 独立重写；上游原始 README 仍按 MIT |
| closure 新增文件（相对 `f7b1a70`） | PolyForm Noncommercial 1.0.0（[LICENSE-CLOSURE](LICENSE-CLOSURE)） | 以文件头 SPDX 标识为准 |
| 游戏素材与数据 | 鹰角网络版权所有 | 见第 6 节与 [NOTICE](NOTICE) |

**判定规则**：closure 新增的代码、文档与模板适用 PolyForm Noncommercial 1.0.0；新增文件应带 `SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0`，漏带标识的新增文件仍按新增文件处理。继承自上游的文件及修改适用 MIT；`README.md` / `README.en.md` 当前版本为 closure 独立重写文档，适用 PolyForm，上游原始 README 仍按 MIT。`LICENSE-CLOSURE` 是许可正文，`CLOSURE-VERSION` 是纯版本号数据，两者不按文件头规则判定。纯数据文件按 [NOTICE](NOTICE) 处理。本说明不是许可合同，不改变许可条款。

### 2.2 PolyForm Noncommercial 1.0.0 的要点

- 允许任何**非商业目的**，包括个人学习、研究、实验、测试、私人娱乐和业余项目；
- 不允许带有预期商业应用的使用；
- 本许可不是 OSI 认证的开源许可证，属于 source-available；
- MIT 上游部分不受本许可限制，仍按 MIT 使用。

**这是版权许可，不是鹰角游戏使用许可。** 它不授权、也不表示可以违反《鹰角网络游戏使用许可及服务协议》运行游戏或使用游戏服务。

### 2.3 允许与禁止

PolyForm 允许对代码本身的非商业使用：为个人学习、研究、内部非商业评估与测试而复制、修改、创作衍生作品；按 MIT / PolyForm 条件再分发并保留 `LICENSE`、`LICENSE-CLOSURE`、`NOTICE`、`USER-NOTICE.md` 四个文件与文件头；查看、审计、修改已发布源码。

PolyForm 不授权在真实游戏账号、真实客户端或真实设备上运行游戏，也不提供相关支持。是否将本项目接入真实游戏环境，由使用者自行判断并承担风险；开发者不授权、不建议、不指导此类使用。

商业使用包括但不限于：代练、代肝、托管、付费接口等付费服务；出售或付费分发；订阅、广告或捐赠变现；营利实体用于生产业务；向第三方提供功能作为服务；为上述行为提供协助。

**商业许可**：本仓库不提供商业许可，也不接受商业许可申请。上述使用不被授权，请停止使用。此限制仅针对 PolyForm 新增文件；MIT 上游文件仍可按 MIT 商业使用。商业限制是版权许可条款，不改变鹰角协议对第三方工具、辅助程序或相关方法的限制。

### 2.4 许可的边界

PolyForm Noncommercial 1.0.0 限制商业目的，不限制 MIT 上游文件的商业使用。许可边界的完整说明见 [NOTICE](NOTICE)。任何版权许可都不构成鹰角网络对游戏软件、游戏服务、游戏数据或游戏素材的授权。

### 2.5 开发者立场

本人不参与、不授权任何以本项目或其衍生作品牟利的运营行为，也不接受捐赠、赞助、广告或付费合作。上述立场是个人声明，不构成对 `LICENSE` / `LICENSE-CLOSURE` 的修改；MIT 上游文件仍按 MIT 使用，本人无权限制。

## 3. 使用风险

### 3.1 使用边界与账号风险

本项目是面向 arknights-mower 的仿真、测试与排班研究项目。
本项目不提供游戏客户端修改、内存读取、网络拦截或真实游戏接入教程。
使用者将本项目或其输出用于真实游戏环境时，应自行确认并遵守游戏服务条款；
账号、设备与数据风险由使用者自行承担。
请勿将本项目用于商业代练、托管或其他违反服务条款的用途。

### 3.2 设备与数据风险

本项目读写配置、数据库、日志、缓存与截图，可能因设备、模拟器、ADB、系统更新、权限或人为操作导致数据丢失或设备异常。请自行备份 `config/`、`data.db` 与排班表；开发者不对数据丢失、设备损坏、系统不稳定承担责任。

### 3.3 第三方服务风险

森空岛签到、MAA、企鹅物流/一图流上报、AI 助手等可能连接第三方服务；可用性、条款与数据处理由对应服务方决定，开发者不对其承担责任。请自行阅读并遵守其条款。

## 4. 无担保与责任限制

本项目按 **“AS IS”** 提供，无任何明示或默示担保，包括适销性、特定用途适用性、不侵权与无错误。

**在适用法律允许的最大范围内**，开发者不对账号处罚、数据丢失、设备损坏、收益损失、第三方索赔及间接、附带、特殊或惩罚性损失承担责任。该限制不排除依法不可排除的责任（如故意或重大过失）；适用法律不允许的部分在该法律允许范围内失效，其余条款继续有效。

不同意本须知，请停止使用并删除本项目。

## 5. 数据与隐私

### 5.1 默认不上传

当前版本不向开发者服务器上传排班表、干员数据、运行日志、账号、密码、手机号或设备标识，也不主动收集或存储 IP；核心功能在本地运行，本项目不是云端服务。访问 GitHub 或第三方服务时，对方会看到您的 IP。

### 5.2 AI 助手与联网请求

AI 助手是可选功能。启用后，您输入的提示、必要的排班/干员/运行上下文与您配置的 API Key，会发送到您选择的模型服务（如 DeepSeek、自定义 OpenAI 兼容接口等）；其条款与隐私政策由对应提供方负责，启用前请自行阅读。不使用 AI 助手时，不主动上传上述内容。AI 助手仅在您主动要求发送反馈时，通过 `submit_issue` 将您确认的内容与必要日志/截图发送给开发组邮箱；不经过开发者自建服务器。

更新检查会访问 GitHub；森空岛、MAA 等第三方请求同样会让对方看到您的 IP。开发者不运营收集这些数据的服务器。

### 5.3 森空岛凭据与本地配置

森空岛自动签到是本地可选功能。森空岛登录凭据（token/credential，可能包含账号标识）以**明文**保存在本地配置（如 `config/conf.yml`），不会上传到开发者服务器；开发者不代理签到、不收集凭据。请勿提交或分享含凭据的配置、日志、截图（公开仓库、Issue、聊天、网盘等）；如曾泄露，请立即更换森空岛密码并重新登录。

### 5.4 可选数据收集（如未来提供）

如未来提供，将默认关闭、需单独勾选同意，适用单独《数据收集说明》；只上传去标识化聚合数据，不上传排班表、干员数据、原始日志、账号或设备标识；可随时暂停或删除；不同意不影响使用。

## 6. 第三方组件与游戏素材

上游 mower 按 MIT 提供，Python/Node 依赖、MAA、ADB、模拟器等按各自许可提供。《明日方舟》素材与游戏数据（含数据文件中源于游戏的内容）权利归鹰角网络；公开 wiki、公开上游数据或公开计算器不等于鹰角对游戏数据/素材的授权。本项目仅就整理结构、字段选择与编排主张权利（见 [NOTICE](NOTICE)），不授予商标、标识或官方背书的许可。若权利人提出异议，开发者将停止分发并在可行范围内移除相关素材或数据。

## 7. 未成年人

本项目不面向未成年人定向提供。已满 18 周岁可独立使用；已满 14 周岁未满 18 周岁的，应取得监护人同意后阅读并决定是否使用；未满 14 周岁不得使用。当前版本不收集未成年人数据；如未来启用数据收集，需监护人单独同意。监护人发现未成年人未经同意使用，请停止使用并删除本项目。

## 8. 确认方式与接受记录

首次进入 closure 功能时，前端显示本须知的确认页；逐项确认并全部勾选后，才继续进入 closure 功能。接受时记录文档版本、内容哈希、时间与语言。该门禁随 v0.1.0 代码发行生效；当前 docs-only 提交只说明规则。

确认项包括：非官方与许可结构、账号与设备及数据风险、数据与隐私、非商业使用、年龄确认。门禁仅适用于 closure 新增功能，不影响上游 MIT 核心；拒绝时仅关闭 closure 功能，仍可使用 Mower 核心。

## 9. 变更、终止与权利异议

须知随 closure 版本更新，重大变更在 release notes 提示；重大变更按第 8 节重新确认。不同意请停止使用 closure 功能。

违反 `LICENSE-CLOSURE` 的使用按该许可条款处理；应立即停止使用并删除副本。权利人（鹰角网络、悠星、上游维护者）提出异议时，开发者将停止分发并配合处理，您应自行停止使用。

## 10. 联系方式

- 权利异议、合规问题：GitHub [@LeeJSwit-HCN](https://github.com/LeeJSwit-HCN)。
- 安全问题与漏洞：通过 GitHub 私下联系，勿在公开 Issue 贴凭据或漏洞细节。
- 商业许可：本仓库不提供，也不接受商业许可申请。

## 声明

本须知是使用许可说明与风险告知，不构成法律意见；具体法律问题请咨询专业人士。

## 附录：English Summary (Courtesy Translation)

Courtesy summary only; the Chinese text is authoritative.

- Unofficial personal fork of Arknights Mower (upstream `f7b1a70` / v4.1.6-alpha.15), closure v0.1.0 (planned tag `closure-v0.1.0`); no affiliation with Hypergryph, Yostar, ArkMowers, or their maintainers.
- Upstream files and modifications stay MIT; closure-added files use PolyForm Noncommercial 1.0.0 per SPDX headers. The license permits noncommercial purposes only. No commercial license is offered or accepted; commercial use is not permitted. PolyForm is source-available, not an OSI-approved open source license.
- The project is a simulation, testing, and scheduling research project built around arknights-mower. It does not provide client modification, memory reading, network interception, or real-game integration tutorials. If you use the project or its output in a real game environment, you are responsible for confirming and complying with the game's terms; account, device, and data risks are yours. Provided "AS IS" without warranties; liability limited as far as law allows.
- No plans, operator data, logs, accounts, passwords, phone numbers, or device IDs are uploaded to developer servers, and IPs are not actively collected or stored; GitHub and third-party services see your IP when contacted. The optional AI assistant sends prompts, necessary context, and your API key to your chosen model service under that provider's terms and privacy policy. When you explicitly request feedback submission, the assistant sends the content you confirm and necessary logs/screenshots to the developer group's email via `submit_issue`; it does not use a developer-operated server. Skland credentials (token/credential) stay in plaintext local config (e.g., `config/conf.yml`); never share them.
- The consent gate is shown before first use of closure features; acceptance records version, content hash, time, and language. Major changes require re-confirmation.
- Users must be 18+, or 14+ with guardian consent; under 14 may not use. The current version does not collect minor data. L3 is in development; no plan generation or export before 0.3.0.
- Game assets and game data belong to Hypergryph; public wikis, upstream data, and public calculators do not grant a game-data or game-asset license.
- L3 output terms and plan provenance are separate future documents and are not effective before 0.3.0.
- This notice does not replace LICENSE / LICENSE-CLOSURE; license terms prevail. It is not legal advice.
