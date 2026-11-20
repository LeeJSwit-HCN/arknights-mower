# arknights-mower（closure 分支）

个人维护的 [Arknights Mower](https://github.com/ArkMowers/arknights-mower) fork，基于上游 `alpha`
快照 `f7b1a70`（v4.1.6-alpha.15），只维护 `closure` 分支。非官方版本，不代表上游维护者立场，
不提供官方支持。

> 本次为 docs-only 基线提交：仅含文档与许可证。L1/L2 代码与可运行包随 closure v0.1.0 代码发行提供。

## 与上游的关系

- 上游 `alpha` 的改动经人工审阅后再合并，不自动跟随；当前基线落后上游若干提交。
- Closure 0.1.0 代码发行时禁用继承自上游的自动更新器，避免被上游 Release/Nightly 或源码分支覆盖；后续提供 Closure 自己的更新器。
- 不向上游提交 PR；继承自上游的文件及对它们的修改保持 MIT。

## 项目定位

本项目是个人学习研究项目，研究开源项目 arknights-mower 在虚拟设备/仿真环境下的自动化测试与排班算法。

- 不修改游戏客户端、不读取游戏内存、不拦截网络通信、不修改游戏文件；
- 这些技术特征只是实现说明，不构成鹰角网络的授权；
- 不授权、不提供将本项目接入真实游戏环境的教程或支持；
- 禁止将本项目用于违反游戏服务条款、商业代练、托管或其他商业用途；
- 与鹰角网络、悠星及 ArkMowers 无隶属关系。

## 使用前须知

- 本项目是非官方、个人维护的 fork，不代表上游维护者，也不代表鹰角网络。
- 继承自上游的文件及对它们的修改为 MIT；本 fork 新增的文件为 PolyForm Noncommercial 1.0.0；**不提供商业许可，也不接受商业许可申请**。
- 自动化操作可能违反游戏服务条款并导致账号处罚；账号、设备与数据风险由使用者自行承担。
- 完整条款、数据与隐私说明、确认流程见 [`USER-NOTICE.md`](USER-NOTICE.md)。

## 内容范围

| 层 | 位置 | 说明 |
|---|---|---|
| L1 基建仿真层 | `ui/src/riic/riic-sim/` | TypeScript 物理引擎与 v2 数值模型；HTTP 桥在 `bridge/` |
| L2 mower 无头执行层 | `sim_bridge/`、`sim_api_bridge.py` | 虚拟时钟驱动 mower 业务逻辑；`/sim/*` 由 `server.py` 注册 |
| L3 排班优化层 | 待发布 | 自动排班搜索，开发中 |

## 架构说明

closure 分支的分层技术文档从 [`architecture/README.md`](architecture/README.md) 开始：

- [L1 仿真层](architecture/l1-simulation.md)：确定性基建世界；用法、快速开始、可靠性论证与适用域；
- [L2 执行层](architecture/l2-execution.md)：无设备跑 mower 业务；快速开始、回放差分、业务回归与 CI 三道门；
- [L3 目标页](architecture/l3-target.md)：排班优化层的目标与边界（仍在开发中，尚未推送）。

L2 文档 §7.6 还说明了 mower-sim：面向 mower 业务核心开发者的命令行回放工作台。首版只提供命令行回放工具，mower-sim 前端与完整工作台属于后续版本。

文档中的经验数字来自开发者本地标定，测试与验收数据不随仓库发布。

## 开发说明

closure 新增文档不提供面向用户的安装、配置或真实游戏接入教程。继承自上游的文档与入口保持上游原样，不代表 closure 的定位或立场。开发与测试约定见 [`CONTRIBUTING.md`](CONTRIBUTING.md)。

## 许可与使用

- 继承自上游的文件及对它们的修改：MIT（`LICENSE`）；本 fork 新增的文件：PolyForm Noncommercial 1.0.0
  （`LICENSE-CLOSURE`），范围见 `NOTICE`。
- 新增 closure 文件是否适用 PolyForm，以文件头是否带 `SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0` 为准；漏带标识的新增文件仍按新增文件处理。`LICENSE-CLOSURE` 是许可正文，`CLOSURE-VERSION` 是纯版本号数据，两者不按此规则判定。
- 允许任何非商业目的（范围见 `LICENSE-CLOSURE`）；**不提供商业许可，也不接受商业许可申请**，代练、代肝、托管、
  付费接口等商业使用不在授权范围内。
- PolyForm Noncommercial 1.0.0 没有 Change Date；它不是 OSI 认证的开源许可证，属于 source-available。
- PolyForm 不限制 MIT 上游文件的商业使用。
- Release 包为 MIT + PolyForm Noncommercial 1.0.0 混合许可分发：上游部分仍按 MIT，closure 新增部分按 PolyForm；分发时需附带 `LICENSE`、`LICENSE-CLOSURE`、`NOTICE`、`USER-NOTICE.md`。
- 使用前请阅读 [`USER-NOTICE.md`](USER-NOTICE.md)（使用须知与风险确认书）。

## 免责声明

- 本项目为个人学习研究项目，非商业；不提供、也不接受商业许可申请；不参与、不授权任何代练、代肝、托管、付费服务或付费合作。
- 开发者不提供任何付费服务，权利人提出异议时停止分发。
- 游戏《明日方舟》及其素材版权归鹰角网络所有；使用本工具可能违反游戏服务条款，
  账号与数据风险由使用者自行承担。
- 不保证稳定性与兼容性，不对使用后果承担责任。