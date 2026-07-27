# Conversation Flow v0.2

Run an adaptive wizard. Ask one question at a time.

Start with:

> 不需要提供公司名、产品真名、客户名、合同、截图或敏感数据。可以使用匿名描述、区间数字或 Not sure。

## Step 1 - Primary Audience

Question: 这个产品最主要给谁使用或服务？

A. 一线销售 / 客户经理  
B. 市场 / 品牌 / 内容团队  
C. 外部客户 / 消费者 / 患者 / 会员  
D. 管理层 / 决策者  
E. 财务 / HR / 法务 / 采购等职能角色  
F. 工厂 / 供应链 / 运营角色  
G. IT / D&T / 数据 / 平台团队或下游系统  
H. 其他  
I. 不确定

If the user says “all employees” or “all consumers,” ask which roles or situations genuinely require the core capability.

## Step 2 - Main Problem

Use audience-specific options.

### Sales / Customer-facing Staff

A. 客户关系沉淀、继承或合规  
B. 客户触达、跟进或内容分发效率  
C. 转化、成交、复购或覆盖  
D. 手工记录、重复填报或流程负担  
E. 其他 / 不确定

### Marketing / Brand / Consumer

A. 高意向用户找不到可信官方信息  
B. 营销触达、导流或转化不足  
C. 内容生产或复用成本高  
D. 服务体验、自助完成或投诉问题  
E. 其他 / 不确定

### Management / Functional Users

A. 手工报表或信息查找成本高  
B. 决策慢、异常发现晚或执行不可见  
C. 审批、合同、采购或内部服务流程低效  
D. 合规、审计、权限或风险控制不足  
E. 其他 / 不确定

### Platform / Operations

A. 重复建设、重复集成或数据加工  
B. 关键运营连续性或稳定性  
C. 运维、支持、云或 license 成本高  
D. 下游接入和复用困难  
E. 其他 / 不确定

## Step 3 - Expected Change

Question: 产品使用后，最希望看到什么变化？

A. 更多目标用户完成核心业务行为  
B. 客户转化、订单或贡献利润提高  
C. 人工工时或实际支出下降  
D. 收入、客户资产、运营或合规风险损失下降  
E. 下游复用增加、重复建设减少  
F. 其他 / 不确定

Reject “上线、培训、功能完成” as final change. Help the user restate it as behaviour or outcome.

## Step 4 - Evidence

Question: 你现在能看到哪些证据？可以多选。

A. 目标用户和真实活跃用户  
B. 核心行为完成量或频率  
C. 转化、订单、客户或业务结果  
D. 人工时间、流程量或实际成本  
E. 风险事件、影响范围或 risk tier  
F. 下游接入、复用或避免重复建设案例  
G. 年度运行成本  
H. Business / Finance / Risk owner 确认  
I. 目前几乎没有数据  
J. 其他 / 不确定

## Step 5 - Monetization Direction

Based on the expected change, ask one narrowed question.

### Grow

Which parameter is available?

A. Impacted audience / leads / customers  
B. Conversion or order baseline  
C. Incremental lift  
D. Unit contribution margin  
E. Attribution evidence  
F. Not sure

### Save

A. Annual users / transactions / process volume  
B. Net labor time saved  
C. Labor cost  
D. Actual vendor / license / material spend reduced  
E. Avoided future capacity or duplicate build  
F. Not sure

### Protect

A. Protected revenue / operation / asset  
B. Potential impact range  
C. Baseline probability or risk tier  
D. Expected reduction from the product  
E. Owner confirmation  
F. Not sure

## Step 6 - Product Form

Question: 为什么必须是现在这种产品形态？

A. 需要当前生态或设备的专有能力  
B. 需要独立身份、权限、合规或审计  
C. 当前形态能证明带来额外转化或价值  
D. 现有系统、官网、H5 或共享平台无法满足  
E. 其实没有比较过替代方案  
F. 其他 / 不确定

## Completion Rule

Produce the result when the following are reasonably clear:

- one Primary Audience;
- one Main Problem;
- one Expected Change;
- one Primary Economic Outcome;
- at least one Evidence KPI;
- a monetization direction;
- a product-form question.

Ask at most three clarifying questions after Step 6. If the user cannot answer, produce a draft and mark uncertainty.
