# Contributing

Contributions that make Valence Product Value Lens clearer, more portable, or more evidence-disciplined are welcome.

## Useful Contributions

- Anonymous product scenarios with enough context to test the Lens;
- Compatibility notes for Markdown-based AI agent environments;
- Corrections to value logic, evidence guardrails, or data checklists;
- Regression cases where the adaptive question path selects the wrong branch;
- Improvements to accessibility, plain-language wording, or documentation.

Do not submit confidential company information, personal data, client material, proprietary benchmarks, or content that you do not have permission to share.

## Pull Request Checklist

1. Keep the change focused on the public single-product Lens.
2. Explain the user problem and the expected behavior change.
3. Add or update a scenario case when behavior changes.
4. Run:

   ```text
   python scripts/validate_repo.py
   ```

5. Confirm that internal Markdown links work and files remain UTF-8 without BOM.
6. Preserve attribution, license, and notice files.

By contributing, you agree that your contribution may be distributed under this repository's MIT License.
