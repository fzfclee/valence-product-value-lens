# Conversation Flow

Run this as an adaptive guided wizard. Ask exactly one question at a time unless the user explicitly asks for a batch intake. Use options first, then short optional free text. Do not ask for sensitive details.

Do not run this as a fixed seven-step questionnaire. Step 1 routes the conversation. Step 2 selects a likely branch. Every later question must be narrowed by the user's previous answer.

## Step 0: Safety and Input Framing

Say:

> 不需要提供公司名、产品真名、客户名、合同、截图、内部文档或敏感数据。可以使用匿名描述、模糊数字、区间数字或 Not sure。

## Step 1: Product Audience / 主要用户是谁？

Question: 这个数字产品主要给谁使用？

A. 一线销售 / 商务团队  
B. 市场 / 品牌 / 内容团队  
C. 经销商 / 门店 / 外部合作伙伴  
D. 客户 / 消费者 / 患者 / 会员  
E. 管理层 / 决策者  
F. 财务 / HR / 法务 / 采购等职能团队  
G. 工厂 / 供应链 / 运营团队  
H. IT / D&T / 数据 / 平台团队  
I. 全体员工  
J. Other / 其他，请填写  
K. Not sure / 不确定

After the answer, acknowledge the routing implication in one sentence, then ask the narrowed Step 2 question.

Example:

> 收到，主要用户是 IT / D&T / 数据 / 平台团队。我会优先判断它是平台赋能、风险控制、AI 能力、运营连续性，还是内部效率工具。

## Step 2: Product Function / 产品主要做什么？

Choose the option set based on Step 1. Do not show all options when a narrower set is available.

### Step 2A: If Step 1 = A / 一线销售 / 商务团队

Question: 对销售团队来说，这个产品主要解决什么问题？

A. 提升销售拜访、门店执行或客户跟进效率  
B. 提升线索转化、成交率、复购或客单价  
C. 提供销售数据、客户洞察或管理看板  
D. 减少手工记录、Excel、邮件或重复填报  
E. 支撑销售合规、审批、价格或合同风险控制  
F. Other / 其他，请填写  
G. Not sure / 不确定

Likely branches: Revenue Growth, Productivity Gain, Decision Quality, Risk Reduction.

### Step 2B: If Step 1 = B / 市场、品牌、内容团队

Question: 对市场 / 品牌 / 内容团队来说，这个产品主要做什么？

A. 提升营销触达、活动执行或内容分发  
B. 提升内容生产效率或知识复用  
C. 提供 campaign / brand / content performance 看板  
D. 支撑 AI 内容生成、创意试点或新能力建设  
E. 降低供应商、agency、制作或素材成本  
F. Other / 其他，请填写  
G. Not sure / 不确定

Likely branches: Revenue Growth, Productivity Gain, Decision Quality, Strategic Capability, Cost Saving/Avoidance.

### Step 2C: If Step 1 = C or D / 外部伙伴或客户用户

Question: 对外部用户来说，这个产品主要改善什么？

A. 提升转化、下单、复购或会员增长  
B. 提升自助服务、任务完成率或体验  
C. 减少投诉、等待时间或人工客服压力  
D. 支撑经销商 / 门店 / 合作伙伴运营效率  
E. 提供外部数据、订单、库存或服务可视化  
F. Other / 其他，请填写  
G. Not sure / 不确定

Likely branches: Revenue Growth, Experience, Productivity Gain, Decision Quality.

### Step 2D: If Step 1 = E / 管理层、决策者

Question: 对管理层来说，这个产品主要支持什么决策或动作？

A. 管理驾驶舱 / BI / performance visibility  
B. 异常预警、风险提示或运营监控  
C. 投资、资源、预算或 portfolio 讨论的事实基础  
D. 销售、库存、供应链、财务等业务决策提速  
E. 减少手工做表、会议沟通或信息查找  
F. Other / 其他，请填写  
G. Not sure / 不确定

Likely branches: Decision Quality, Productivity Gain, Risk Reduction, Operational Continuity.

### Step 2E: If Step 1 = F / 职能团队

Question: 对职能团队来说，这个产品主要解决什么？

A. 自动化审批、合同、采购、HR、财务等流程  
B. 替代纸质、Excel、邮件、微信群等手工作业  
C. 降低 vendor、license、外包、物料或流程成本  
D. 支撑合规、审计、权限、质量或风险控制  
E. 提供职能管理看板或服务质量指标  
F. Other / 其他，请填写  
G. Not sure / 不确定

Likely branches: Productivity Gain, Cost Saving, Cost Avoidance, Risk Reduction, Decision Quality.

### Step 2F: If Step 1 = G / 工厂、供应链、运营团队

Question: 对工厂 / 供应链 / 运营团队来说，这个产品主要保障或改善什么？

