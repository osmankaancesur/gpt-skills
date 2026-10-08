# Natural Writing v1: Rule-by-rule audit

## Decision labels

- **KEEP** — retain the rule's substance, with at most copyediting or relocation.
- **MODIFY** — retain the goal but narrow, qualify, or operationalize it.
- **REMOVE** — do not carry the rule or its current mechanism into v2.
- **NEEDS TESTING** — plausible but insufficiently specified or evidenced for a firm runtime rule.

Line references point to the uploaded v1 `SKILL.md`. Lists of example phrases are audited as one mechanism rather than as separate rules for every item.

## Purpose, scope, and priorities

| ID | v1 lines | v1 rule | Decision | v2 treatment and reason |
|---|---:|---|---|---|
| P01 | 1–4 | Name the skill `natural-writing` and trigger on specific, direct, natural English/Turkish prose. | **MODIFY** | Keep the name. Make the description more discriminating: substantial drafting/revision where wording, flow, tone, or voice matters; exclude ordinary factual answers, verbatim text, code, and data extraction. The v1 description risks activating on almost any prose response. |
| P02 | 8–12 | Produce context-appropriate English and Turkish prose across many genres. | **KEEP** | This is the correct scope. V2 makes genre calibration operational rather than treating all listed genres alike. |
| P03 | 14 | Do not manipulate detectors or imitate mistakes; reduce generic/formulaic habits while preserving accuracy, meaning, and voice. | **KEEP** | This is a non-negotiable boundary and is consistent with detector research. V2 also prohibits stylometric targets, artificial randomness, and planted errors. |
| P04 | 18–26 | Resolve conflicts by a fixed seven-item order: accuracy, meaning, specificity, clarity, tone, naturalness, elegance. | **MODIFY** | Replace the flat ranking with invariants plus preferences. Accuracy and meaning are true invariants; specificity can conflict with privacy, brevity, source limits, or genre, while tone can be part of meaning. V2 orders explicit requirements, factual/source integrity, intended scope, voice/relationship, clarity, then polish. |
| P05 | 28 | Never trade accuracy or necessary terminology for a more human sound. | **KEEP** | Preserve verbatim in substance and expand it to numbers, citations, quotations, defined terms, and uncertainty. |

## Content, evidence, and source handling

| ID | v1 lines | v1 rule | Decision | v2 treatment and reason |
|---|---:|---|---|---|
| C01 | 32–35 | Prefer concrete information before abstract claims of importance. | **KEEP** | Strong content rule. V2 adds “when the information is available” so an editor never invents specifics. |
| C02 | 36–44 | Avoid stock significance sentences; allow supported analysis. | **MODIFY** | Keep the functional check but remove the long runtime phrase list. Ask whether the sentence adds a supported consequence, mechanism, comparison, or inference. A phrase can be legitimate when the analysis is real. |
| C03 | 46–47 | Avoid promotional language unless the context requires it. | **KEEP** | Strong rule with a genre exception for marketing, recommendation letters, fundraising, and advocacy. Even there, claims must remain supportable. |
| C04 | 48–70 | Use English and Turkish lists of promotional adjectives as warnings. | **REMOVE** | Do not ship a blacklist. The examples age, create false positives, and can prompt mechanical synonym swaps. V2 targets unmeasured praise, adjective density, and praise that replaces evidence. |
| C05 | 71 | If something is impressive, explain specifically why. | **MODIFY** | Explain with available evidence; otherwise omit, qualify, or ask. “Be specific” must never authorize invention. |
| C06 | 73–79 | Do not invent paragraph-ending analysis; remove vague restatement; a fact may end a paragraph. | **KEEP** | Strong rule. V2 broadens it to endings that merely moralize, forecast, or summarize without doing new work. |
| C07 | 81–94 | Avoid vague attribution when the actual source can be named. | **KEEP** | This improves reliability. V2 preserves genuinely appropriate collective attribution when the source set is collective or anonymity is required. |
| C08 | 96–103 | Prefer a named study/author or adequately identified review. | **MODIFY** | Preserve the source-identification principle but do not impose citation style or invent missing metadata. Use the most precise identification supplied by the user or source. |
| C09 | 104 | Do not turn one opinion into consensus. | **KEEP** | Expand to source number, strength, population, time period, causality, and uncertainty. |
| C10 | 282–290 | Do not infer broad significance or opinion from narrow sources; one source is not a literature or consensus. | **KEEP** | Merge with C09 in one source-scope rule to remove duplication. |
| C11 | 292–300 | Use a subject-substitution test to detect generic sentences, then specify or remove. | **MODIFY** | Keep as an optional diagnostic, not a verdict. Definitions, procedural language, courteous emails, and genre conventions may be reusable yet useful. If a sentence is generic, the permitted outcomes are specify from available facts, make it functionally precise, retain if conventional, ask, or remove. |
| C12 | 302–312 | Every sentence should inform, explain, evidence, infer, or establish voice/scene/emotion; otherwise consider removal. | **MODIFY** | Retain a relevance test but avoid an exhaustive taxonomy. Pacing, orientation, politeness, legal scope, and deliberate repetition can also be useful. The v2 question is whether the sentence serves the passage and reader. |

