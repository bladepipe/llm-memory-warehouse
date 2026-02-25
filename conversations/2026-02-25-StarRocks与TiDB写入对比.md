---
date: 2026-02-25
topic: StarRocks与TiDB写入对比
summary: StarRocks以“活扣”思维优化写入吞吐与简易性，TiDB以“死扣”思维保障事务强一致与长期可溯性，二者非优劣之分，而是适用场景的哲学选择。
key_points:
- 活扣：刘震云定义为“随时间流逝而有望解开的结”，技术上指 StarRocks 对输入格式的宽容与快速响应能力
- 死扣：刘震云定义为“自我设限的心结”，技术上指 TiDB 对 ACID 的刚性保障与多副本校验机制
- flat_json_v2：StarRocks 4.0 引入的 JSON 解析器，支持直接映射嵌套字段至列存，免 ETL 拆解
action_items:
- 验证 Stream Load 失败率是否 <5%
- 检查 TiDB v7.5 中 `raftstore.apply-pool-size` 是否 ≥ `store-pool-size × 2`
- 执行 `tiup cluster check` 预检
source: conversations/2026-02-25-StarRocks与TiDB写入对比.md
---