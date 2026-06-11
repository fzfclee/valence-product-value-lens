# Runtime Compatibility

Valence Product Value Lens is a pure Markdown skill. It has no runtime-specific code, no tool dependency, and no hidden application layer. Any compatible AI runtime can use it by loading `SKILL.md` first, then loading the referenced Markdown files as needed.

## Compatibility Contract

Every runtime must preserve these behaviors:

- Use the human-facing name `Valence Product Value Lens`.
- Use the skill id `valence-product-value-lens` when a machine-readable id is needed.
- Ask one adaptive multiple-choice question at a time.
- Narrow each next question based on the previous answer.
- Include Other and Not sure options where appropriate.
- Avoid asking for sensitive company, customer, contract, financial, system, screenshot, or internal-document details.
- Produce value framing, recommended metrics, data maturity, and next steps.
- Do not produce formal ROI, investment, shutdown, portfolio ranking, or full Valence governance conclusions.
- Preserve the closing note into formal Product Value Diagnostic / Valence review without labeling it as a visible conversion heading.
- Include a Directional Value Calculation section when the value path is clear.

## Codex

Recommended installation:

```text
~/.codex/skills/valence-product-value-lens/
```

Invoke with:

```text
$valence-product-value-lens
```

Codex should read `SKILL.md`, then use `conversation_flow.md`, `value_taxonomy.md`, `data_checklists.md`, and `output_templates.md` as needed.

## Claude Code

Recommended use:

1. Place the folder where Claude Code can load local skills, or explicitly reference `SKILL.md`.
2. Ask: `Use $valence-product-value-lens to assess this digital product's value path and data readiness.`
3. If Claude Code does not auto-load linked files, read `conversation_flow.md` before the intake and read `output_templates.md` before producing the result.

Claude Code must not convert this into a software build task. It should run the adaptive Markdown workflow.

## Open Claw

Recommended use:

1. Load `SKILL.md` as the main instruction.
2. Treat relative links as files in the same skill folder.
3. Run the adaptive wizard exactly as written.
4. If Open Claw has no native skill registry, paste or attach `SKILL.md` plus this compatibility file and reference the folder path.

Open Claw should keep the interaction lightweight and option-led. It should not ask for open-ended discovery unless the option set is insufficient.

## Hermes

Recommended use:

Hermes can use this skill in two modes:

- Guided assistant mode: ask the user adaptive intake questions and generate the Product Value Lens result.
- Review mode: evaluate whether another agent's Product Value Lens output followed the skill.

When used in review mode, Hermes should check:

- Did the agent ask adaptive one-question-at-a-time questions?
- Did it avoid sensitive data requests?
- Did it identify likely value paths conservatively?
- Did it generate recommended metrics and data maturity?
- Did it avoid formal ROI, portfolio governance, or investment conclusions?
- Did it include Directional Value Calculation without using a formal aggregate value label?
- Did it include the Product Value Diagnostic / Valence review closing note without labeling it as a visible conversion heading?

Hermes verdict options:

- `PASS`: output follows the skill and has no material issue.
- `REVISE`: output is useful but has missing adaptive flow, weak data readiness, missing directional calculation, overclaiming, or missing closing note.
- `REJECT`: output asks for sensitive data, exposes full Valence governance, gives formal ROI/investment decisions, or ignores the skill structure.

## Portable Invocation Prompt

Use this prompt in any runtime:

```text
Use Valence Product Value Lens (`valence-product-value-lens`) to assess one digital product. Follow the adaptive one-question-at-a-time wizard. Do not ask for sensitive data. Do not calculate formal ROI or make portfolio governance decisions. Produce value path, recommended metrics, directional value calculation, data maturity, next steps, and the formal Product Value Diagnostic / Valence review closing note.
```


