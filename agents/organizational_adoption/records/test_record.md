# Test and Revision Record

## Design and observed results

The same LLM, application, industry, adoption posture, risk boundary, management question, and time horizon apply throughout. The case differences are organizational. All three profiles are fictional. The test exercises prompt reasoning and the JSON contract. It does not test a procurement model or measure actual savings.

| Case | Version | Saved decision | Interpretation |
| --- | --- | --- | --- |
| [Harbor Components](../cases/primary.json) | 1.0.0 | [HOLD](../responses/primary_response.json) | Missing stop authority, reviewer capacity, exception handling, and traceable identifiers block the pilot. |
| [Ridge Components](../cases/contrast_1.json) | 1.0.0 | [PILOT ONLY](../responses/contrast_1_response.json) | Delegated stop authority, approved data, rehearsed review, and funding support a four-week test. Recurring capacity and outcomes remain open. |
| [Ridge with authority omitted](../cases/contrast_2.json) | 0.1.0 | [Proceed with scoped trial](../responses/contrast_2_v0.1.0_response.json) | Weakness. It detected the missing authority but treated it as a setup item and requested generic governance evidence before rollout. |
| [Ridge with authority omitted](../cases/contrast_2.json) | 1.0.0 | [REQUEST EVIDENCE](../responses/contrast_2_response.json) | The same input now prompts a request for signed stop delegation and incident coverage before launch. |

**Stable finding.** Confabulation risk, source verification, the manual decision boundary, and conditional application fit stay the same across the revised responses.

**Changed finding.** Harbor's gaps require corrective action before a pilot. Ridge's controls support a bounded test. Removing authority evidence from Ridge withholds the pilot decision without treating missing evidence as an established deficiency.

**Revision.** The [initial instructions](specialist_instructions_v0.1.0.md) asked for a bounded recommendation and uncertainty, but gave no decision gate for unknown authority. The revision separates missing critical evidence from known gaps and requires a named decision-maker, signed delegation or equivalent, and an incident route. It also separates pilot capacity from sustained operating capacity.

**Method and limits.** The prompt packets were built with the instructor's script and evaluated in the ChatGPT/Codex session. Saved JSON captures the in-session evaluations. These are single examples per prompt and profile. Separate-session repeatability and real-world pilot performance were outside the test. To reproduce the earlier prompt, use the archived initial instructions as the specialist file in a temporary copy, set metadata version to `0.1.0`, and build with the same `contrast_2.json`.

## Source verification

NIST AI 600-1, *Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile* (July 26, 2024), section 2.2 and actions GV-3.2-003 and GV-3.2-004, identifies confabulation and provides voluntary guidance on acceptable use and feedback. Those passages support the verification and reporting controls. Specific stop-authority gates and proposed pilot criteria are specialist judgments. Organizational facts come from the case files. No vendor, legal, performance, or market adoption claim drives the outcome. [Original NIST report](https://doi.org/10.6028/NIST.AI.600-1)

## Verification results

- Frozen core integrity checker passed. All files listed in the original package manifest also matched.
- The instructor's prompt builder generated a packet for each revised case and the initial failure case.
- All three inputs and four saved responses validated against the frozen JSON Schemas. All four responses also passed the instructor's response validator.
- The revised decision labels matched the expected case outcomes. The general technology and application findings stayed identical in the matched tests. Each revised profile covered all eight dimensions.
