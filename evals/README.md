# Behavioral evaluation

These are synthetic maintainer fixtures, not references to load during normal skill use. They contain no copied research reports or private personal history. The application fixture uses generic science-site notes as invented test input.

`cases/` contains raw user requests and source material. `rubrics.md` contains expected invariants. Keep the rubric and prior outputs away from an executing agent. `routing-cases.json` is a description-selection exercise with positive, negative, composition and ambiguous cases; strip expected answers before giving it to an evaluator.

For a behavioral pass, provide a fresh agent only the skill path, the raw case, and any needed permission/side-effect limits. Ask it to perform the task. Inspect the actual result against the rubric rather than matching headings, exact sentences, or a self-reported pass. The source-only fixtures need no browsing. Evaluation outputs must not modify installed skills or live systems.

Cases:

| File | Requested operation |
|---|---|
| `evidence.txt` | Audit and synthesize a supplied source packet |
| `instructions.txt` | Repair proposed agent instructions |
| `writing.txt` | Preserve Turkish and English voice; draft from sparse notes |
| `lesson.txt` | Complete a source-only worksheet |
| `live-lesson.txt` | Explain, ask a question, and wait for the learner |
| `writing-boundaries.txt` | Preserve an overclaim during style-only editing; translate an authorized quotation |
| `instructions-no-change.txt` | Audit sound instructions without manufacturing a patch |

Observed responses and routing outcomes are retained in `observed-2026-09-20.md`. The four focused routing rechecks are also recorded there with their requests; the original routing corpus retains its original case identifiers.

For a meaningful improvement claim, run the same raw requests in fresh sessions with and without the skill, keeping model, tools and source access comparable. Record actual model/runtime identifiers when available. Use blind assessment where practical and more than one run for variable behavior. The recorded first pass does not isolate the skill's causal effect.

Add regressions for observed failures and counterexamples where no edit, no criticism, or no skill invocation is correct. Add language-specific cases in that language; do not translate an English rubric and call it native review. Keep useful failures rather than turning every unusual example into another universal instruction.