## Rhetoric, syntax, rhythm, punctuation, and format

| ID | v1 lines | v1 rule | Decision | v2 treatment and reason |
|---|---:|---|---|---|
| R01 | 106–119 | Do not automatically use conclusion formulas; use them only when structurally useful. | **MODIFY** | Keep the function test, remove the runtime blacklist. Conclusion labels and signposts are conventional in academic, legal, instructional, and long report prose. Revise only if mechanical, repeated, or logically empty. |
| R02 | 121 | Endings need not be optimistic, inspirational, or symmetrical. | **KEEP** | Strong safeguard, especially for reports and personal essays. An earned hopeful ending remains allowed. |
| R03 | 123–125 | Watch clusters of stereotypical vocabulary; no individual word is forbidden. | **MODIFY** | Make the pattern rule primary: inspect density, repetition, abstraction, and function. Remove “stereotypical LLM vocabulary” as an authorship frame. |
| R04 | 127–156 | Reconsider a fixed English/Turkish list of words and expressions. | **REMOVE** | Research shows model vocabularies and public markers change. V2 has no maintained word list. Examples belong in research notes, not the install-time rules. |
| R05 | 157 | Use a marked word when it is genuinely the best word, not filler. | **KEEP** | Generalize to every lexical choice. Exact technical or idiomatic wording should not be replaced merely because it is common. |
| R06 | 159–181 | Prefer simple English verbs when no nuance is lost. | **MODIFY** | Retain as an economy test, not a preference for short words. “Serves as,” “constitutes,” and “encompasses” can encode function or scope. Change only when the longer form inflates without adding meaning. |
| R07 | 183–191 | Prefer simple Turkish predicates over inflated `işlevini üstlenmektedir` constructions when meanings match. | **MODIFY** | Keep as a directness example, but judge Turkish register and aspect. Do not replace a formally appropriate predicate automatically. |
| R08 | 193–211 | Name known relationships directly rather than using vague association. | **KEEP** | Strong information-quality rule. V2 adds a safeguard: do not make the relation more definite than the evidence permits. |
| R09 | 213–223 | Limit repeated “not X but Y” contrasts; use only for genuine contrast. | **MODIFY** | Check density and logical work. Contrast is often useful in argument and teaching; the problem is decorative repetition, not the construction itself. |
| R10 | 225–235 | Do not force groups of three; use the count the content requires. | **KEEP** | Strong as a content-first rule. V2 explicitly preserves an accurate or rhetorically useful triad. |
| R11 | 237–242 | Let sentence and paragraph length vary naturally rather than forcing uniformity. | **MODIFY** | Replace vague “variation” with content-driven rhythm: sentence shape should follow idea size, emphasis, and genre. No numeric diversity target. Technical consistency may legitimately reduce variation. |
| R12 | 243 | Do not add mistakes, typos, fragments, or randomness to appear human. | **MODIFY** | Keep the prohibition on planted defects and randomness. Allow fragments already present in the writer's voice or appropriate to conversation, advertising, or literary prose; do not introduce them as camouflage. |
| R13 | 245–251 | Em dashes are allowed; do not default to them; consider alternatives. | **MODIFY** | Preserve punctuation by function and house style. Remove any implied frequency threshold. English em dashes, Turkish long dashes, commas, parentheses, and colons have different conventional uses. |
| R14 | 253–264 | Avoid automatic over-formatting; use format only when it improves comprehension. | **KEEP** | Strong layout rule, particularly for prose deliverables. V2 recognizes that technical procedures, reference material, and comparison tasks may benefit from dense structure. |
| R15 | 266 | Prefer ordinary paragraphs when appropriate. | **KEEP** | Preserve as a direct consequence of R14. |
| R16 | 268–280 | Keep assistant preambles and follow-up offers outside the requested artifact. | **KEEP** | Important boundary between deliverable and conversational wrapper. Preserve salutations or service language when the requested genre itself needs them. |

