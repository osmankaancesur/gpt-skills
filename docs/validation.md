# Collection audit and staging validation

20 September 2026. Status: first versions staged and checked, then imported into the public repository. Publication does not change the limited scope of the validation below.

## Completed checks

All four folders passed the available skill validator. After the final edits, natural-writing and instruction-audit were validated again. Frontmatter names/descriptions, optional UI metadata, local reference paths and absence of scaffold placeholders were checked. Descriptions in the design document match the staged files. No runtime scripts, assets, model-version dependencies or cross-skill imports were introduced.

| Skill | Entrypoint words | All skill Markdown words | Resources loaded conditionally |
|---|---:|---:|---|
| evidence-integrity | 515 | 1,094 | Audit or synthesis mode |
| source-tutor | 485 | 954 | Explanation and assessment |
| instruction-audit | 609 | 609 | None |
| natural-writing | 666 | 1,356 | English or Turkish; relevant genre |

Counts use whitespace-separated words, including frontmatter. They are context-size approximations, not tokenizer measurements. The original natural-writing file contains 2,179 such words. Its staged entrypoint is 666; language and genre detail is conditional. The original remains byte-for-byte unchanged, with SHA-256 `ae358dce5955f23c8290512139363082474d574857879aafc77d8365f86c0925`.

## Independent behavioral executions

| Case | Observable result | Assessment |
|---|---|---|
| Evidence packet | Preserved valid completer result; distinguished two studies from three sources; retained attrition, uncertainty and incompatible measures; supplied attributed synthesis | Staging invariants met |
| Instruction repair | Returned completed replacement rules; preserved deployment approval and generated-ledger restriction; bounded retries; distinguished static predictions from execution | Staging invariants met |
| English/Turkish and application prose | Kept sound prose unchanged; retained Turkish evidential/contrastive forms, British spelling and quotation; invented no biography | Staging invariants met |
| Standalone source lesson | Completed lesson, three questions and separate key; preserved elastic-range assumption; kept constructed examples inside the source model | Staging invariants met |
| Live source lesson | Explained the source and asked one unsolved diagnostic question; stopped at the required learner-response boundary | Staging invariants met |
| Writing boundary repairs | Preserved the overclaim during style-only work with a separate concern; translated the authorized quotation and attribution | Staging invariants met |
| Instruction no-change case | Found no established instruction defect and produced no manufactured patch | Staging invariants met |

The author inspected actual outputs against the recorded invariants. Executing agents did not receive the rubrics or expected answers. Some cases intentionally resemble documented failure categories; this is not a held-out benchmark. Excerpts and selection outcomes are preserved in [the execution record](../evals/observed-2026-09-20.md).

A separate description-only selection exercise matched 19 of 20 cases. Routine image-prompt creation incorrectly selected natural-writing. Adding that exclusion corrected the failed case in a fresh selection exercise while retaining natural-writing for three neighboring prose tasks. This is not a claim of 20/20 on a complete rerun or a test of the host's actual implicit skill router.

## Final collection audit

| Concern | Finding and treatment |
|---|---|
| Overlapping triggers | Evidence review and traceable synthesis share one owner. Teaching is restricted to designated sources. Prompt creation and software localization are excluded from prose editing. The observed routine-prompt collision was repaired and rechecked. |
| Duplicated instructions | Each independently usable skill retains the small preservation constraints needed for its operation. Full evidence, teaching or instruction-audit workflows are not copied into natural-writing. No mandatory common policy file. |
| Unnecessary context | One-file instruction-audit avoids needless indirection. Other skills load only the relevant mode/language detail. Maintainer documents and evaluation cases are outside runtime loading. |
| Generic advice | No universal critical-review persona, coding checklist, prompt formula, decision scorecard or general explanation skill. Candidate exclusions explicitly identify baseline competence that does not need restating. |
| Language overgeneralization | Universal preservation and style-function rules stay in the core. Turkish preserves evidentiality, address and normal nominal constructions. No passive-voice ban, English punctuation mandate or national-language stereotype. No unreviewed Spanish/German/French stubs. |
| Model-specific assumptions | Runtime instructions do not name a model generation, rely on a tool registry or make comparative capability claims. Astra guidance informed design, not a public runtime dependency. |
| Maintenance value | Four bounded skills, seven references and no runtime scripts/assets. The proposed value is prevention of recurring boundary failures; measured improvement over the base model remains unestablished. |
| Internal instruction conflict | The English example now respects style-only scope; quotation translation has an explicit authorized path; instruction-audit permits no-change findings. Independent boundary cases exercised all three repairs. |

The independent architectural reviewer recommended keeping all four and adding no generic review skill or extra language module. The author agrees, subject to the limits below.

## Remaining limits and release work

No unassisted baseline, repeated-run comparison, actual automatic-routing test, or human language review was performed. Passing these small synthetic cases does not establish general reliability, specialist referee competence, or a causal benefit from the skills. Evidence-integrity is explicitly not a formal proof verifier; source-tutor has no persistent learner memory; natural-writing has only English/Turkish modules; instruction-audit cannot diagnose unseen controlling rules.

The public repository uses the MIT License. Representative comparisons and competent language review are still needed before making strong quality or language-support claims.

The Git bundle remains the original portable staging deliverable. Its contents were subsequently imported into the public repository; publication does not imply skill installation or deployment.
