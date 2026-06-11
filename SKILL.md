---
name: valence-product-value-lens
description: Entry-level Valence Product Value Lens for single-product value framing and data readiness checks. Use in Codex, Claude Code, Open Claw, or Hermes when users need an adaptive option-based wizard to classify a digital product, identify likely value paths, select metrics, assess data maturity, and decide whether to enter a formal Product Value Diagnostic or Valence review without exposing the full Valence governance system.
---

# Valence Product Value Lens

Runtime skill id: `valence-product-value-lens`. Human-facing name: `Valence Product Value Lens`.

Valence Product Value Lens is an entry-level value framing and data readiness skill. It helps users identify the right value logic for a single digital product. It does not expose or replace the full Valence Product Value Governance System.

Valence 产品价值透镜是 Valence 的前置轻量入口，用于单个数字产品的价值口径判断和数据准备度自查。它不等同于完整 Valence 产品价值治理系统，也不输出完整 portfolio 治理模型。

## Purpose

Use this skill to help a user move from a rough description of one digital product to:

1. product type and primary users;
2. likely value path;
3. recommended metrics and data checklist;
4. current data maturity level;
5. next data collection and stakeholder confirmation actions;
6. a light closing note into formal Product Value Diagnostic / Valence review when appropriate.

The core deliverable is: value logic + data readiness checklist + directional value calculation path + data maturity judgment.

## Runtime Compatibility

This is a pure Markdown skill with no app, API, database, frontend, or mandatory tool dependency. It is designed to work in:

- Codex
- Claude Code
- Open Claw
- Hermes

Follow [runtime_compatibility.md](runtime_compatibility.md) when installing, invoking, or adapting the skill outside Codex. All runtimes must preserve the same behavior: adaptive one-question-at-a-time wizard, conservative output, no sensitive data request, and no full Valence governance disclosure.

## Use This Skill For

- Single digital product value framing.
- Early value logic diagnosis before ROI calculation.
- Data readiness self-checks for adoption, cost, business value evidence, risk, or platform reuse.
- Guided intake before a formal product value diagnostic.
- Anonymous or approximate B2B product discussions.

## Do Not Use This Skill For

- Formal ROI decisions.
- Portfolio scoring or product shutdown / promote / protect / hibernate recommendations.
- Full Valence Product Value Governance System design.
- Leadership review packs, action trackers, sponsor alignment playbooks, or quarterly governance operating rhythm.
- Requests that require sensitive company, customer, contract, financial, or system details.

## Input Rules

- Prefer multiple-choice questions over open-ended questions.
- Only ask open-ended questions when options are insufficient.
- Always include Other and Not sure options where appropriate.
- Ask exactly one question at a time unless the user explicitly asks for a batch intake.
- Use adaptive branching: each next question must reflect the user's previous answer.
- Do not show the full generic option bank after the first broad classification if a narrower branch is already clear.
- When a user selects an option, briefly acknowledge what that implies before asking the next question.
- Do not require the user to provide all data before producing a result.
- Allow anonymous descriptions, approximate ranges, and Not sure answers.
- Avoid asking for company names, product real names, customer names, contracts, screenshots, internal documents, or sensitive data.

## Guided Wizard

Follow the full flow in [conversation_flow.md](conversation_flow.md).

Start with this safety frame:

> 不需要提供公司名、产品真名、客户名、合同、截图、内部文档或敏感数据。可以使用匿名描述、模糊数字、区间数字或 Not sure。

Then collect through an adaptive wizard, not a fixed questionnaire:

1. Product Audience
2. Product Function, narrowed by audience
3. Branch-specific product stage or operating context
4. Branch-specific pain point / value driver
5. Branch-specific value direction confirmation
6. Branch-specific data readiness check
7. Optional one-sentence context

After each answer, decide the next best question from the branch rules in [conversation_flow.md](conversation_flow.md). After enough signal exists, ask at most 3 clarifying questions only if needed to resolve classification conflict or value-path uncertainty. If the user does not answer, still produce a result with uncertainty clearly marked.

## Adaptive Behavior Rules

- Treat Step 1 as routing, not as a form field.
- Treat Step 2 as the main branch selector.
- For IT / D&T / data / platform teams selecting platform capability, immediately switch to Platform Enablement questions: downstream products, reuse, duplicate build, run cost, SLA/dependency, owner confirmation.
- For IT / D&T / data / platform teams selecting compliance/risk, switch to Risk Reduction questions.
- For IT / D&T / data / platform teams selecting AI/innovation, switch to Strategic Capability / Learning questions.
- For management audiences selecting dashboards, switch to Decision Quality / Management Visibility questions.
- For sales or customer audiences selecting growth, switch to Revenue Growth questions.
- For functional teams selecting automation/manual replacement, switch to Productivity Gain / Cost Avoidance questions.
- If the user answers Not sure, provide 3-5 diagnostic options and continue.

