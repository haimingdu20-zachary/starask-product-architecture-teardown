# StarAsk 网站版｜产品架构逆向拆解

本项目依据 2026-08-19 的公开官网与访客模式页面实证，使用 `product-architecture-teardown v2` 完成。它是功能等价分析，不是 StarAsk 官方架构、官方提示词或内部实现说明。

## 开源说明

原创分析、图表与报告排版采用 [CC BY 4.0](LICENSE.md)；`evidence/page-captures/` 中的第三方页面摘录不在该许可的再授权范围内。独立分析、非隶属关系与隐私说明见 [NOTICE.md](NOTICE.md)。

## 交付文件

1. [01-StarAsk-用户旅程-页面取证版.html](01-StarAsk-用户旅程-页面取证版.html)
2. [02-StarAsk-Agent契约-页面证据版.html](02-StarAsk-Agent契约-页面证据版.html)
3. [03-StarAsk-问事分析与追踪-功能等价SystemPrompt.html](03-StarAsk-问事分析与追踪-功能等价SystemPrompt.html)
4. [04-StarAsk-产品全景架构-证据分层版.html](04-StarAsk-产品全景架构-证据分层版.html)
5. [05-StarAsk-架构分层图.html](05-StarAsk-架构分层图.html)

辅助文件：

- [00-范围与证据规则.md](00-范围与证据规则.md)
- [evidence/evidence-ledger.md](evidence/evidence-ledger.md)
- `evidence/page-captures/`：18 份 URL + 可见文本 + DOM 快照
- `evidence/screenshots/README.md`：截图接口缺口说明
- [delivery/README.md](delivery/README.md)

## 最强结论

StarAsk 的产品核心并不是一次“AI 算命回答”，而是一个围绕个人档案持续生长的关系与时间上下文系统：问题可以变成可回访事件，好友在权限范围内成为分析对象，日常节奏、性格卡、报告和订阅额度共享同一用户入口。当前最需要验证的是结果面、计费失败/退款、好友权限撤回，以及面相/掌纹等敏感资产的全生命周期。
