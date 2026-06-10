# Valence Product Value Lens - 3 Scenario Test Results

Test date: 2026-06-11  
Skill under test: `valence-product-value-lens` / Valence Product Value Lens  
Install path example: `~/.codex/skills/valence-product-value-lens/`

## Pass Criteria

- Uses option-based wizard input rather than open-ended questionnaire.
- Produces product type, audience, core use case, likely value path, suggested value logic, recommended metrics, data maturity level, what-not-to-do, next step, and CTA.
- Does not output formal ROI, product shutdown, investment, portfolio ranking, or full Valence governance conclusion.
- Includes the lead-generation CTA into Product Value Diagnostic / Valence review.

## Scenario 1: Sales Visit / Store Execution Tool

### Wizard Input

- Step 1 Product Audience: A. 一线销售 / 商务团队
- Step 2 Product Function: A. 提升销售、转化或客户增长; F. 提升协作、审批、任务跟踪或知识获取效率
- Step 3 Product Stage: E. 已推广，但价值不清楚
- Step 4 Main Pain Point: A. 销售或业务增长受限; B. 人工处理太慢 / 重复劳动太多
- Step 5 Expected Value Direction: A. Revenue Growth; D. Productivity Gain; F. Decision Quality / Management Visibility
- Step 6 Available Data: A. 实际活跃用户数; B. 目标用户总数; C. 使用频次; D. 处理量 / 交易量 / 订单量; Q. Not sure
- Step 7 Context: 匿名销售拜访和门店执行工具，用于记录拜访、任务完成和门店反馈。

### Clarifying Questions Used

1. 这个产品的主要目标更偏向销售转化，还是拜访效率和执行透明度？
2. 是否有 rollout 前后的 sales conversion / visit completion baseline？
3. 是否已有 business owner 确认该工具对销售结果的贡献？

### Result Summary

# Valence Product Value Lens Result

## 1. Product Type
Sales execution / field-force productivity product.

## 2. Primary Users / Audience
一线销售 / 商务团队。

## 3. Core Use Case
帮助销售记录拜访、跟踪门店执行任务、提高现场执行透明度，并可能间接改善销售覆盖质量。

## 4. Likely Value Path
- User-Business Value -> Productivity Gain
- User-Business Value -> Decision Quality / Management Visibility
- User-Business Value -> Revenue Growth

## 5. Suggested Value Logic
当前应以 Productivity Gain 和 Decision Quality / Management Visibility 作为主价值口径。Revenue Growth 可以作为次级价值假设，但需要 conversion lift、订单变化、baseline 和 attribution 证据后再进入估算。

## 6. Recommended Metrics to Collect

| Metric | Why It Matters | Suggested Owner | User Has It? |
| ------ | -------------- | --------------- | ------------ |
| Active users | Confirms adoption | Product owner | Yes |
| Target user base | Shows coverage | Sales operations | Yes |
| Usage frequency | Indicates repeated use | Product owner | Yes |
| Visit / task volume | Connects usage to work output | Sales operations | Yes |
| Conversion or order lift | Tests revenue hypothesis | Sales owner | Not selected |
| Baseline before rollout | Enables comparison | Sales operations | Not selected |
| Business owner confirmation | Reduces over-attribution | Business owner | Not sure |

## 7. Data Maturity Level
Level 1: Value Logic Draft Ready. Usage data exists, but value evidence and owner confirmation are not yet strong enough for reliable value estimation.

## 8. What Not To Do
- 不要把“销售使用了工具”直接等同于“销售增长由工具产生”。
- 不要把所有销售增长都归因于产品。
- 不要把记录拜访数量直接当成业务价值。

## 9. Recommended Next Step
补齐 rollout 前后 visit completion、sales conversion proxy、订单或覆盖改善数据，并找 sales business owner 确认价值口径。

## 10. CTA
如果你有多个数字产品需要统一价值口径、adoption、cost 和 value evidence，可以进入正式 Product Value Diagnostic / Valence review。这个 Skill 只帮助完成单产品的价值口径和数据准备度自查，不替代正式治理评估。

### Pass Judgment

PASS. The output identifies a conservative value path and includes a clear CTA into formal Product Value Diagnostic / Valence review.

## Scenario 2: Compliance / Risk Control System

### Wizard Input

- Step 1 Product Audience: F. 财务 / HR / 法务 / 采购等职能团队; H. IT / D&T / 数据 / 平台团队
- Step 2 Product Function: G. 支撑合规、审计、安全、质量或风险控制
- Step 3 Product Stage: D. 已上线，已有稳定使用
- Step 4 Main Pain Point: G. 合规、审计、安全或质量风险较高
- Step 5 Expected Value Direction: H. Risk Reduction
- Step 6 Available Data: L. 错误率 / 异常率 / 审计发现 / 风险事件; O. 业务 owner 或 finance 已确认的数据
- Step 7 Context: 匿名权限审批和审计留痕系统，用于敏感操作控制。

### Clarifying Questions Used

1. 是否存在明确 regulatory deadline 或 audit remediation deadline？
2. 风险降低口径由 compliance / security / audit 哪个 owner 确认？
3. 当前是否能描述潜在影响范围，而不是具体敏感金额？

### Result Summary

# Valence Product Value Lens Result

## 1. Product Type
Compliance / access control / audit trail product.

## 2. Primary Users / Audience
职能团队、IT / D&T / 数据 / 平台团队。

## 3. Core Use Case
通过权限审批、操作留痕和异常控制降低合规、审计或安全风险。