A. 保障订单、生产、供应链或门店运营连续性  
B. 减少停机、故障、异常处理或人工 workaround  
C. 提升计划、库存、预测、排产或履约可视化  
D. 支撑质量、安全、审计或合规控制  
E. 降低运营、物流、库存、外包或材料成本  
F. Other / 其他，请填写  
G. Not sure / 不确定

Likely branches: Operational Continuity, Productivity Gain, Decision Quality, Risk Reduction, Cost Saving/Avoidance.

### Step 2G: If Step 1 = H / IT / D&T / 数据 / 平台团队

Question: 对 IT / D&T / 数据 / 平台团队来说，这个产品最接近哪一类？

A. API / 数据平台 / 中台 / 统一入口等共享平台能力  
B. 数据治理、权限、安全、审计、RAI 或合规控制  
C. DevOps / observability / 监控 / 稳定性 / 运维连续性  
D. AI capability、知识助手、创新试点或新能力建设  
E. 自动化内部流程，减少工单、手工处理或重复支持  
F. 管理看板、数据产品或决策可视化  
G. Other / 其他，请填写  
H. Not sure / 不确定

Likely branches: Platform Enablement, Risk Reduction, Operational Continuity, Strategic Capability, Learning Value, Productivity Gain, Decision Quality.

### Step 2H: If Step 1 = I / 全体员工

Question: 对全体员工来说，这个产品主要改善什么？

A. 员工自助服务、体验或任务完成率  
B. 知识获取、协作、内容生成或办公效率  
C. 审批、流程、合同、采购、HR、财务等内部服务  
D. 合规、安全、权限、培训或风险控制  
E. 企业统一入口、门户或平台能力  
F. Other / 其他，请填写  
G. Not sure / 不确定

Likely branches: Experience, Productivity Gain, Cost Avoidance, Risk Reduction, Platform Enablement.

### Step 2I: If Step 1 = Other or Not sure

Question: 先粗略判断一下，这个产品更像哪类？

A. 增长 / 销售 / 客户转化工具  
B. 流程自动化 / 效率工具  
C. 报表 / 数据洞察 / 管理驾驶舱  
D. 合规 / 风险 / 安全 / 审计工具  
E. 平台 / API / 数据底座 / 中台能力  
F. AI / 创新 / PoC / 新能力建设  
G. 关键运营系统 / 稳定性保障  
H. Other / 其他，请填写  
I. Not sure / 不确定

## Branch-Specific Next Questions

After Step 2, select one branch and ask only the next question in that branch. Do not continue with the generic stage/pain-point list.

### Branch P: Platform Enablement

Use when Step 2 is platform/API/data/middleware/shared capability.

Next question P1: 这个平台现在主要被谁复用？

A. 多个下游产品 / 应用  
B. 多个业务团队  
C. 主要是一个核心系统依赖  
D. 还在建设中，尚未明显复用  
E. Other / 其他，请填写  
F. Not sure / 不确定

Then P2: 你现在能看到哪些平台证据？可以多选。

A. 下游系统数量  
B. 接入团队数量  
C. API calls / 数据调用量  
D. 复用次数或复用场景  
E. 避免重复建设的案例  
F. 年度 run cost  
G. SLA / incident / 稳定性数据  
H. Owner 或 finance 确认  
I. 目前几乎没有数据  
J. Other / 其他，请填写  
K. Not sure / 不确定

Then P3 if needed: 平台价值目前更像哪一种？

A. 避免重复建设 / Cost Avoidance  
B. 支撑下游产品 / Platform Enablement  
C. 保障关键依赖 / Operational Continuity  
D. 降低运维或支持成本 / Productivity Gain  
E. Not sure / 不确定

### Branch R: Risk / Compliance / Security

Next question R1: 它主要降低哪类风险？

A. 合规 / 监管 / 审计风险  
B. 信息安全 / 权限 / 数据泄露风险  
C. 质量 / 追溯 / 操作风险  
D. AI / RAI / 模型或内容风险  
E. Other / 其他，请填写  
F. Not sure / 不确定

Then R2: 你现在有哪些风险证据？可以多选。

A. 审计发现 / 整改项  
B. 风险事件或异常记录  
C. 风险等级或潜在影响区间  
D. 合规 / 安全 / QA owner 确认  
E. deadline 或监管 / 审计时间窗口  
F. 目前几乎没有数据  
G. Other / 其他，请填写  
H. Not sure / 不确定

### Branch O: Operational Continuity

Next question O1: 如果这个产品不可用，主要影响什么？

A. 订单 / 支付 / 交易  
B. 生产 / 工厂 / 供应链  
C. 门店 / 客服 / 外部服务  
D. 关键接口 / 平台依赖  
E. 只是内部效率下降，不影响连续性  
F. Other / 其他，请填写  
G. Not sure / 不确定

Then O2: 你有哪些连续性数据？

