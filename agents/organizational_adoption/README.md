# Assignment 7 Organizational Adoption Agent

Shenghao Ma · MASY1-GC 1800 · Week 9 · v1.0.0 · November 9, 2026

This specialist assesses whether an organization can absorb, govern, and sustain a proposed application. For a read-only packaging RFQ drafting assistant, Harbor Components should hold the pilot. Ridge Components can run a four-week historical pilot within the charter. Both organizations are fictional.

- [Completed Agent Record (Word)](records/Agent_Record.docx)
- [Agent Record (Markdown)](records/agent_record.md)
- [Readiness framework and decision rules](specialist_instructions.md)
- [Test and revision record](records/test_record.md)

## Reproduce from the repository root

Use Python 3 and the instructor's original scripts. Build each prompt, paste it into ChatGPT, save the returned JSON to a new local file, and validate that file. The saved responses provide a reference for comparison. Each run may phrase its findings differently.

```bash
agent=agents/organizational_adoption
python tools/check_frozen_core.py
for case in primary contrast_1 contrast_2; do
  python tools/build_prompt.py --agent "$agent" --case "$agent/cases/$case.json"
done
for response in "$agent"/responses/*.json; do
  python tools/validate_response.py "$response"
done
```

Prompts are written to `work/`. No API key is needed. The specialist uses the frozen input and output contracts. It puts the eight-dimension readiness profile in `organization_specific_finding`, the decision and ordered actions in `recommendation_management_implication`, and unresolved questions in `abstention_or_more_information_needed`.

## Team integration

Capture sponsor and approval status, named operator and stop authority, incident coverage, reviewer training and capacity, workflow checkpoints and fallback, approved input provenance, sandbox permissions, budget duration, and actual feedback evidence. Include source and date for each control. Keep the specialist label scoped to readiness. A PILOT ONLY result means the supplied profile supports the proposed trial. The orchestrator still needs technology fit and other specialist findings, and management retains approval.
