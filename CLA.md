SPDX-FileCopyrightText: 2026 LeeJSwit
SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0

# Closure 贡献者许可协议（CLA）

> 版本：1.0  
> 适用：向 `closure` 分支提交的 L1 / L2 / L3 代码贡献。  
> 本文件不构成法律意见；正式启用前应由律师审阅。

## 1. 范围

本 CLA 仅适用于贡献者向本仓库 `closure` 分支提交的、属于以下范围的代码：

```text
L1：ui/src/riic/riic-sim/、ui/src/riic/sim/
L2：sim_bridge/、sim_api_bridge.py
L3：sim_bridge/autoschedule/、ui/src/riic/autoschedule/
以及维护者明确允许的其他 closure 新增代码目录
```

本 CLA **不适用于**：

```text
arknights_mower/
上游跟踪的 server.py、webview_ui.py、webui_zip.spec、
ui/package.json、ui/package-lock.json、ui/.gitignore、ui/src/pages/Plan.vue
等上游文件及其修改
```

涉及 mower 核心的修改，请提交到上游项目，不要提交到 `closure` 分支。

## 2. 贡献者保留版权

贡献者保留其贡献的版权。  
本 CLA 不要求转让版权，只要求授予维护者以下许可。

## 3. 授予维护者的许可

贡献者授予 LeeJSwit（以下简称“维护者”）一项：

- 永久；
- 全球范围；
- 非独占；
- 免许可费；
- 不可撤销；

的版权许可，允许维护者：

- 复制、修改、分发贡献；
- 创作衍生作品；
- 将贡献与项目其他部分组合；
- 以 PolyForm Noncommercial 1.0.0 或维护者选择的未来许可证分发、再许可贡献；
- 为项目运营、发布和维护目的使用贡献。

该许可不影响贡献者对其贡献的其他使用，但贡献者不得要求维护者删除已经发布的版本。

## 4. 专利许可

贡献者授予维护者一项永久、全球、非独占、免许可费、不可撤销的专利许可，覆盖贡献者拥有或有权许可的、因使用其贡献而必然侵权的专利权利要求。

如果贡献者或其所属组织对项目提起专利侵权主张，本条第 4 款授予的专利许可立即终止。

## 5. 贡献者声明

贡献者声明并保证：

- 其有权提交该贡献；
- 贡献为原创，或已获得必要的第三方许可；
- 贡献不包含未经授权的第三方代码、游戏素材、账号数据、密钥或个人信息；
- 贡献不包含明知会侵犯他人权利的代码；
- 贡献不用于代练、代肝、托管、付费接口等商业服务；
- 贡献符合 `CONTRIBUTING.md` 的范围和许可要求。

## 6. 许可文件与文件头

贡献者同意：

- 新增 closure 文件使用 PolyForm Noncommercial 1.0.0；
- 新增文件头按实际贡献者逐行标注：
  ```text
  SPDX-FileCopyrightText: 2026 LeeJSwit
  SPDX-FileCopyrightText: 2026 <贡献者>
  SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0
  ```
- 每位贡献者保留自己的版权行，不合并、不覆盖，也不替未参与者添加；
- 修改 MIT 文件时保留原 MIT 版权和许可声明，不把 MIT 文件改成 PolyForm；
- 不删除 `LICENSE`、`LICENSE-CLOSURE`、`NOTICE`、`USER-NOTICE.md`。

## 7. 接受方式

贡献者通过以下方式接受本 CLA：

- 在 Pull Request 中按 CLA Assistant 提示回复同意；或
- 在 PR 描述中明确写明“我接受 CLA.md 1.0”。

未完成接受的 PR 不进入合并审查。

## 8. 维护者权利

维护者可以：

- 拒绝不符合范围、许可或项目定位的贡献；
- 要求贡献者补充权利证明；
- 移除违反本 CLA 或项目规则的贡献；
- 在不违反已发布许可证的前提下调整项目许可证。

## 9. 免责声明

本 CLA 是贡献者与维护者之间的许可安排，不改变上游 MIT 代码的许可，也不构成对游戏厂商、平台或第三方的任何承诺。

本文件不构成法律意见；正式启用前应咨询律师。