A. SLA / downtime  
B. incident frequency  
C. 每小时 / 每天影响量  
D. workaround 人工成本  
E. 受影响系统 / 团队 / 区域范围  
F. 目前几乎没有数据  
G. Other / 其他，请填写  
H. Not sure / 不确定

### Branch A: AI / Innovation / Strategic Capability

Next question A1: 这个产品当前更像哪一类？

A. AI 内容生成 / 知识助手 / 办公效率  
B. AI governance / RAI / 风险控制  
C. PoC / MVP / innovation experiment  
D. 数据 / AI capability foundation  
E. 已经进入稳定业务使用  
F. Other / 其他，请填写  
G. Not sure / 不确定

Then A2: 现在最能证明价值的证据是什么？

A. 活跃试点用户和使用频次  
B. 单次节省时间或质量提升  
C. validated / invalidated hypotheses  
D. 支撑的业务试点或未来机会  
E. sponsor 确认的战略能力里程碑  
F. 目前几乎没有数据  
G. Other / 其他，请填写  
H. Not sure / 不确定

### Branch D: Decision Quality / Dashboard

Next question D1: 这个看板 / 数据产品主要支持什么动作？

A. 替代手工报表  
B. 提前发现异常或风险  
C. 支持业务会议和管理决策  
D. 改善销售 / 库存 / 供应链 / 财务等业务指标  
E. 只是信息展示，决策动作还不清楚  
F. Other / 其他，请填写  
G. Not sure / 不确定

Then D2: 你有哪些数据？

A. 活跃查看人数  
B. 查看频次  
C. 手工报表节省时间  
D. 决策动作或业务改善案例  
E. 业务指标变化  
F. Owner 确认  
G. 目前几乎没有数据  
H. Other / 其他，请填写  
I. Not sure / 不确定

### Branch W: Workflow / Productivity / Cost

Next question W1: 这个工具主要替代了什么？

A. 人工处理时间  
B. 纸质 / Excel / 邮件 / 微信群  
C. 外包 / vendor / license / 物料费用  
D. 未来新增人手或重复建设  
E. 等待时间或审批周期，但实际人工节省不确定  
F. Other / 其他，请填写  
G. Not sure / 不确定

Then W2: 你有哪些效率或成本数据？

A. 活跃用户数  
B. 使用频次 / 年处理量  
C. 单次节省人工时间  
D. 人工小时成本或角色成本  
E. 原成本 / 新成本 / 被取消费用  
F. finance 或 process owner 确认  
G. 目前几乎没有数据  
H. Other / 其他，请填写  
I. Not sure / 不确定

### Branch G: Revenue / Growth

Next question G1: 增长更可能来自哪里？

A. 更多流量 / 线索  
B. 更高转化率 / 成交率  
C. 更高客单价 / 复购  
D. 更好销售覆盖或客户跟进  
E. 只是增长假设，还没有证据  
F. Other / 其他，请填写  
G. Not sure / 不确定

Then G2: 你有哪些增长数据？

A. 流量 / 线索 / 客户基数  
B. 转化率 / 成交率  
C. 订单数 / 客单价 / 毛利率  
D. baseline / control group  
E. attribution assumption  
F. business owner 确认  
G. 目前几乎没有数据  
H. Other / 其他，请填写  
I. Not sure / 不确定

## Legacy Full Option Bank

Use this full option bank only when the user explicitly asks to see all options, wants a batch intake, or the branch cannot be inferred.

Question: 这个产品主要帮助用户完成什么事情？

A. 提升销售、转化或客户增长  
B. 提升营销触达、内容生产或活动执行  
C. 自动化流程，减少人工处理  
D. 替代纸质、Excel、邮件、微信群等手工作业  
E. 提供报表、数据洞察或管理驾驶舱  
F. 提升协作、审批、任务跟踪或知识获取效率  
G. 支撑合规、审计、安全、质量或风险控制  
H. 支撑平台能力，例如 API、数据平台、中台、统一入口  
I. 支撑 AI、创新试点或新能力建设  
J. 保障关键系统运行或运营连续性  
K. Other / 其他，请填写  
L. Not sure / 不确定

## Generic Step 3: Product Stage / 当前状态是什么？

Question: 这个产品现在处于什么阶段？

A. 想法阶段 / 尚未启动  
B. PoC / MVP / 试点中  
C. 已上线，但使用有限  
D. 已上线，已有稳定使用  
E. 已推广，但价值不清楚  
F. 老系统，持续维护中  
G. 正在考虑优化、合并或停用  
H. Other / 其他，请填写  
I. Not sure / 不确定

## Generic Step 4: Main Pain Point / 过去主要痛点是什么？

Question: 没有这个产品之前，主要问题是什么？