## 4. Likely Value Path
- Risk Reduction / Opportunity Enablement -> Risk Reduction
- Time Criticality -> Compliance / Regulatory Timing, if a confirmed deadline exists

## 5. Suggested Value Logic
当前应以 Risk Reduction 作为主价值口径。若存在审计整改或监管截止日期，再补充 Compliance / Regulatory Timing。该产品不适合用 adoption rate 或短期 ROI 单独判断。

## 6. Recommended Metrics to Collect

| Metric | Why It Matters | Suggested Owner | User Has It? |
| ------ | -------------- | --------------- | ------------ |
| Risk event type | Defines protected outcome | Compliance / security owner | Yes |
| Audit findings or risk events | Shows evidence baseline | Audit / compliance owner | Yes |
| Potential impact range | Frames materiality without sensitive details | Risk owner | Not selected |
| Risk reduction mechanism | Explains product contribution | IT / security owner | Not selected |
| Owner confirmation | Gives credibility | Compliance / security owner | Yes |

## 7. Data Maturity Level
Level 3: Evidence Review Ready if owner confirmation is documented. If owner confirmation is informal only, treat as Level 2 until documented.

## 8. What Not To Do
- 不要把合规系统只按 adoption rate 判断。
- 不要把 Risk Reduction 简单混同为 Cost Avoidance。
- 不要输出精确 ROI 或投资建议。

## 9. Recommended Next Step
用匿名区间补齐潜在影响范围、风险降低机制和 owner 背书记录；如涉及 deadline，再确认监管或审计时间窗口。

## 10. CTA
如果你有多个数字产品需要统一价值口径、adoption、cost 和 value evidence，可以进入正式 Product Value Diagnostic / Valence review。这个 Skill 只帮助完成单产品的价值口径和数据准备度自查，不替代正式治理评估。

### Pass Judgment

PASS. The output avoids ROI overclaiming, treats risk correctly, and routes multi-product governance need into formal Valence review.

## Scenario 3: API / Data Platform

### Wizard Input

- Step 1 Product Audience: H. IT / D&T / 数据 / 平台团队
- Step 2 Product Function: H. 支撑平台能力，例如 API、数据平台、中台、统一入口
- Step 3 Product Stage: D. 已上线，已有稳定使用
- Step 4 Main Pain Point: I. 重复建设多，平台复用差
- Step 5 Expected Value Direction: C. Cost Avoidance; J. Platform Enablement
- Step 6 Available Data: G. 年度 run cost; N. 下游系统数量 / 复用次数 / API calls; O. 业务 owner 或 finance 已确认的数据
- Step 7 Context: 匿名 API / data platform，为多个下游系统提供共用数据和接口能力。

### Clarifying Questions Used

1. 平台是否已经避免多个团队重复建设同类接口或数据处理能力？
2. 下游产品是否存在运营连续性依赖？
3. run cost 是否可与下游复用或避免重复建设成本放在同一口径比较？

### Result Summary

# Valence Product Value Lens Result

## 1. Product Type
Platform enablement / shared API and data capability.

## 2. Primary Users / Audience
IT / D&T / 数据 / 平台团队，以及依赖平台的下游产品团队。

## 3. Core Use Case
为多个下游产品提供可复用接口和数据能力，减少重复建设，并提高平台化交付效率。

## 4. Likely Value Path
- Risk Reduction / Opportunity Enablement -> Platform Enablement
- User-Business Value -> Cost Avoidance
- Time Criticality -> Operational Continuity, if downstream dependency is critical

## 5. Suggested Value Logic
平台类产品应从复用、避免重复建设、运行成本和关键依赖四个角度评估。不要只用单一产品 ROI 判断。

## 6. Recommended Metrics to Collect

| Metric | Why It Matters | Suggested Owner | User Has It? |
| ------ | -------------- | --------------- | ------------ |
| Downstream applications | Measures dependency and reuse | Platform owner | Yes |
| Reuse count / API calls | Shows platform usage depth | Platform owner | Yes |
| Avoided duplicate build cost | Supports Cost Avoidance | PMO / finance | Not selected |
| Annual run cost | Required for cost-to-value view | Platform owner | Yes |
| Dependency criticality / SLA | Tests operational continuity | IT operations | Not selected |
| Owner confirmation | Supports credibility | Platform / finance owner | Yes |

## 7. Data Maturity Level
Level 2: Rough Estimate Possible. Reuse and run cost data exists, but avoided duplicate build cost and dependency criticality need confirmation.

## 8. What Not To Do
- 不要把 Platform Enablement 简单按单一 ROI 判断。
- 不要把所有下游业务价值全部归因给平台。
- 不要忽略低可见但高关键性的下游依赖。

## 9. Recommended Next Step
建立下游应用清单，估算避免重复建设成本，标注 critical dependency，并用 finance / platform owner 确认 attribution 口径。

## 10. CTA
如果你有多个数字产品需要统一价值口径、adoption、cost 和 value evidence，可以进入正式 Product Value Diagnostic / Valence review。这个 Skill 只帮助完成单产品的价值口径和数据准备度自查，不替代正式治理评估。

### Pass Judgment

PASS. The output handles platform value without reducing it to single ROI and includes a natural lead-in to formal Product Value Diagnostic / Valence review.

## Overall Result

All 3 scenarios PASS.

The skill can generate conservative single-product value framing, identify data readiness, avoid overclaiming ROI/governance decisions, and consistently route suitable users toward formal Product Value Diagnostic / Valence review.
