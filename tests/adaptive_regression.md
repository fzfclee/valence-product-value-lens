# Valence Product Value Lens - Adaptive Wizard Regression

Test date: 2026-06-11  
Skill under test: `valence-product-value-lens` / Valence Product Value Lens

## Regression Case: User Answers H then H

### Input

Step 1 answer: H. IT / D&T / 数据 / 平台团队

Expected next prompt:

- Acknowledge IT / D&T / 数据 / 平台团队.
- Show the narrowed IT / platform option set, not the full generic Step 2 list.

Step 2 answer: H before the optimization mapped to "支撑平台能力，例如 API、数据平台、中台、统一入口". In the optimized version, the equivalent narrowed answer is:

A. API / 数据平台 / 中台 / 统一入口等共享平台能力

Expected next prompt:

- Switch to Branch P: Platform Enablement.
- Ask about platform reuse or downstream dependency.
- Do not ask the generic "产品现在处于什么阶段？" question yet.

### Expected Assistant Prompt After Step 2

收到，这更像是平台赋能类产品。下一步先判断平台价值来自复用、下游依赖、避免重复建设，还是运营连续性。

这个平台现在主要被谁复用？

A. 多个下游产品 / 应用  
B. 多个业务团队  
C. 主要是一个核心系统依赖  
D. 还在建设中，尚未明显复用  
E. Other / 其他，请填写  
F. Not sure / 不确定

### Pass Judgment

PASS if the next question is platform-specific and does not show the generic full stage/pain-point questionnaire.