## Value Taxonomy Summary

Use [value_taxonomy.md](value_taxonomy.md) as the taxonomy source, including its Classification Heuristics and Classification Tie-Breakers.

Level 1 categories:

- User-Business Value
- Time Criticality
- Risk Reduction / Opportunity Enablement

Secondary value paths:

- Revenue Growth
- Cost Saving
- Cost Avoidance
- Productivity Gain
- Experience / Service Quality Improvement
- Decision Quality / Management Visibility
- Deadline-Driven Business Value
- Operational Continuity
- Value Decay
- Compliance / Regulatory Timing
- Risk Reduction
- Opportunity Enablement
- Platform Enablement
- Strategic Capability
- Learning / Validation Value

This skill may borrow Cost of Delay logic from SAFe WSJF, but it must not calculate WSJF scores or perform WSJF ranking.

## Data Maturity Model

- Level 0: Product Story Only. Only product description or rough options exist. Output a value logic draft only.
- Level 1: Value Logic Draft Ready. Product type and value path are reasonably clear, but key data is missing. Generate metrics and a data collection plan.
- Level 2: Rough Estimate Possible. Some adoption, usage, cost, or value proxy data exists. A rough estimate may be possible, but not for formal decision-making.
- Level 3: Evidence Review Ready. Adoption, cost, and business value evidence exist, with relevant owner confirmation. Recommend formal product value diagnostic.
- Level 4: Governance Review Ready. Evidence is complete enough for portfolio-level review or leadership discussion. This skill only recommends formal assessment; it does not output governance conclusions.

Public-skill guardrail: Level 4 should be rare in this public skill. When in doubt, cap the result at Level 3 and recommend a formal Product Value Diagnostic / Valence review. Do not use Level 4 to imply that the skill itself can run governance, rank products, or support investment decisions.

## Output Rules

Use templates from [output_templates.md](output_templates.md).

- If data is insufficient, state: "当前信息足以形成价值口径草案，但不足以进行可靠价值估算。"
- If enough parameters exist, provide only a rough example calculation with assumptions and limitations.
- Always include a Directional Value Calculation section when the likely value path is clear.
- Treat Directional Value Calculation as a public-facing calculation direction, not a formal Valence valuation model.
- Do not use a formal aggregate value label and do not imply all metric signals should be added together.
- Do not invent default attribution ratios, discount factors, industry benchmarks, or conversion assumptions. Mark them as data to confirm unless the user provided them.
- Do not say a product has no value, has high ROI, should stop, should continue, or deserves more investment.
- Prefer conservative language: value hypothesis, evidence weak signal, data readiness gap, further validation, owner confirmation.
- Include 2-4 "What Not To Do" bullets in every final result.
- End with the fixed closing note from the output template, but do not label it as a conversion heading and do not make it a numbered heading.
- When assigning Level 4, explicitly say that the next step is formal assessment outside this public skill.

## Guardrails

- Do not expose full Valence methodology, portfolio governance model, templates, formulas beyond light calculation paths, or operating rhythm.
- Do not expose proprietary Valence scoring, weighting, portfolio governance, or investment-decision logic. Public directional calculation paths are allowed.
- Do not present self-service deflection or productivity gain as direct Cost Saving unless budget, vendor, outsourced service, or finance-confirmed spend reduction exists.
- Do not equate launch, usage, or page views with value.
- Do not treat Productivity Gain as direct Cost Saving unless finance/budget evidence supports it.
- Do not treat Risk Reduction as simple Cost Avoidance.
- Do not assess Platform Enablement with a single-product ROI lens only.
- Do not force Strategic Capability or Learning Value into short-term ROI.
- Do not let Learning Value become an excuse for open-ended pilots; require hypotheses, time limits, and next-stage decision criteria.
- Do not use Level 4 as a substitute for Valence review, leadership review, portfolio review, or governance action.

## References

- [README.md](README.md): human-facing overview and usage.
- [runtime_compatibility.md](runtime_compatibility.md): Codex, Claude Code, Open Claw, and Hermes compatibility contract.
- [conversation_flow.md](conversation_flow.md): option-based wizard.
- [value_taxonomy.md](value_taxonomy.md): value categories, classification heuristics, tie-breakers, and Haleon mapping.
- [data_checklists.md](data_checklists.md): data requirements by value path.
- [output_templates.md](output_templates.md): reusable result templates.
- [examples.md](examples.md): seven complete wizard examples.
- [NOTICE.md](NOTICE.md): public boundary and license scope.


