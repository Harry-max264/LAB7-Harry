# Organizational Adoption Agent Record

## A. Agent and Version

- **Student / team** — Shenghao Ma (individual submission)
- **Assignment / specialist agent** — Assignment 7 / Organizational Adoption Agent v1.0.0
- **Date** — November 9, 2026
- **GitHub repository** — https://github.com/Harry-max264/LAB7-Harry
- **Branch** — assignment-7
- **Commit** — b0c88ed91c0bb8491f2e219070f6034ad09193e1
- **Frozen scaffold version** — MASY1800_ET_Agent_Scaffold_v1_0

## B. Specialist Purpose and Context

- **Governing analytical question** — Can this organization absorb, govern, and sustain the proposed application?
- **Emerging technology** — Large language model (LLM) generative AI.
- **Intended application** — Draft source-linked packaging RFQ comparison briefs from sanitized historical bid packets. Buyers verify claims and retain manual approvals.
- **Organization / industry** — Harbor Components and Ridge Components, fictional mid-sized U.S. industrial manufacturers. Harbor is the primary case.
- **Adoption posture** — Moderate fast-follower. The organization favors reversible trials.
- **Risk / consequence context** — Wrong prices or terms could distort sourcing decisions. Bid confidentiality, source traceability, and a manual fallback matter.
- **Management question / time horizon** — Decide pilot eligibility this week, assess a four-week pilot if eligible, and revisit rollout within 90 days.

## C. Three-Level Finding

- **ET generally** — Generative AI can produce plausible factual errors. The selected model’s accuracy is unmeasured.
- **ET for this application** — Read-only drafting is plausible if buyers can trace prices and terms, catch omissions, and keep sourcing decisions manual.
- **ET for this application in this organization** — Harbor has director support, a sandbox, and manual sign-off. It lacks accountable stop authority, reviewer capacity, an AI exception path, and complete source traceability.
- **Bounded management implication** — HOLD Harbor’s pilot. First delegate stop and escalation authority. Next fund and rehearse buyer review and fallback. Reconcile packet IDs and revisions before admitting them.
- **Confidence / uncertainty** — High confidence in the hold given explicit gaps. Trial performance, staffing needs, and ongoing culture remain uncertain.
- **What evidence or condition would change the conclusion** — Reconsider after signed delegation, a passed escalation and review rehearsal, protected hours, and verified packet identifiers. Require measured quality and value plus recurring support for rollout.

## D. Evidence and Testing

- **Most important evidence/source(s)** — Case JSON files document the fictional profiles. NIST AI 600-1 (July 26, 2024), section 2.2 and actions GV-3.2-003/004, supports the general risk and oversight analysis. DOI 10.6028/NIST.AI.600-1.
- **Primary test - result** — Harbor: HOLD. Multiple pilot controls are explicitly absent, led by stop and escalation authority.
- **Contrast test - what appropriately stayed stable** — The same use has the same confabulation exposure, source-verification requirement, and conditional fit.
- **Contrast test - what appropriately changed** — Ridge: PILOT ONLY. Delegated authority, verified packet identifiers, rehearsed review, and funded capacity support a four-week historical test.
- **Weakness/failure found** — The initial response spotted missing stop authority but still advised proceeding. Its evidence request was generic and deferred until rollout.
- **Revision made and why** — Added a pre-launch evidence gate. On the same input the revised agent requested a signed delegation clause and incident coverage and withheld launch authorization.
- **Remaining limitation / abstention condition** — If authority is unclear, ask who can pause the pilot and who handles incidents during absences. Fictional cases and one response per prompt cannot establish repeatability or performance.

## E. Independent Judgment and Handoff

- **Is the agent credible enough for team consideration? Why?** — Yes, as bounded readiness advice. The agent distinguishes hold, pilot-only, and missing evidence while keeping technology and use fixed. I would hold Harbor and prioritize delegated stop authority.
- **Most important recommendation to the team** — Capture named owners, delegation and coverage evidence, budget and reviewer time, training rehearsal, approved data, fallback, and feedback mechanisms. Let management own launch approval.
- **AI / verification note** — ChatGPT/Codex helped draft, evaluate, and revise the agent. I checked the original NIST passages and traced organizational claims to the case inputs. The original scaffold checker and JSON validation passed.

The commit above pins the tested agent and its evidence. The following commit adds this completed record.

See the [test and revision record](test_record.md) for the saved responses and checks.
