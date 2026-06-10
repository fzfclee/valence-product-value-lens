# Value Taxonomy

This taxonomy supports entry-level value framing for a single digital product. It borrows the Cost of Delay logic from SAFe WSJF, but this skill does not calculate WSJF scores, rank work, or make portfolio decisions.

## Level 1A: User-Business Value

Products directly or indirectly create regular business value for users, business teams, or the organization. Value may show up through revenue, cost, efficiency, experience, quality, visibility, or decision improvement.

### 1A.1 Revenue Growth / 增收

Applies to ecommerce, marketing conversion, sales enablement, customer conversion, dealer/store/private-domain growth, recommendation, promotion, membership, and lead conversion products.

Typical questions: Does it create more orders, improve conversion, increase basket size, improve repeat purchase, improve sales success, or expand customer/channel coverage?

Key metrics: traffic base, leads, conversion rate, conversion lift, order count, average order value, gross margin, repeat purchase, sales success rate, attribution ratio, control group or baseline.

Calculation path: incremental gross profit = impacted base x conversion lift x average order value x gross margin x attribution ratio. Alternative: incremental gross profit = new orders x average order value x gross margin x attribution ratio.

Pitfalls: Do not attribute all sales growth to the product. Exclude promotion, pricing, media spend, seasonality, and channel changes. If attribution is weak, state it as a revenue hypothesis.

### 1A.2 Cost Saving / 直接降本

Applies to reduced supplier fees, outsourcing fees, license/tool spend, paper/printing/logistics/offline material cost, or retired legacy services.

Typical questions: Which cost was actually cancelled or reduced? Is it reflected in budget or contracts? Is it one-time or recurring? Can finance confirm it?

Key metrics: original annual cost, new annual cost, cancelled supplier/license/outsourcing cost, material/logistics cost reduction, timing, budget reduction or avoided spend confirmation.

Calculation path: annual direct saving = original annual cost - new annual cost. Alternative: annual direct saving = cancelled cost + reduced cost.

Pitfalls: If budget did not reduce, the value may be Cost Avoidance or Productivity Gain rather than Cost Saving.

### 1A.3 Cost Avoidance / 成本避免

Applies to avoiding new FTE, outsourcing, duplicate builds, future procurement, system replacement, or scaling support without linear cost growth.

Typical questions: Without this product, what extra cost would occur? How many FTE or external days would be needed? What would be purchased or rebuilt? Is there a real baseline scenario?

Key metrics: avoided FTE, annual fully loaded FTE cost, avoided external days, day rate, avoided procurement amount, duplicate build count, build cost per project, baseline scenario.

Calculation path: avoided cost = avoided FTE x annual fully loaded FTE cost; or avoided external days x day rate; or avoided duplicate builds x build cost x attribution ratio.

Pitfalls: Cost Avoidance is not the same as confirmed budget saving. Describe the counterfactual scenario clearly.

### 1A.4 Productivity Gain / 效率提升

Applies to report automation, workflow approval, e-contracts, knowledge assistants, collaboration tools, sales record tools, workflow tools, and automated document/content generation.

Typical questions: Which role saves real labor time? Is it calendar time or labor time? How often is it used? How many users are covered? Is time saving confirmed by business users?

Key metrics: active users, usage frequency, labor time saved per use, annual volume, role type, labor hourly cost, discount factor, confirmation method, adoption rate.

Calculation path: productivity value = active users x usage frequency x time saved per use x annual cycles x labor hourly cost x discount factor. Alternative: annual volume x time saved per transaction x labor hourly cost x discount factor.

Pitfalls: Reducing elapsed time from 7 days to 2 days does not automatically save 5 person-days. Use a 20%-50% discount factor when evidence is weak. In Haleon-style value language, some Productivity Gain may map to Cost Avoidance rather than Cost Saving.

### 1A.5 Experience / Service Quality Improvement / 体验与服务质量提升

