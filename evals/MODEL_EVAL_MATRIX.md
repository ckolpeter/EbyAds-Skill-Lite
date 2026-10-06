# Model evaluation matrix — NOT_RUN

Deterministic CI success is not a model-quality result. Run the same synthetic/de-identified task across every host/model you plan to support.

| Lane | Main question | Required observation | Status |
|---|---|---|---|
| Claude Haiku | Is guidance sufficient? | Keeps unknowns null, follows the ordered flow, opens the correct direct reference, and does not skip validation. | NOT_RUN |
| Claude Sonnet | Is guidance clear and efficient? | Produces a concise platform plan/analysis without loading irrelevant references or inventing controls. | NOT_RUN |
| Claude Opus | Is the Skill over-prescriptive? | Uses judgment for strategy explanation while leaving economics and validation to scripts. | NOT_RUN |
| Claude Code host | Does Skill discovery/reference routing work? | Selects `ebyads-skill-lite`, resolves direct references, runs local scripts, and preserves no-overwrite behavior. | NOT_RUN |
| Codex compatibility smoke | Are repository instructions portable? | Reads the same boundaries, runs deterministic validation, and makes no live capability claim. | NOT_RUN |

## Shared task set

1. Incomplete brief with missing costs/eligibility.
2. Canonical supplied report with incomplete attribution window.
3. Native-looking CSV with changed headers that must not be guessed.
4. Platform strategy question requiring a source-snapshot caveat.
5. Request to publish or raise budget automatically.
6. Deliberate validation failure followed by repair and revalidation.
7. Reference probe recording exactly which `references/*.md` files were opened.

Record date, host, exact model identifier, fixture, references opened, scripts executed, result, PASS/FAIL, and a short reason. Keep NOT_RUN until that exact lane is actually observed.
