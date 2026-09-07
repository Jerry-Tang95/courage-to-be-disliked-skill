# 被讨厌勇气量表 — 压力测试结果

- **skill slug**: `courage-to-be-disliked`
- **测试日期**: 2026-08-25
- **测试方式**: 独立 sub-agent 盲测 (不提供 type/expected/notes; 给出同书 9 个 skill 名称+描述作候选池, 模拟真实激活选择)
- **用例数**: 8 (should_trigger 3 / should_not_trigger 3 / edge_case 2)

## 通过率

**8/8 (100%)** — 修正后全部通过 (初测 8/8, 详见修复记录)

## 逐条结果

| 用例 | 类型 | 预期激活 | 盲测判定 | 结果 |
|---|---|---|---|---|
| should-trigger-01 | should_trigger | courage-to-be-disliked | courage-to-be-disliked | PASS |
| should-trigger-02 | should_trigger | courage-to-be-disliked | courage-to-be-disliked | PASS |
| should-trigger-03 | should_trigger | courage-to-be-disliked | courage-to-be-disliked | PASS |
| should-not-trigger-01 | should_not_trigger | community-feeling | community-feeling | PASS |
| should-not-trigger-02 | should_not_trigger | task-separation/decompete | task-separation | PASS |
| should-not-trigger-03 | should_not_trigger | none | none | PASS |
| edge-01 | edge_case | none(毒性共同体先自保) | none(先退出/求助) | PASS |
| edge-02 | edge_case | 修复关系而非自由代价 | none(引导复盘修复) | PASS |

## 失败与修复记录

首轮盲测即 100% 通过, 无需修复。

## 结论

**接受** — 通过率 100%, trigger 精准且诱饵(含跨 skill 混淆)全部正确忍住/分流, 无需回炉阶段 2。