A. 销售或业务增长受限  
B. 人工处理太慢 / 重复劳动太多  
C. 成本太高，例如外包、供应商、license、物料等  
D. 数据分散，看不清业务情况  
E. 决策慢、决策不准、异常发现晚  
F. 用户体验差、投诉多、使用不方便  
G. 合规、审计、安全或质量风险较高  
H. 系统不稳定，影响运营连续性  
I. 重复建设多，平台复用差  
J. 新能力缺失，影响未来机会  
K. Other / 其他，请填写  
L. Not sure / 不确定

## Generic Step 5: Expected Value Direction / 你认为它主要创造什么价值？

Question: 你认为这个产品最可能带来哪类价值？可以多选。

A. Revenue Growth / 增收  
B. Cost Saving / 直接降本  
C. Cost Avoidance / 成本避免  
D. Productivity Gain / 效率提升  
E. Experience or Service Quality Improvement / 体验或服务质量提升  
F. Decision Quality or Management Visibility / 决策质量或管理可视化  
G. Time Criticality / 时间窗口价值  
H. Risk Reduction / 风险降低  
I. Opportunity Enablement / 机会赋能  
J. Platform Enablement / 平台赋能  
K. Strategic Capability / 战略能力建设  
L. Learning / Validation Value / 学习与验证价值  
M. Not sure / 不确定  
N. Other / 其他，请填写

If the user's selection conflicts with prior answers, say:

> 你选择了 X，但根据当前描述，Y 可能也是重要价值路径。是否也需要纳入？

## Generic Step 6: Available Data / 你现在有哪些数据？

Question: 你现在已经有哪些数据？可以多选。

A. 实际活跃用户数  
B. 目标用户总数  
C. 使用频次  
D. 处理量 / 交易量 / 订单量  
E. 单次节省时间  
F. 人工成本或角色成本  
G. 年度 run cost  
H. Vendor / license / support cost  
I. 原流程成本或旧系统成本  
J. 转化率 / 成交率 / 客单价 / 毛利率  
K. NPS / 满意度 / 投诉量 / 体验指标  
L. 错误率 / 异常率 / 审计发现 / 风险事件  
M. SLA / 停机时间 / 故障损失  
N. 下游系统数量 / 复用次数 / API calls  
O. 业务 owner 或 finance 已确认的数据  
P. 目前几乎没有数据  
Q. Not sure / 不确定  
R. Other / 其他，请填写

Do not immediately say the user "lacks" data. First generate the recommended data checklist for the likely value path, then compare it with the user's selected available data.

## Step 7: Optional Short Free Text

Say:

> 如愿意，可以用一句话补充这个产品的具体场景。不需要提供公司名、产品真名或敏感信息。

This step is optional.

## Clarifying Questions

After Step 1-7, ask at most 3 questions only when needed to resolve conflict or uncertainty. Examples:

- 这个产品是否已经有真实用户，还是仍在 PoC？
- 它主要替代了人工流程，还是主要改善管理可视化？
- 它是否存在明确 deadline、合规要求或运营连续性风险？

If the user does not answer, produce the initial result and mark uncertainty.

## Classification Heuristics

- Sales, ecommerce, conversion, lead, promotion, and member products usually start with Revenue Growth.
- Workflow automation, e-contracts, reporting production, knowledge assistant, and internal operations tools usually start with Productivity Gain, sometimes Cost Avoidance.
- Confirmed budget/license/vendor removal usually maps to Cost Saving.
- Avoided hiring, avoided outsourcing, avoided duplicate build, or platform reuse usually maps to Cost Avoidance or Platform Enablement.
- Dashboards and BI usually map to Decision Quality / Management Visibility plus Productivity Gain if manual reporting is reduced.
- Compliance, security, QA, audit, access control, and traceability products usually map to Risk Reduction and possibly Compliance / Regulatory Timing.
- Factory, order, payment, supply-chain, store, or critical interface products usually map to Operational Continuity.
- API, data platform, middleware, enterprise portal, and shared capability products usually map to Platform Enablement.
- AI capability, innovation tooling, design capability, and early capability building usually map to Strategic Capability or Opportunity Enablement.
- PoC/MVP/experiments usually map to Learning / Validation Value until there is strong adoption or business evidence.

## Data Maturity Model

| Level | Name | Criteria | Output stance |
| --- | --- | --- | --- |
| 0 | Product Story Only | Only description or rough options | Value logic draft only |
| 1 | Value Logic Draft Ready | Product type and value path clear, key data missing | Metrics and data collection plan |
| 2 | Rough Estimate Possible | Some adoption, usage, cost, or proxy data | Rough estimate with limitations |
| 3 | Evidence Review Ready | Adoption, cost, business value evidence, and owner confirmation | Recommend formal diagnostic |
| 4 | Governance Review Ready | Data complete enough for portfolio/leadership review | Recommend formal Valence review, no governance conclusion |

