# 工程实践与项目记录

这里记录我在 Python 自动化、Linux 服务维护、网络策略与可观测性方面的实践。
我关注小范围可回退的修改、可复核的测试，以及对“配置正确”和“真实业务可用”的明确区分。

## 精选项目

### [网络分流与可观测性工程实践](https://github.com/xiaowd1996/network-policy-lab)

围绕既有网络服务，整理策略分流、元数据诊断、配置维护与安全迁移的工程方法。

- **Python 自动化**：有前置条件的规则变换，保留原顺序与非目标字段，支持幂等检查。
- **运维与观测**：分层检查客户端、入口、握手和出口，区分流量统计口径。
- **安全与回退**：脱敏模板、备份与候选检查、原子更新、迁移回退边界。
- **可运行验证**：无需生产服务器或凭据的离线演示与单元测试。

[项目说明](https://github.com/xiaowd1996/network-policy-lab#readme) · [设计取舍](https://github.com/xiaowd1996/network-policy-lab/blob/main/docs/design-decisions.md) · [测试与限制](https://github.com/xiaowd1996/network-policy-lab/blob/main/docs/validation.md)

## 阅读说明

代码与文档整理采用 AI 辅助，上游组件按其来源说明；以实际实现、测试和限制为准，不宣称从零实现这些组件。
公开仓库仅包含适合展示的脱敏内容，不包含真实服务器地址、访问凭据、用户日志或业务数据。

Engineering notes on automation, configuration safety and observability — with runnable offline examples and explicit validation boundaries.