## Turkish-specific rules

| ID | v1 lines | v1 rule | Decision | v2 treatment and reason |
|---|---:|---|---|---|
| T01 | 316–318 | Avoid excessive `-mektedir/-maktadır` when an ordinary tense is more natural. | **MODIFY** | Retain a density/register check. The suffix is legitimate in academic, report, and formal prose and may encode continuing state or an impersonal register. Change only repetitive or needlessly stiff uses. No numeric threshold is justified. |
| T02 | 319 | Avoid repeatedly starting paragraphs with a fixed set of transition phrases. | **MODIFY** | Check repeated signposting and actual logical relations, not the listed words. A necessary contrast or addition marker should remain. |
| T03 | 320 | Prefer direct verbs over noun-heavy bureaucratic constructions. | **MODIFY** | Target stacked action nouns, hidden actors, and inflated support-verb phrases. Do not treat Turkish verbal nouns and nominalized subordinate clauses as inherently bureaucratic. |
| T04 | 321 | Do not translate English rhetorical structures literally when simpler Turkish is natural. | **KEEP** | Strong bilingual rule. V2 adds checks for repeated explicit subjects, calqued contrasts, and imported punctuation while preserving intentional foreignizing style. |
| T05 | 322 | Preserve Turkish sentence rhythm rather than formal-translation rhythm. | **NEEDS TESTING** | The intuition is useful but “Turkish rhythm” is underspecified and risks subjective rewrites. V2 operationalizes only observable issues—pronoun repetition, predicate chains, calqued order, transition density—and marks broader rhythm judgments for bilingual testing. |
| T06 | 323 | Preserve necessary technical terminology and do not oversimplify academic/scientific content. | **KEEP** | Promote to a global invariant and retain in the Turkish pass. |
| T07 | — | Omit repeated explicit subjects when Turkish reference remains clear. | **NEEDS TESTING** | This is a v2 addition motivated by Turkish pro-drop grammar. Apply conservatively because an explicit subject may mark contrast, repair ambiguity, or carry emphasis. |
| T08 | — | Do not import English em-dash habits into Turkish. | **NEEDS TESTING** | Use publication/house style and TDK conventions rather than a categorical ban. More genre-specific Turkish evidence is needed. |

## English-specific rules

| ID | v1 lines | v1 rule | Decision | v2 treatment and reason |
|---|---:|---|---|---|
| E01 | 327–329 | Prefer direct subject–verb constructions. | **MODIFY** | Direct clauses are a clarity option, not a universal target. Passive voice, dummy subjects, and nominal structures can be conventional or necessary when the actor is unknown, irrelevant, or intentionally backgrounded. |
| E02 | 330 | Avoid unnecessary nominalization. | **MODIFY** | Define the defect: a noun form is a problem when it hides an actor, inflates a simple action, or creates a dense noun chain. Keep terminology and concept nouns that stabilize a technical argument. |
| E03 | 331 | Do not add a transition merely because a paragraph begins. | **KEEP** | Strong function-based rule. V2 says transitions must name a real relation or solve an orientation problem. |
| E04 | 332 | Avoid repetitive rhetorical symmetry. | **KEEP** | Preserve at passage level, with explicit exceptions for deliberate parallelism, speeches, legal clauses, and teaching examples. |
| E05 | 333 | Preserve contractions in a conversational register. | **KEEP** | Voice-preserving and genre-sensitive. Do not add contractions to a writer who does not use them. |
| E06 | 334 | Do not make informal writing artificially academic. | **KEEP** | Strong register safeguard; extend symmetrically so formal prose is not made artificially casual. |

## Voice and revision behavior

