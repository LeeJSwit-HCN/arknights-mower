SPDX-FileCopyrightText: 2026 LeeJSwit
SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0

# 贡献指南

> English: [CONTRIBUTING.en.md](CONTRIBUTING.en.md)

## 1. 先签 CLA

任何代码 PR 必须先接受 [CLA.md](CLA.md)（[English](CLA.en.md)）。未签 CLA 的 PR 不进入合并审查。

维护者需在仓库配置 `CLA_SIGNATURES_TOKEN`（contents: write）；该说明属于仓库配置，不写入 CLA 正文。

安全漏洞不要提交公开 Issue，请按 [`SECURITY.md`](SECURITY.md) 私密报告。

CLA 只覆盖：

```text
L1：ui/src/riic/riic-sim/、ui/src/riic/sim/
L2：sim_bridge/、sim_api_bridge.py
L3：sim_bridge/autoschedule/、ui/src/riic/autoschedule/
维护者明确允许的其他 closure 新增代码目录
```

## 2. 不要修改 mower 核心

以下内容不接受外部 PR：

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

需要修改 mower 核心，请去上游项目提交。  
closure 分支不接受“顺手改一下上游”的 PR。

## 3. 只接受 L1/L2/L3 代码

- L1：仿真实体、技能、心情、生产、订单、无人机、电力；
- L2：虚拟时钟、seam、无头执行、服务、缓存、回归；
- L3：排班优化、候选评估与搜索（认证类能力 0.3.0 前不提供）；
- 文档修正可以单独提交，但不要混入商业使用、代练、托管功能。

不接受：

- 商业使用功能；
- 代练、代肝、托管、付费接口；
- 真实游戏接入教程；
- 游戏内存修改、网络拦截、客户端破解；
- 真实账号、日志、截图、凭据、个人信息；
- 规避检测、绕过限制的功能。

## 4. 文件头

新增 closure 文件：

```text
SPDX-FileCopyrightText: 2026 LeeJSwit
SPDX-FileCopyrightText: 2026 <贡献者>
SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0
```

每位实际贡献者保留自己的版权行；不要合并、覆盖或替未参与者添加版权行。仅由 LeeJSwit 创建的文件只写 LeeJSwit；其他贡献者实际修改/共同创作时，再追加其版权行。

修改 MIT 文件：

- 保留原版权和 MIT 声明；
- 不添加 PolyForm 头；
- 不删除 `LICENSE`、`NOTICE`、`USER-NOTICE.md`。

## 5. 测试

提交前至少运行与改动相关的定向测试：

```text
L1: ui/ 下的 vitest 定向测试
L2: sim_bridge 相关 pytest
L3: 对应 L3 测试
```

不要提交需要真实游戏账号、真实设备或真实数据的测试。

## 6. PR 要求

- 一个 PR 只做一类改动；
- 说明改动范围、测试结果和已知限制；
- 不包含 `arknights_mower/` 改动；
- 不包含商业/代练相关内容；
- 不包含未完成的功能入口；
- 不包含真实凭据或个人数据；
- 通过路径守卫和 CLA 检查。

## 7. 项目定位

本项目是个人学习研究项目，研究开源项目 arknights-mower 在虚拟设备/仿真环境下的自动化测试与排班算法。

本项目不提供将代码接入真实游戏环境的教程或支持；禁止将本项目用于违反游戏服务条款、商业代练、托管或其他商业用途。

## 8. 许可

- 上游 MIT 文件保持 MIT；
- 新增 closure 文件适用 PolyForm Noncommercial 1.0.0；
- 不接受商业许可申请；
- 贡献即表示同意 [CLA.md](CLA.md)。