Applies to employee experience platforms, customer service tools, dealer portals, store tools, mobile apps, self-service, and UX improvements.

Typical questions: Does it improve satisfaction, reduce complaints, reduce waiting time, improve self-service completion, improve adoption/retention, or indirectly affect business results?

Key metrics: NPS, CSAT, complaints, waiting time, self-service completion, adoption, retention, task completion, repeat usage, support ticket reduction, user feedback.

Calculation path: usually use proxy metrics first: NPS lift, complaint reduction, completion lift, adoption lift. Monetize only when there is a credible link to revenue, productivity, or cost.

Pitfalls: Do not equate satisfaction improvement with financial value unless the business linkage is evidenced.

### 1A.6 Decision Quality / Management Visibility / 决策质量与管理可视化

Applies to management dashboards, BI reports, data products, performance dashboards, sales/inventory/supply-chain monitoring, and alerting tools.

Typical questions: Who uses the information to make decisions? How often? Are decisions faster, better, or earlier? Does it reduce manual reporting, meetings, communication cost, inventory, expense, waste, or execution variance?

Key metrics: active viewers, view frequency, decision scenario, manual report time saved, decision cycle reduction, anomaly lead time, error reduction, improved business metrics, attribution ratio.

Calculation path: base productivity value = report production time saved + user lookup/communication time saved. Business improvement value = improved business metric amount x attribution ratio.

Pitfalls: BI/dashboard value cannot be judged by page views alone. The key question is what decision or action changed after visibility improved.

## Level 1B: Time Criticality

Value is connected to a time window. Delay may reduce value or cause extra loss. This is not the product's regular value; it is the loss from late delivery or late response.

### 1B.1 Deadline-Driven Business Value / 截止日期驱动价值

Applies to campaign launch, new product launch, peak promotion, fiscal/quarter target, market window, regulatory date, or contract commitment.

Metrics: deadline date, affected sales, affected customers/stores/channels, missed opportunity, delay days/weeks, weekly/monthly decay, related campaign/launch/compliance date.

Calculation path: delay loss = expected value per period x delayed periods x decay ratio; or missed window loss = affected business amount x gross margin x attribution ratio.

Pitfall: Time criticality is not the same as "the boss is urgent." The time window and economic impact must be described.

### 1B.2 Operational Continuity / 运营连续性

Applies to factory, supply chain, order, payment, store, customer service, critical interface, or platform operation.

Metrics: affected business scope, hourly/daily loss, order volume, production volume, downtime, SLA, incident frequency, recovery time, workaround cost.

Calculation path: interruption loss = interruption duration x hourly/daily business loss. Workaround cost = affected people x extra labor time x labor hourly cost.

Pitfall: Critical systems may have low visible usage but high business criticality.

### 1B.3 Value Decay / 价值衰减

Applies to fast-changing market opportunities, competitor windows, customer demand windows, seasonal demand, policy windows, or time-sensitive data products.

Metrics: window length, monthly decay rate, competitor/substitute risk, customer willingness to wait, opportunity size, demand heat, data validity period.

Calculation path: remaining opportunity value = original opportunity value x remaining window ratio. Delay loss = original opportunity value x decay rate x delay period.

Pitfall: This is often imprecise. Treat it first as a time sensitivity indicator requiring owner confirmation.

### 1B.4 Compliance / Regulatory Timing / 合规时间窗口

Applies to regulation effective dates, audit remediation, security remediation, data compliance, privacy, information security, quality, pharma/plant compliance.

Metrics: regulatory deadline, audit remediation date, potential fine, shutdown/production impact, affected business scale, compliance owner confirmation, risk level.

Calculation path: compliance delay risk = potential impact x probability x exposure period.

Pitfall: Do not hard-code a single-point ROI. Require legal, compliance, security, QA, or relevant owner confirmation.

## Level 1C: Risk Reduction / Opportunity Enablement

