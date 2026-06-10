# Valence Product Value Lens

Runtime skill id: `valence-product-value-lens`. Human-facing name: `Valence Product Value Lens`.

Valence Product Value Lens is an entry-level value framing and data readiness skill. It helps users identify the right value logic for a single digital product. It does not expose or replace the full Valence Product Value Governance System.

Valence 产品价值透镜是 Valence 的前置轻量入口，用于单个数字产品的价值口径判断和数据准备度自查。它不等同于完整 Valence 产品价值治理系统，也不输出完整 portfolio 治理模型。

## What This Skill Is

Valence Product Value Lens is a guided, option-based skill. It helps users quickly classify a digital product, identify likely value paths, and understand what data would be needed for a more reliable product value assessment.

Valence 产品价值透镜是一个选项式引导 Skill，帮助用户快速判断数字产品类型、可能价值路径，以及后续若要做可靠价值评估需要准备哪些数据。

It is designed to prevent one common failure mode in digital product conversations: jumping from "the product exists" or "people use it" directly to "the product has value." The skill helps users slow down, identify the right value logic, and understand what evidence is still needed.

它解决的不是“帮你直接算 ROI”，而是避免数字产品价值讨论里最常见的误区：把“上线了”“有人用”“老板觉得重要”直接等同于“产生了可证明价值”。

## Typical 3-Minute Flow

A typical run should feel like a lightweight guided wizard, not a consulting interview.

1. Choose the main user or audience of the product.
2. Choose what the product mainly helps users do.
3. Answer 1-2 narrowed branch questions based on the previous choices.
4. Select which data is already available, unknown, or not applicable.
5. Receive a `Valence Product Value Lens Result` with likely value paths, recommended metrics, data maturity, and next steps.

The runtime should ask one adaptive multiple-choice question at a time. It should not show a long open-ended questionnaire or require sensitive internal documents.

## Who It Is For

- Product owners who need a first value logic view for one digital product.
- Digital, D&T, data, AI, and platform teams preparing for value conversations.
- Business owners who want to understand which metrics are needed before discussing ROI.
- Teams that need a lightweight pre-diagnostic before a formal Valence review.

## Who It Is Not For

- Teams needing a formal ROI, investment, shutdown, or prioritization decision.
- Portfolio governance owners needing a full scoring model or leadership review pack.
- Users expecting the full Valence Product Value Governance System.
- Requests requiring sensitive internal data, customer names, contracts, screenshots, or confidential finance details.

## How To Invoke

Ask the runtime to use `$valence-product-value-lens` or say:

> 帮我用 Valence Product Value Lens 判断这个数字产品的价值口径和数据准备度。

The skill will guide the user through short multiple-choice questions. It is adaptive: each answer narrows the next question and option set. It accepts anonymous descriptions, approximate numbers, ranges, and Not sure answers.

## Install

### Codex

Copy this repository folder into your local Codex skills directory:

```text
~/.codex/skills/valence-product-value-lens/
```

Then invoke:

```text
$valence-product-value-lens
```

### Claude Code / Open Claw / Hermes

Load `SKILL.md` as the main instruction and follow the linked Markdown references in this repository. For portable instructions, see [runtime_compatibility.md](runtime_compatibility.md).

## Public Boundary

`Valence` and `Valence Product Value Lens` are project names of the author. The MIT license covers this Markdown skill, examples, and supporting text in this repository. It does not publish or grant rights to the full Valence Product Value Governance System, portfolio governance model, internal operating rhythm, or proprietary client materials.

See [NOTICE.md](NOTICE.md) for the public boundary and license scope.

## Runtime Compatibility

This is a pure Markdown skill and can be used by Codex, Claude Code, Open Claw, and Hermes. See [runtime_compatibility.md](runtime_compatibility.md).

- Codex: install as a local skill folder and invoke `$valence-product-value-lens`.
- Claude Code: load the skill folder or `SKILL.md`, then follow linked Markdown references.
- Open Claw: load `SKILL.md` as the main instruction and preserve the adaptive wizard.
- Hermes: use as an evaluation or guided assistant skill; preserve the no-sensitive-data and no-governance-conclusion guardrails.

## Example Input

```text
我有一个销售拜访和门店执行工具，主要给一线销售使用，已经上线但价值不清楚。请帮我判断价值口径。
```

The skill should respond with option-based intake rather than a long open-ended questionnaire. After each user answer, it should show the next narrowed option set rather than the same generic full list.

## Example Output

```markdown
# Valence Product Value Lens Result

## 1. Product Type
Sales execution / field-force productivity product.

## 2. Primary Users / Audience
一线销售 / 商务团队。

## 3. Core Use Case
帮助销售记录拜访、执行门店任务、减少手工跟进，并可能改善销售覆盖质量。

## 4. Likely Value Path
- User-Business Value -> Productivity Gain
- User-Business Value -> Revenue Growth
- User-Business Value -> Decision Quality / Management Visibility

## 5. Suggested Value Logic
Start with productivity and management visibility. Treat revenue as a hypothesis until conversion, order lift, or execution improvement can be credibly attributed.

## 6. Recommended Metrics to Collect

| Metric | Why It Matters | Suggested Owner | User Has It? |
| --- | --- | --- | --- |
| Active users | Confirms adoption and coverage | Product owner | Yes |
| Usage frequency | Measures usage depth | Sales operations | Yes |
| Visit completion / execution rate | Tests whether field execution improved | Sales operations | Not selected |
| Conversion, order lift, or sales proxy | Tests revenue hypothesis | Sales owner / finance | Not selected |
| Annual run cost | Needed before any investment efficiency discussion | D&T / finance | Not selected |
| Business owner confirmation | Prevents over-attribution | Business owner | Not sure |

## 7. Data Maturity Level
Level 1: Value Logic Draft Ready. Usage data exists, but baseline, cost, and business value evidence are not yet sufficient for reliable value estimation.

## 8. What Not To Do
- Do not count all sales growth as product value.
- Do not treat visit records as revenue evidence by themselves.
- Do not call productivity a direct saving without budget or finance evidence.

## 9. Recommended Next Step
Collect active usage, usage frequency, annual run cost, and one business outcome proxy. Ask the business owner to confirm which value path should be used first.

## 10. CTA
如果你有多个数字产品需要统一价值口径、adoption、cost 和 value evidence，可以进入正式 Product Value Diagnostic / Valence review。这个 Skill 只帮助完成单产品的价值口径和数据准备度自查，不替代正式治理评估。
```

## Relationship With Valence

This skill is a front-door helper for Valence. It helps users discover value framing and data readiness gaps for a single digital product.

It does not include formal portfolio-level governance, leadership review, action tracking, sponsor alignment, quarterly operating rhythm, or the full Valence methodology.

If multiple products need consistent value logic, adoption, cost, and value evidence, the next step is a formal Product Value Diagnostic / Valence review.

## File Guide

- [SKILL.md](SKILL.md): agent-facing usage instructions.
- [runtime_compatibility.md](runtime_compatibility.md): compatibility instructions for Codex, Claude Code, Open Claw, and Hermes.
- [conversation_flow.md](conversation_flow.md): guided wizard questions and clarification rules.
- [value_taxonomy.md](value_taxonomy.md): value taxonomy, classification heuristics, and Haleon mapping.
- [data_checklists.md](data_checklists.md): data requirements, owners, and pitfalls by value path.
- [output_templates.md](output_templates.md): reusable final-answer templates.
- [examples.md](examples.md): seven complete option-based examples.
- [NOTICE.md](NOTICE.md): public boundary and license scope.
