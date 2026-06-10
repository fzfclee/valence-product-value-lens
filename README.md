# Valence Product Value Lens

Runtime skill id: `valence-product-value-lens`. Human-facing name: `Valence Product Value Lens`.

Valence Product Value Lens is an entry-level value framing and data readiness skill. It helps users identify the right value logic for a single digital product. It does not expose or replace the full Valence Product Value Governance System.

Valence 产品价值透镜是 Valence 的前置轻量入口，用于单个数字产品的价值口径判断和数据准备度自查。它不等同于完整 Valence 产品价值治理系统，也不输出完整 portfolio 治理模型。

## What This Skill Is

Valence Product Value Lens is a guided, option-based skill. It helps users quickly classify a digital product, identify likely value paths, and understand what data would be needed for a more reliable product value assessment.

Valence 产品价值透镜是一个选项式引导 Skill，帮助用户快速判断数字产品类型、可能价值路径，以及后续若要做可靠价值评估需要准备哪些数据。

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

## 7. Data Maturity Level
Level 1: Value Logic Draft Ready
```

## Relationship With Valence

This skill is a front-door helper for Valence. It helps users discover value framing and data readiness gaps for a single digital product.

It does not include formal portfolio-level governance, leadership review, action tracking, sponsor alignment, quarterly operating rhythm, or the full Valence methodology.

If multiple products need consistent value logic, adoption, cost, and value evidence, the next step is a formal Product Value Diagnostic / Valence review.

## File Guide

- [SKILL.md](SKILL.md): agent-facing usage instructions.
- [runtime_compatibility.md](runtime_compatibility.md): compatibility instructions for Codex, Claude Code, Open Claw, and Hermes.
- [conversation_flow.md](conversation_flow.md): guided wizard questions and clarification rules.
- [value_taxonomy.md](value_taxonomy.md): value taxonomy and Haleon mapping.
- [data_checklists.md](data_checklists.md): data requirements, owners, and pitfalls by value path.
- [output_templates.md](output_templates.md): reusable final-answer templates.
- [examples.md](examples.md): seven complete option-based examples.

