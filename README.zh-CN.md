<div align="center">

# Valence 产品价值透镜

**用大约三分钟，把“这个产品已经上线”变成一条可以验证的价值实现假设。**

说清产品服务谁、解决什么问题、期待什么变化、需要什么证据、价值如何落到经济结果，以及当前产品形态是否合理。

<p>
  <a href="https://github.com/fzfclee/valence-product-value-lens/actions/workflows/validate.yml"><img src="https://img.shields.io/github/actions/workflow/status/fzfclee/valence-product-value-lens/validate.yml?branch=main&amp;style=for-the-badge&amp;label=validation" alt="Validation"></a>
  <a href="SKILL.md"><img src="https://img.shields.io/badge/lens-v0.2-0f766e?style=for-the-badge" alt="Lens v0.2"></a>
  <a href="https://github.com/fzfclee/valence-product-value-lens/stargazers"><img src="https://img.shields.io/github/stars/fzfclee/valence-product-value-lens?style=for-the-badge" alt="GitHub stars"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-2563eb?style=for-the-badge" alt="MIT license"></a>
</p>

[30 秒开始](#30-秒开始) · [价值透镜](#价值透镜) · [输出示例](#输出示例) · [质量证据](#质量证据) · [English](README.md) · [Valence](https://www.o2vframework.com/zh/valence)

</div>

---

## 为什么需要它

数字产品的价值讨论经常停得太早：

- 把“上线了”当成价值；
- 只报使用量，却没说明人的行为或业务结果发生了什么变化；
- 只要节省时间，就直接算成降本；
- 说品牌、平台复用或风险控制有价值，却没有证据链；
- 默认现有 App、看板或小程序就是正确的产品形态。

Valence 产品价值透镜让 AI 用一套轻量、重证据的方式挑战这些跳步，最终形成一条能继续验证的价值假设。

## 30 秒开始

### Codex

```powershell
git clone https://github.com/fzfclee/valence-product-value-lens.git "$env:USERPROFILE\.codex\skills\valence-product-value-lens"
```

新建任务后输入：

```text
$valence-product-value-lens
请帮我判断这个数字产品的价值假设和数据准备度：
[请描述产品，不要提供敏感信息]
```

### 其他 AI Agent

把 [`SKILL.md`](SKILL.md) 及其引用的 Markdown 文件放入 Agent 的 Skill 或项目指令目录即可。本仓库以 Markdown 为主，不需要额外运行环境。

## 价值透镜

```mermaid
flowchart LR
    W["服务谁"] --> P["核心问题"]
    P --> C["预期变化"]
    C --> E["证据指标"]
    E --> M["经济价值方向"]
    M --> F["为什么必须是这种产品形态？"]
    F --> N["下一步取证行动"]
```

它每次只问一个自适应问题，最后回答七个决策问题：

| 决策问题 | 输出 |
|---|---|
| 核心用户是谁？ | 一个主要受众 |
| 最重要的问题是什么？ | 一个核心问题 |
| 希望发生什么变化？ | 可观察的行为或结果变化 |
| 什么才算证据？ | 证据指标和当前数据缺口 |
| 经济价值落在哪里？ | 一个主要的 **Grow、Save 或 Protect** 方向 |
| 为什么需要当前产品形态？ | 产品形态挑战和替代方案 |
| 下一步做什么？ | 数据准备度和下一步行动 |

## Grow、Save、Protect

Valence 把经济结果和价值机制分开：

| 经济结果 | 含义 | 证据路径示例 |
|---|---|---|
| **Grow** | 增加收入、利润或现金流入 | 增量转化 × 单位贡献利润 |
| **Save** | 减少或避免成本和资源消耗 | 经核实的净节省时间 × 可兑现的成本或产能 |
| **Protect** | 减少收入损失、风险损失或业务中断损失 | 潜在影响 × 基准概率 × 预期下降幅度 |

效率、体验、决策质量、品牌、时效、平台复用、学习和战略能力属于价值机制。只有说明它们如何连接到 Grow、Save 或 Protect，才可以进一步讨论经济价值。

## 适用场景

| 场景 | 它帮助判断什么 |
|---|---|
| 产品已经存在，但价值说不清 | 应该围绕什么结果和证据讲价值 |
| 使用率偏低 | 问题出在用户、痛点、行为变化还是产品形态 |
| 过早被要求计算 ROI | 做方向性估算前还缺哪些数据 |
| 平台产品声称有复用价值 | 下游依赖是否真实，是否存在重复计算 |
| 合规产品看起来“使用量不高” | Protect 价值是否比使用量更重要 |
| 独立 App 或小程序受到质疑 | 其他交付形态能否创造同样的价值 |

它适合单个数字产品的早期价值讨论。正式 ROI 审批、产品组合排序、投资决策和生命周期治理需要更完整的评估。

## 输出示例

**输入**

```text
我们有一个品牌小程序，主要发布官方产品信息，但访问量不高。我不知道该怎么说明它的价值。
```

**精简输出**

```markdown
主要受众：正在比较产品的潜在客户。
核心问题：客户在做决定时不容易找到可信的官方产品信息。
预期变化：更多高意向访客看到可信信息后，继续进入购买路径。
主要经济方向：Grow，目前仍待验证。
证据指标：高意向访问中继续进入零售、留资或购买动作的比例。
方向性逻辑：增量高意向路径 × 转化提升 × 贡献利润。
产品形态问题：是否一定需要独立小程序，还是官网、零售商集成、H5 或现有平台也能提供同样的可信路径？
数据准备度：Level 1，已经可以形成价值实现草案。
下一步：打通流量来源和后续动作，先验证一个决策阶段的具体场景。
```

它不会默认“品牌曝光”天然有价值，也不会默认当前产品形态必须保留。

## 兼容环境

| Agent / 工具 | 推荐方式 |
|---|---|
| Codex | 本地 Skill 目录 |
| Claude Code | 项目或个人 Skill 目录 |
| Claude Projects | Project Instructions 加引用文件 |
| Cursor / Windsurf | 项目规则或可复用指令 |
| Hermes / OpenClaw / WorkBuddy | Markdown Skill 目录或可复用指令 |

详细的可移植运行约定见 [`runtime_compatibility.md`](runtime_compatibility.md)。

## 质量证据

本仓库明确区分结构校验和场景证据：

- **自动仓库校验：** 每次提交和 Pull Request 都检查必需文件、UTF-8、frontmatter、内部链接、核心价值规则和引用资产。
- **自适应回归案例：** [`tests/adaptive_regression.md`](tests/adaptive_regression.md) 检查用户选择平台场景后，下一个问题是否真正改变。
- **三组场景记录：** [`tests/three_scenario_tests.md`](tests/three_scenario_tests.md) 覆盖销售执行、合规与风险控制、平台赋能。
- **完整示例：** [`examples.md`](examples.md) 展示价值机制、经济方向、数据成熟度和边界如何落到输出中。

本地运行结构校验：

```powershell
python scripts/validate_repo.py
```

## 仓库结构

| 文件 | 用途 |
|---|---|
| [`SKILL.md`](SKILL.md) | 运行指令和质量边界 |
| [`conversation_flow.md`](conversation_flow.md) | 一次一个问题的自适应流程 |
| [`value_taxonomy.md`](value_taxonomy.md) | Grow / Save / Protect 与价值机制 |
| [`data_checklists.md`](data_checklists.md) | 最低证据和货币化数据 |
| [`output_templates.md`](output_templates.md) | 标准输出结构 |
| [`examples.md`](examples.md) | 完整示例 |
| [`tests/`](tests) | 回归和场景记录 |

## Valence 与 O2V

本仓库提供可独立使用的 Valence 产品价值透镜，适合单产品的轻量价值梳理。

[Valence 产品价值运营与治理模型](https://www.o2vframework.com/zh/valence)进一步覆盖价值实现设计、计划货币化价值、实际确认价值、采用率、投资效率、产品组合评审和生命周期决策。Valence 属于 [O2V Framework](https://www.o2vframework.com/zh)，用于把机会信号连接到有证据的行动和可实现价值。

本仓库原创的 Markdown Skill、示例和支持文本采用 [MIT License](LICENSE)。Valence 与 O2V 方法论资产依据 [`NOTICE.md`](NOTICE.md) 中的权利说明分别维护。

## 参与贡献

欢迎提交场景案例、兼容性说明、更清楚的证据边界和可移植性改进。提交 Pull Request 前请阅读 [`CONTRIBUTING.md`](CONTRIBUTING.md)。

方法论或咨询合作：

- 中文：微信 `lizhi_ch`
- 英文：[LinkedIn 联系 Zhi Li](https://www.linkedin.com/in/li-zhi/)

---

<div align="center">

**上线是一个事件，价值是一个有证据的变化。**

如果这个透镜帮你把产品问题想清楚了，欢迎 Star，让更多产品团队找到它。

</div>