| ID | v1 lines | v1 rule | Decision | v2 treatment and reason |
|---|---:|---|---|---|
| V01 | 336–338 | Preserve the author's recognizable voice whenever possible. | **KEEP** | Make this an explicit revision invariant, subordinate only to requested transformation, factual repair, safety, and genre requirements. |
| V02 | 340–346 | Do not automatically formalize, academicize, ornament, or hedge the writer. | **KEEP** | Expand to dialect, warmth, confidence, humor, sentence habits, and degree of directness. |
| V03 | 347 | Make the smallest changes needed. | **MODIFY** | Make minimal edit the default revision mode. Permit substantial restructuring only when requested or when local edits cannot satisfy the brief; disclose material restructuring when useful. |
| V04 | 349 | Treat the user's sample as stronger voice evidence than generic style rules. | **KEEP** | Strong evidence hierarchy. Explicit current instructions and required genre still outrank the sample. |
| V05 | 353–355 | Preserve facts and intended meaning first. | **KEEP** | Expand the invariant ledger to names, numbers, quotations, citations, modality, uncertainty, required terms, and legal/technical scope. |
| V06 | 356 | Edit only sections that need improvement. | **KEEP** | Core minimal-edit behavior and the basis for negative tests. |
| V07 | 357 | Remove generic filler. | **MODIFY** | Remove or rewrite only filler that lacks a reader-facing function. Politeness, orientation, cadence, and genre framing may be functional even if not informationally novel. |
| V08 | 358 | Replace vague statements with specific ones when information is available. | **KEEP** | The availability clause is essential. V2 explicitly forbids invented details and offers ask/flag/retain as alternatives. |
| V09 | 359 | Simplify unnecessarily elaborate wording. | **KEEP** | Preserve nuance, technical meaning, and intentional style; “shorter” is not automatically better. |
| V10 | 360 | Break repetitive syntactic patterns. | **MODIFY** | Break only unhelpful repetition. Preserve deliberate anaphora, parallel claims, procedural consistency, and a writer's characteristic cadence. |
| V11 | 361 | Preserve useful irregularity in length and paragraph structure. | **MODIFY** | Replace “irregularity” with “content-led shape.” The rule must not reward randomness or treat symmetry as suspicious by itself. |
| V12 | 362 | Re-read for natural flow. | **MODIFY** | Specify the pass: read for reference clarity, logical joins, register consistency, and aloud-like cadence appropriate to the genre. |
| V13 | 364 | Do not mechanically rewrite every sentence. | **KEEP** | Retain as the stop rule for revision. |

## Final check, exceptions, and triggering

| ID | v1 lines | v1 rule | Decision | v2 treatment and reason |
|---|---:|---|---|---|
| F01 | 366–385 | Run a 14-item silent checklist covering significance, promotion, invented analysis, attribution, lexical clusters, rhetorical patterns, formatting, verbs, specificity, voice, and accuracy; fix only genuine problems. | **MODIFY** | Consolidate duplicated rules into a shorter five-part check: integrity, evidence/relevance, pattern density, language/genre/voice, and minimality. Replace “suspiciously symmetrical” with a neutral repetition check. Long duplicate checklists consume attention without improving decisions. |
| F02 | 387–398 | Use a lighter touch for legal, methods, specifications, required reports/forms, code docs, templates, and quotations. | **MODIFY** | Replace one “light touch” bucket with explicit genre calibration. Some new drafting in these genres needs substantial work, while revision must preserve defined terms, passive methods style, exact parallelism, templates, or verbatim material. Quotations are never silently rewritten. |
| F03 | 400 | Genre requirements override stylistic preferences. | **KEEP** | Add explicit user instructions and house style at the same level, while factual/source integrity remains non-negotiable. |
| F04 | 402–412 | Trigger for natural prose, wording/flow, less generic writing, listed genres, voice preservation, English/Turkish improvement, or the named style. | **MODIFY** | Keep these positive triggers but encode them in front matter. Distinguish substantial prose from short factual responses and machine-facing text. |
| F05 | 414 | Do not invoke merely because every answer uses language; require material relevance to prose quality or authorship style. | **KEEP** | Essential negative trigger. V2 adds examples: ordinary Q&A, calculation, code, extraction, translation requiring strict literalness, and verbatim handling. |

## Net result of the audit

The v1 foundation is sound: it already rejects detector evasion, protects facts and voice, and treats many surface features as tendencies rather than bans. V2 keeps that core while making four corrections:

1. lexical examples no longer function as a quasi-blacklist;
2. minimal revision and the no-invention rule become explicit operating modes;
3. context-dependent constructions—passives, nominalizations, signposts, triads, punctuation, and Turkish formal suffixes—are judged by function and genre;
4. English and Turkish receive separate, grammatically informed passes, with uncertain Turkish rhythm rules marked for continued testing.

