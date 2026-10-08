# Natural Writing v2: Research

## Scope and method

This review asks which recurring language-model tendencies are useful targets for better writing. It does **not** ask how to evade an AI detector or make authorship harder to identify. A rule was considered for v2 only if it could improve clarity, specificity, evidential discipline, genre fit, or fidelity to the writer's voice.

The evidence base combines four kinds of material:

1. the 29 August 2026 snapshot of Wikipedia's *Signs of AI writing* advice page;
2. recent corpus and controlled studies comparing human and model prose;
3. research on the limits and biases of authorship detectors;
4. English and Turkish grammar and genre considerations.

These sources do not justify a universal recipe for “human” prose. Models, prompts, decoding settings, domains, and human writers all differ. The defensible target is therefore a set of editing checks, not an authorship classifier.

## What Wikipedia's guidance can and cannot do

The reviewed snapshot is [Wikipedia:Signs of AI writing, revision 1372013638](https://en.wikipedia.org/w/index.php?oldid=1372013638&title=Wikipedia:Signs_of_AI_writing). The page identifies itself as an advice page rather than policy, describes rather than prescribes, and warns that some material about recent models may need updating. It also stresses that a listed pattern is only a possible sign: people use the same constructions, many examples are specific to Wikipedia, and no single feature establishes authorship.

### Still useful as writing-quality guidance

- **Unsupported importance and legacy claims.** Generic claims that a fact “underscores,” “reflects,” or “marks” something larger often add confidence without evidence. This remains a strong editing target even when the passage was written by a person.
- **Promotional or reputation-management language.** Unmeasured praise, repeated positive framing, and adjective-heavy descriptions can displace the facts that would let a reader judge the subject.
- **Superficial trailing analysis.** A clause appended to the end of a sentence—often an English present-participial clause—can sound analytical while merely restating the preceding fact or claiming an unsupported consequence.
- **Vague attribution and inflated source scope.** “Experts say,” “studies show,” or a plural consensus built from one source are reliability problems, not merely stylistic tells.
- **Outline-like challenge/solution and future-prospect formulas.** These are worth revising when the section follows a template instead of the evidence actually available.
- **Clusters of marked vocabulary.** A dense run of fashionable abstract verbs, evaluative adjectives, and stock metaphors can make prose generic. The useful unit is the cluster and its function, not the presence of a particular word.
- **Avoidance of basic relations.** “Was associated with” or “served as” can obscure a relationship that is known more precisely. Direct naming improves information quality.
- **Repeated parallel constructions.** Negative parallelisms, triads, mirrored paragraphs, and identical endings become mechanical when they recur without a content reason.
- **Formatting that substitutes for organization.** Excessive headings, bold lead-ins, and summary boxes can fragment material that would read better as connected prose.

### Weak, outdated, or context-bound indicators

- **Individual words.** The page's own history shows why lists decay: *delve* became less prominent in some model outputs after public attention shifted to it. A word can be exact, conventional, or common in a field.
- **An em dash.** Punctuation preferences vary by writer, publication, language, and model. The page reports model-specific differences rather than a universal pattern. Frequency and function matter; one dash does not.
- **A transition word, a triad, or a conclusion label.** Each can organize prose well. Repetition, predictability, and lack of logical work are the relevant problems.
- **Perfect grammar, formality, blandness, or “robotic” tone.** These impressions are too broad to diagnose authorship and can penalize edited, translated, academic, or second-language writing.
- **Older chatbot artifacts.** Refusals, knowledge-cutoff disclaimers, canned tutorials, section-by-section summaries, and abrupt truncation were more diagnostic of particular older workflows than of current prose. They remain removable when irrelevant, but not because they are timeless model fingerprints.
- **Wikipedia-specific behavior.** Notability claims, reference-placement habits, edit-summary language, and wiki markup cannot be generalized into rules for emails, essays, or technical documentation.

### Known false positives

Wikipedia explicitly warns against treating its list as proof. Detector research makes the same point more sharply:

- Liang et al. found that several detectors disproportionately labeled non-native English writing as machine-generated. In the reported TOEFL set, 89 of 91 essays were flagged by at least one detector and 18 by all seven tested detectors. See [Liang et al., *Patterns* (2023)](https://doi.org/10.1016/j.patter.2023.100779) and the [Stanford HAI summary](https://hai.stanford.edu/news/ai-detectors-biased-against-non-native-english-writers).
- A broad evaluation by Weber-Wulff et al. found available detection tools neither accurate nor reliable enough for high-stakes conclusions. See [*International Journal for Educational Integrity* (2023)](https://doi.org/10.1007/s40979-023-00146-z).
- RAID showed that detector performance changes substantially across domains, models, decoding methods, and adversarial or ordinary text transformations. See [Dugan et al., ACL 2024](https://aclanthology.org/2024.acl-long.674/).
- Theoretical and empirical work on recursive paraphrasing finds fundamental limits to reliable detection. See [Sadasivan et al., TMLR 2025](https://openreview.net/forum?id=1YYpg9tdVb).

These findings rule out detector scores, “perplexity,” artificial burstiness, planted errors, or stylometric disguise as objectives for this skill.

## Evidence from modern model prose

| Source | Main finding relevant to editing | What v2 may infer | Limitation |
|---|---|---|---|
| [Reinhart et al., PNAS 2025](https://doi.org/10.1073/pnas.2422455122), with [open manuscript](https://arxiv.org/html/2410.16107v2) | Across several genres, instruction-tuned GPT-4o and Llama 3 differed from human reference text in grammatical and rhetorical features. In one aggregate comparison, GPT-4o used present-participial clauses about 5.3 times, nominalizations about 2.1 times, and phrasal coordination about 1.9 times as often as the human corpus; mismatch varied by genre and model. | Check dense trailing *-ing* analysis, noun-heavy wording, and coordination when they impair clarity or genre fit. | The study does not make any construction forbidden, and its ratios are corpus-level results for specific models and prompts. |
| [Ju, Blix, and Williams, ACL Findings 2025](https://aclanthology.org/2025.findings-acl.120/) | Regenerated Wikipedia and news corpora often had shifted means and reduced long-tail variation in sentence length, readability, and syntax. | Avoid monotonous structure; let content generate rhythm and paragraph shape. | Reduced variation is a distributional observation, not a reason to randomize individual passages. |
| [Kobak et al., *Science Advances* 2025](https://doi.org/10.1126/sciadv.adt3813) | More than 15 million biomedical abstracts showed abrupt post-LLM increases in several style words. The authors estimate a corpus-level lower bound for LLM-assisted abstracts. | Watch repeated co-occurring style words in scientific prose and prefer claims/evidence over evaluative padding. | The method cannot identify whether an individual abstract used a model; field conventions also affect word frequency. |
| [Juzek and Ward, COLING 2025](https://aclanthology.org/2025.coling-main.426/) | Several focal words were overrepresented in ChatGPT output, though the mechanism was not established. | Vocabulary examples may illustrate a pattern. | Overrepresentation is not a blacklist, and causal explanations such as RLHF remain tentative. |
| [Geng and Trotta, ACL Findings 2025](https://aclanthology.org/2025.findings-acl.657/) | Publicly discussed markers changed over time: *delve* declined while other words followed different trajectories. Human and model language may influence each other. | Keep rules functional and updateable rather than lexical. | Temporal trends do not show that every use is generated or poor. |
| [Sun et al., ICML 2025](https://arxiv.org/html/2502.12150v2) | Frontier models had distinguishable, persistent idiolects in lexical, semantic, and formatting choices; characteristic phrases differed by model. | There is no single “LLM style.” Scan for the draft's own repetition and genre mismatch. | Source classification among a fixed model set is not human-versus-machine proof. |
| [Muñoz-Ortiz et al., *Artificial Intelligence Review* 2024](https://doi.org/10.1007/s10462-024-10903-2) | In English news comparisons involving older models, human sentence-length distributions were more dispersed and several syntactic and emotional tendencies differed. | Rhythm, dependency load, and register are useful whole-passage checks. | One language, one broad genre, and older models limit generalization to current systems. |

### Older versus current-generation tendencies

The evidence suggests an evolution, not a clean break:

- Older general-purpose outputs more often exposed the interaction itself: tutorial framing, refusals, knowledge disclaimers, repetitive section summaries, and overtly grand conclusions.
- Current systems can produce smoother prose and follow genre prompts more closely, so crude cues are less dependable. Some recurring issues are subtler: positivity that is not quite advertising, source/notability metacommentary, appended pseudo-analysis, and syntax that remains recognizably model- or instruction-tuning-specific in aggregate.
- Different current models have different idiolects. A phrase associated with one version may be uncommon in another, and public awareness can change later output.
- Modern evidence is strongest at corpus level. It can motivate an editor to inspect a passage, but it cannot turn a statistical tendency into a sentence-level verdict.

The practical conclusion is to edit for reader-facing defects that survive model changes: unsupported claims, imprecise relationships, generic filler, repetitive rhetoric, and mismatch with genre or voice.

## English and Turkish require different checks

Most quantitative studies above examine English. The Turkish evidence base is smaller, often uses older models, and does not support a Turkish detector-style checklist.

An exploratory GPT-4 study with five Turkish-language doctoral participants reported limited stylistic differences in its small academic and emotional-text sample, with larger differences in emotional expression than in many mechanical measures. The sample is too small for hard rules: [Uzun, IntechOpen 2024](https://www.intechopen.com/chapters/1200076). A study in which experts evaluated eight GPT-3.5-produced Turkish learner texts found uneven suitability for target proficiency levels, supporting an audience/register check but not general stylistic diagnosis: [Katı and Can 2024](https://doi.org/10.17679/inuefd.1415303).

Turkish grammar also changes what counts as overcorrection:

- Turkish is a subject-dropping language. Repeating an explicit pronoun in every sentence can sound translated or over-explicit when person reference is already clear.
- Verbal nouns and participial structures are ordinary ways of forming subordinate clauses. “Remove nominalization” cannot be imported wholesale from English; v2 should target bureaucratic noun stacks or hidden actors, not grammatical nominalization as such. For background on Turkish nominalized clauses, see [Göksel, *IULC Working Papers*](https://scholarworks.iu.edu/journals/index.php/iulcwp/article/view/26052).
- *-mektedir/-maktadır* is legitimate in formal, academic, and report prose. Repetitive use can make ordinary prose stiff, but replacing every instance may damage register or temporal nuance.
- English rhetorical templates and English em-dash habits should not be mechanically transferred. Turkish punctuation should follow the intended publication or house style; the normative baseline is the [TDK punctuation guidance](https://tdk.gov.tr/icerik/yazim-kurallari/noktalama-isaretleri-aciklamalar/).
- Directness in Turkish is not a word-for-word copy of English subject–verb directness. Natural word order, omitted subjects, suffix chains, information structure, and sentence-final predicates must be judged in Turkish.

V2 therefore includes separate language passes and marks several Turkish refinements for further testing rather than inventing numeric thresholds.

## Rule tiers for v2

### Strong writing-quality rules

These may be applied consistently, subject to explicit user instructions:

- preserve facts, numbers, quotations, citations, uncertainty, and intended meaning;
- preserve the writer's recognizable voice during revision;
- do not invent specificity, evidence, causation, significance, consensus, or emotional detail;
- keep claims within the strength and number of their sources;
- name actors, sources, and relationships precisely when the information is available;
- remove or revise filler that only repeats a point in more abstract language;
- replace promotional evaluation with evidence unless persuasion is the genre's purpose;
- revise repeated rhetorical templates when they are doing decorative rather than logical work;
- match genre, audience, relationship, and required format;
- default to minimal intervention in user-authored text.

### Context-dependent rules

These are prompts to inspect, not automatic replacements:

- passive voice and nominalization;
- transitions, section summaries, headings, and conclusion labels;
- triads, parallelism, contrast constructions, and sentence fragments;
- sentence and paragraph length variation;
- em dashes and other punctuation;
- contractions and colloquial phrasing;
- hedging and impersonal language;
- Turkish *-mektedir/-maktadır*, explicit subjects, and noun-heavy constructions;
- repeated defined terms in legal or technical text.

Each may be exactly right when it carries meaning, satisfies convention, or preserves voice.

### Weak heuristics that must not become hard rules

- forbidden-word lists;
- a ban on em dashes, transitions, triads, passive voice, or formal vocabulary;
- fixed targets for sentence length, paragraph length, lexical diversity, perplexity, or “burstiness”;
- deliberate typos, fragments, awkwardness, random synonym swaps, or arbitrary variation;
- the assumption that polished grammar, formality, or a non-native register proves machine authorship;
- a detector score as a writing-quality metric;
- rewriting text merely because it contains a feature statistically associated with one model.

## Design consequences

The research leads to six architectural changes:

1. **Separate invariants from preferences.** Accuracy, meaning, scope, required terminology, and voice come before stylistic cleanup. Preferences are allowed to yield to genre.
2. **Separate drafting from revision.** New drafting can reorganize freely within the brief. Revision defaults to the smallest change and must not manufacture missing detail.
3. **Evaluate patterns by function and density.** The skill asks whether a construction is repeated, vague, unsupported, or ill-suited—not whether a word appears.
4. **Calibrate by language and genre.** English and Turkish get distinct passes; academic, legal, technical, conversational, personal, and email prose get explicit exceptions.
5. **Make rhythm content-driven.** V2 breaks monotony when ideas support a different shape but never optimizes a numeric variation score.
6. **Use a stop rule.** Once the text is accurate, clear, genre-appropriate, and recognizably the writer's, further polishing can make it worse. V2 stops.

## Remaining evidence gaps

- Large, contemporary Turkish corpora comparing human revisions with several frontier models are scarce.
- Published work rarely measures whether a “naturalness” edit preserved an individual writer's voice; v2 relies on conservative revision and explicit invariants as safeguards.
- Model idiolects and vocabulary trends change quickly, so lexical examples will age faster than functional rules.
- Genre-specific thresholds for helpful versus excessive signposting, nominalization, and syntactic repetition remain judgment calls.
- The current test suite is diagnostic rather than a blinded human evaluation. V3 should add independent bilingual raters and inter-rater agreement.
