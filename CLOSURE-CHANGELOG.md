SPDX-FileCopyrightText: 2026 LeeJSwit
SPDX-License-Identifier: PolyForm-Noncommercial-1.0.0

# Closure 更新日志

## 0.1.0（计划）

> 本文档版本从 1.0 起算：当前 1.0 为重新起算的正式版本；此前编号为 1.0、1.1、1.2 的文本（如存在）均为内部草案，不作为正式版本。旧仓库中的草案不构成当前正式文本。
>
> 以下功能随 v0.1.0 代码发行提供；当前 docs-only 提交不包含代码，未实现项不作为既成事实。

### New

- Closure 分支用户许可与风险确认书 1.0：MIT 上游 + PolyForm Noncommercial 1.0.0 新增文件。
- 用户须知保留简明协议风险提示；不在公开文档中逐条引用协议条款。
- 新增 README、USER-NOTICE、CONTRIBUTING 英文参考版；`README.en.md` 与 `README.md` 当前版本按 PolyForm 处理。
- 新增 SECURITY 中英文版本与 Issue 隐私确认模板。
- CLA 1.1：增加职务发明/职务行为声明、维护者终止权和中华人民共和国法律适用；新增英文参考版。
- closure 功能级许可门禁：首次进入 closure 功能时确认；拒绝不进入 closure，不影响上游 Mower；门禁随代码发行生效。
- 基建模拟器：
  - 演算当前排班；
  - 演算下一周；API 单次推进上限 28 天，产品界面可分段继续（见 L2 §4.3）；
  - 展示时间与后台进度分离；
  - 任意时刻统一基建上下文；
  - 产出/心情/跑单/诊断分析入口。
- 双版本展示：Closure 0.1.0 / Alpha 4.1.6-alpha.15。
- L1 文档新增数据来源与边界说明。

### Notes

- 本版本不包含 mower-sim 前端/可视化工作台；命令行回放工具随代码发行提供。
- 本版本不包含 L3 自动排班，不生成或导出 L3 plan。
- PolyForm Noncommercial 1.0.0 不是 OSI 认证的开源许可证；新增文件仅允许非商业目的。
- L1 校准与设备侧对账仍在进行；仿真结果是模型估计，不是真实产出承诺。