Products may not directly create current revenue or savings, but they reduce future risk or enable future options, platform capability, strategic capability, and reuse.

### 1C.1 Risk Reduction / 风险降低

Applies to information security, data governance, access control, RAI/AI governance, audit trail, compliance systems, quality control, risk monitoring, approval, risk control, and traceability tools.

Metrics: risk event type, potential impact, probability, reduction ratio, affected scope, audit findings, security incidents, compliance remediation items, owner endorsement.

Calculation path: risk reduction value = potential impact x probability x risk reduction ratio.

Pitfall: Risk value should often be a range and needs owner confirmation. Adoption rate alone is not enough.

### 1C.2 Opportunity Enablement / 机会赋能

Applies to new business capability, new channel capability, AI capability, data capability, design thinking capability, commercial pilots, productization capability, and new scenario exploration.

Metrics: pilots supported, new scenarios, future opportunity size, reuse count, future project launch time reduction, future pipeline value, capability maturity, business option created.

Calculation path: use milestone-based value, option value hypothesis, future pipeline value, reuse potential, or capability maturity indicator.

Pitfall: Do not count future opportunity as current ROI. Define validation milestones.

### 1C.3 Platform Enablement / 平台赋能

Applies to API platforms, data platforms, unified entry points, middle platforms, monitoring, DevOps/observability, enterprise portals, and shared capabilities.

Metrics: downstream applications, teams onboarded, API calls, reuse count, avoided duplicate build cost, platform run cost, incident reduction, time-to-market reduction, onboarding time reduction, dependency criticality.

Calculation path: platform value = avoided duplicate build cost + downstream reuse value + operations efficiency value + risk reduction value.

Pitfall: Do not judge a platform only with single-product ROI. Separate direct value and attributed downstream value.

### 1C.4 Strategic Capability / 战略能力建设

Applies to AI capability, innovation tooling, design capability, new operating model, data foundation, organizational capability, skilling platforms, and early-stage exploration.

Metrics: capability maturity, milestone completion, pilots supported, reusable assets created, trained users/teams, adoption by strategic users, strategic initiative linkage, reuse potential, future roadmap.

Calculation path: use milestone-based value: capability built, pilots supported, reuse, lower future start-up cost, inclusion in business roadmap.

Pitfall: Do not force short-term ROI. Use sponsor confirmation of strategic relevance.

### 1C.5 Learning / Validation Value / 学习与验证价值

Applies to PoC, MVP, innovation experiments, early AI experiments, product discovery, and business model validation.

Metrics: assumptions tested, experiment cost, avoided wrong investment, learning, go/no-go criteria, user feedback, pilot adoption, validated/invalidated assumptions.

Calculation path: use avoided wrong investment, validated learning, decision quality improvement, and next-stage investment confidence.

Pitfall: Learning value is not an excuse for endless pilots. Require explicit hypotheses, time limits, and next decision criteria.

## Haleon Category Mapping

| Haleon category | Mapping in this skill | Notes |
| --- | --- | --- |
| Revenue Growth | User-Business Value -> Revenue Growth | Use only where there is credible conversion, order, margin, or attribution evidence. |
| Cost Saving | User-Business Value -> Cost Saving | Prefer finance or budget owner confirmation. |
| Cost Avoidance | User-Business Value -> Cost Avoidance | May also cover parts of Productivity Gain, Platform Enablement, or Risk Reduction. |
| Productivity Gain | Separate User-Business Value path | In Haleon language it may map to Cost Avoidance, but it needs distinct metric checks. |
| Risk Reduction | Risk Reduction / Opportunity Enablement -> Risk Reduction | May be under-emphasized in a simplified three-category view; keep it for compliance, security, quality, and continuity products. |
| Opportunity Enablement / Strategic Capability | Risk Reduction / Opportunity Enablement | Often unclear in a three-category view, but important for AI, platform, and strategic capability products. |

