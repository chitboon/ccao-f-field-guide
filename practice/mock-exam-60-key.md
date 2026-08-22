# CCAO-F MOCK EXAM — ANSWER KEY & DOMAIN MAP
**Do not open until your 120-minute timer has stopped.**

---

## Quick answer line

```
 1. C    2. A    3. D    4. B    5. C    6. D    7. A    8. C    9. B,D  10. B
11. B   12. A   13. C   14. B   15. A,D 16. D   17. A   18. C   19. B   20. D
21. A   22. C   23. B   24. A,C 25. D   26. A   27. C   28. B   29. B   30. A
31. C   32. B   33. B,E 34. D   35. A   36. A   37. B   38. A   39. A   40. C
41. B   42. A,D,E 43. D  44. A   45. C   46. B   47. D   48. A   49. C   50. B
51. D   52. C,E 53. A   54. C   55. B   56. D   57. A   58. C   59. B   60. B,D
```

---

## How this paper was validated

This mock went through three adversarial review passes. Each found real defects, and what they found is worth knowing, because two of the defects are the kind you should watch for in *any* practice material you use:

| Cue | First draft | Now | Chance |
|---|---|---|---|
| Correct answer is the longest option | 94% (2.62× length ratio) | 25% (1.00× ratio) | 25% |
| Correct answer is 2nd-longest | 66% | 30% | 25% |
| Correct option contains a dash, colon, or semicolon | 89% of such items | 0% (removed from all 248 options) | — |
| Option that justifies itself with "since/because" is wrong | 95% precision | 28% correct vs 25% distractor | — |

The first draft could be beaten by a knowledge-free reader scoring roughly 39/60 on punctuation and length alone. That is now closed. **Also corrected:** one mis-keyed item, and **twelve items that were near-clones of questions in the author's own earlier drill sets** — already answered correctly once, so they measured recall of a key rather than knowledge. They were replaced with scenarios that appear nowhere else.

Position distribution: A 15 · B 15 · C 13 · D 10. Longest same-letter run: 2. Positions were also re-lettered *within item families* — four items sharing a taxonomy template were all keyed D in an earlier draft, which was 4 free marks to anyone who noticed.

If you catch yourself reasoning from position, length, or a keyword, that is a signal you have run out of knowledge on that item. Reason from the stem.

---

## Blueprint coverage

| Domain | Weight | Items | Count |
|---|---|---|---|
| D1 Prompting and Task Execution | 14% | 1, 12, 19, 26, 33, 40, 49, 56 | 8 |
| D2 Output Evaluation and Validation | 21% | 2, 6, 9, 13, 16, 21, 25, 29, 34, 37, 42, 46, 50 | 13 |
| D3 Product and Model Selection | 12% | 5, 14, 23, 31, 39, 48, 57 | 7 |
| D4 Workflow Integration and Solution Design | 16% | 4, 10, 15, 22, 28, 35, 41, 47, 52, 59 | 10 |
| D5 Configuration and Knowledge Management | 12% | 7, 18, 27, 36, 45, 53, 60 | 7 |
| D6 Governance, Risk, and Responsible Use | 15% | 3, 11, 17, 24, 32, 38, 44, 51, 58 | 9 |
| D7 Troubleshooting and Optimization | 10% | 8, 20, 30, 43, 54, 55 | 6 |
| **Total** | **100%** | | **60** |

Multi-response: **9, 15, 24, 33, 42, 52, 60**. #42 is Select THREE; the rest are Select TWO.

---

## Scoring

Multi-response items are **all-or-nothing**: wrong unless every required option is selected and no extra ones are.

| Raw | Read |
|---|---|
| 54–60 (90%+) | Comfortably clear. Sit as booked. |
| 48–53 (80–88%) | Solid margin. Review the misses; no need to move the date. |
| 43–47 (72–78%) | Passing but thin. Work the misses hard in the days you have left. |
| 38–42 (63–70%) | Below the line. Consider using the free reschedule window. |
| < 38 | Move the sitting and take the extra week. |

Pearson VUE's free reschedule normally runs until 24 hours before, so if you are going to move the date, that deadline is the one to work backwards from.

The real exam scales 100–1000 with a 720 cut, which does not map linearly onto percent-correct. Treat 72% here as approximately the boundary, not precisely it.

---

## Rationale by item

**1. C** — D1, *matching the prompting approach to the kind of task*. Research tasks need scope, sourcing, and explicit treatment of uncertainty. A and D ask for research but specify nothing about evidence or structure. B is a *drafting* prompt wearing research clothes, and "confident, authoritative register" actively works against flagging thin evidence.

**2. A** — D2, *checking output for both accuracy and completeness*. The conclusion is defensible; omitting a material conflict is the defect. Nothing was fabricated, so B is wrong. C mistakes "the appendix governs" for "the reader needed no warning" — the paralegal needs to know the contract contradicts itself. D invents a mechanism.

**3. D** — D6, *data sensitivity, regulation and privacy*. The controlling instrument is the data-sharing agreement, and the answer is to read it and get approval. **The trap is that there is no personal data**, which makes A and C feel safe — but the restriction here is contractual, not privacy-based. Sensitivity is not only about PII. B offers deletion afterwards, which does not cure a disclosure that has already happened.

**4. B** — D4, *explaining both the value and the limits*. Names both the gain and the retained control. A oversells. C under-uses. D asserts the human validation step disappears, which is precisely what the stem is testing; connecting a data source is also a governance decision rather than the Associate's to make unilaterally.

**5. C** — D3, *choosing the right product feature for the job*. One specific published figure is a single factual lookup, which is web search's documented profile. A is Research, which is built for multi-source synthesis over several tool calls and is disproportionate here. B reasons about a fact instead of retrieving it. D builds durable infrastructure for a one-off need. **Know the three-way split cold** — see also items 39 and 31.

**6. D** — D2, *judging when a human check or further verification is needed*. Accurate but unfit: the defect is authority, not fact. This tests whether you equate "accurate" with "sendable." A misapplies "hallucination" to a commitment rather than a false claim about the world. B and C reach for mechanisms the scenario does not support.

**7. A** — D5, *keeping configurations and instructions current*. Uncontrolled editing by three people is a governance-of-configuration problem, and the fix is ownership plus an agreed change process. B abandons the shared configuration. C fragments one Project into nine and guarantees divergence. D freezes the instructions, which stops the drift but also stops legitimate maintenance, and no such edit-lock exists in the product — so it fails twice over.

**8. C** — D7, *diagnosing and fixing a prompt that is underperforming*. Replace a vague directive with a measurable constraint. A is the "try harder" distractor. B treats a specification problem as a capability problem — **contrast item 43, where the capability diagnosis is the correct one.** D accepts permanent manual rework.

**9. B,D** — D2, *organising and curating information, and picking the right output format*. Substantial and iterated (B); referenced and reused outside the conversation (D). A argues against an artifact. C is a data-handling consideration, not a format criterion — sensitivity does not determine whether something should be an artifact. E is unrelated to format.
> *Multi-response discipline:* one option alone scores zero.

**10. B** — D4, *using Claude to work through requirements and candidate use cases*. Segment the eleven steps by suitability before recommending anything. A skips the analysis. C optimises for goodwill over value. D escalates work that is explicitly Associate scope — process mapping appears in the guide's intended-audience description.

**11. B** — D6, *telling suitable use cases from unsuitable ones*, plus the escalation theme. Regulatory filings on a matter under active investigation must be owned by legal and compliance from the start, not drafted and then reviewed. **A is the trap** and it is a good one: routing a draft through legal sounds responsible, but it inverts who owns the document, and the drafting choices made first will shape the filing. C applies a verification step to work that should not have started here. D assumes public information cannot create exposure, which is wrong in an investigation context.

**12. A** — D1, *breaking a task into parts*. Sequenced sub-tasks with defined handoffs. B requests the finished artefact in one step. C is repetition, not decomposition. D confuses a longer preamble with decomposition — a common conflation worth naming.

**13. C** — D2, *fact-checking and validation*. Get the derivation, then verify the inputs. A is self-reported confidence, which the official guide's own rationale calls out as unreliable. B removes the appearance of precision while leaving the number unverified. D averages several unverified figures, which is false rigour.

**14. B** — D3, *matching the model tier to what the task needs on cost, speed and quality*. Mixed workloads are best served by routing, not by one tier for everything. A and C each optimise one axis and lose the other. D takes the middle tier as a default, which is the reasoning failure even where the tier might be defensible. **This is one of two items where a tier decision is the right answer** — see 43.

**15. A,D** — D4, *bringing Claude into an existing workflow*, plus the escalation theme. Process mapping and Project configuration are Associate work. B, C and E are Architect/Developer scope: API integration, fine-tuning, and production error-handling architecture. Sections 1 and 3 of the guide both state that Associates escalate these.

**16. D** — D2, *spotting fabrication, inconsistency and bias*. A systematic skew the submitted material did not support is bias. C misapplies "hallucination" — the assessments were factually accurate, and what was imported was the *weighting*, not a false fact. A misreads a consistent pattern as inconsistency, which is close to its opposite. B reaches for a mechanism the scenario does not establish. Distinguishing bias from hallucination is a recurring D2 item type, and the giveaway is whether anything asserted is actually false.

**17. A** — D6, *working inside your organisation's AI policy and governance*. Good outcomes do not retroactively authorise a skipped control. B and C reason from outcome and from perceived stakes. D makes the violation contingent on harm, which is the same error stated more precisely.

**18. C** — D5, *standing a Project up with its instructions and its knowledge*. Project configuration is a property of the Project, not of the user, so it applies to everyone working inside it. A, B and D each add per-user work that the Project already does — and B in particular would recreate the divergence problem from item 7. The discriminator is **scope**: what is configured where, and for whom.

**19. B** — D1, *matching the prompting approach to the kind of task*. Brainstorming wants divergent volume with filtering explicitly deferred. A and D are evaluative and convergent. C is retrospective analysis.

**20. D** — D7, *diagnosing and resolving problems*. Two instruction layers are in direct conflict, and the resolution is to reconcile them rather than re-prompt around the symptom. A blames the tier. B invents a precedence rule that is not documented. C misattributes it to conversation length. **The right diagnosis here is structural** — this is your historical miss pattern's territory.

**21. A** — D2, *fact-checking and validation*. Isolate the unverifiable claim. B generalises from a partial match, which is exactly backwards. C discards verified work. D asks the source of a claim to adjudicate its own claim, the same circularity as 13's option A.

**22. C** — D4, *bringing Claude into an existing workflow, to strengthen it or to redesign it*. States the distinction with its trade-off, which is what the stakeholder needs. A is unqualified advocacy. B wrongly puts redesign outside Associate scope when process redesign is named in the intended audience. D dissolves a distinction the department head has correctly drawn.

**23. B** — D3, *working within context limits, and knowing when to restart, summarise or persist*. The useful content is a small fraction of the conversation, so carry it forward and drop the rest. A instructs the model to ignore context that remains present. C accepts ongoing correction as a working method. D summarises the abandoned exploration along with everything else, preserving the problem. **The discriminator is what is worth carrying, not merely that the conversation is long.**

**24. A,C** — D6, *telling suitable use cases from unsuitable ones* and *data sensitivity*. Sole-basis consequential decisions about individuals (A), and unprotected regulated data (C). B describes a well-controlled use. D is benign. E is a verification concern, not the governance risk asked about.

**25. D** — D2, *editing and adapting output for the audience it is meant for*. Same facts, re-framed by what each audience must decide. B is mechanical deletion, which strips the board version of the reasoning it needs to act. A ignores the requirement. C defers a judgement the analyst should be making.

**26. A** — D1, *iterating on a prompt to get better output*. Targeted correction that preserves what worked. B discards 80% that was right. C substitutes comparison for direction. D delegates the diagnosis to the model rather than supplying it — weaker than naming the defect, though not the same error as asking for a confidence rating.

**27. C** — D5, *keeping configurations, knowledge sources and instructions current*. The requirement is account-wide across all her work, so it belongs at account level rather than being repeated per Project. A works but scales badly and drifts, as item 7 shows. B must be redone every conversation. D confuses instructions with knowledge. **The D5 discriminator is scope: account-wide, Project-wide, or single-conversation.**

**28. B** — D4, *using Claude for research, planning and process improvement*. "The team reports it feels faster" is not a measurement. Check against the measures set at the outset, error rates included, because a workflow can save time while degrading quality. A closes the loop without verifying it. C scales an unverified result. D measures satisfaction, which is real but not the same as effectiveness.

**29. B** — D2, *checking output for both accuracy and completeness*. Silent omission, with nothing in the output signalling it. This is the completeness half of the objective, which candidates under-weight relative to accuracy. A treats accuracy as sufficient. D stretches "hallucination" to cover an omission, and C stretches "bias".

**30. A** — D7, *making a workflow more efficient and more effective*, plus D1 decomposition. Section-then-synthesise. B is emphasis rather than structure. C conflates length with depth. D compounds the problem and adds a merge step.

**31. C** — D3, *choosing the right product feature for the job*. Computing over a data file and generating a chart requires code execution. A retrieves rather than computes. B reasons without executing. D stores the file without computing over it. *Note: the D3 objective names the product features individually — Projects, Research mode, chat, artifacts — so an argument exists for filing this and item 48 under D2's output-format objective instead. The distinction being tested is the same either way.*

**32. B** — D6, *working inside your organisation's AI policy and governance*. Work material on a personal account sits outside the organisation's approved controls, retention, and audit, regardless of who pays. A treats payment as the relevant question. C offers deletion, which does not restore the controls that were bypassed. D invents an internal/external line the policy does not draw.

**33. B,E** — D1, *writing prompts that work, for business and technical tasks alike*. Audience-and-decision framing (B) and explicit success criteria or a worked exemplar (E). A is self-assessed confidence, which the official rationale rejects. C is actively harmful, since length is not specificity. D is folklore.

**34. D** — D2, *spotting fabrication, inconsistency and bias*. Fabricated citations with plausible metadata are the canonical case, and the second clause is the real point: one fabrication raises your prior on the others, so the document needs re-checking. C is the trap — treating a hallucination as locally contained. A invents a retrieval mechanism.

**35. A** — D4, *using Claude for research, planning and process improvement*. Claude structures the comparison and generates the questions; the team owns the facts and the verification. B has Claude both research and recommend, leaving the team ratifying work it has not checked. C hides a judgement inside a weighting scheme. D writes the conclusion before gathering the evidence.

**36. A** — D5, *looking after uploaded knowledge and connected sources*. Sync from live sources, plus a defined cycle for removing superseded files. C is unnecessary churn. B invents a recency rule that the product does not implement. D creates ambiguity about which version is authoritative.

**37. B** — D2, *spotting inconsistency* plus validation. Generation variance is expected, and the response is to verify where the decision turns on it. A treats recency as authority. C treats normal behaviour as a fault to report. D reaches for configuration differences that the scenario does not establish.

**38. A** — D6, *the ethical implications of using AI*. Direct client questions get truthful answers, with the human review explained. B is a misrepresentation. C hides behind proprietary methodology. D makes honesty contingent on a contractual trigger, which inverts the ethical question — the client asked.

**39. A** — D3, *choosing the right product feature for the job*. Complex reasoning with no external retrieval need. B and C both retrieve when nothing needs retrieving. D applies execution to a problem that is not computational. Together with items 5 and 31 this is the feature-selection family; the documented split is web search for straightforward lookup, extended thinking for reasoning without retrieval, Research for multi-source synthesis, and code execution for computing over data.

**40. C** — D1, *writing prompts that work*. Exemplars are the reliable mechanism for voice consistency. A guarantees drift across twenty conversations. B describes a voice rather than demonstrating it. D bolts consistency on afterwards instead of specifying it up front.

**41. B** — D4, *augmenting an existing workflow versus redesigning it*, plus limitations. Improve what reaches each approver, and recognise the number of approvals as a governance decision the Associate is not positioned to change. A and C both quietly assume authority the Associate does not have. D refuses a legitimate improvement.

**42. A,D,E** — D2, spanning *accuracy*, *audience adaptation*, and *when a human check is required*. B is capability, not fitness. C is wrong on its face, since a summary should not stand in place of the policy. F is self-assessment, which the official rationale explicitly rejects.
> *Multi-response discipline:* this is the Select THREE. Stopping at two scores zero. When an item asks for three, keep working until you have three defensible options.

**43. D** — D7, *changing tack in response to what the results show*. Three refinement rounds failing specifically on the harder cases is evidence that the binding constraint is capability, not specification. **This is the item where "use a more capable model" is correct**, and it is here deliberately: that heuristic is *nearly* always wrong, which is exactly what makes it dangerous. A keeps refining past the point of diminishing return. B abandons a workflow that works for 85% of cases. C escalates before making the cheap diagnosis. Learn the discriminator against item 8: tier is the answer when the evidence points to a capability ceiling, not when the prompt, the configuration, or a missing control is the real problem.

**44. A** — D6, *the ethical dimension*, plus escalation. Covert staff monitoring is an ethics-and-legal problem that anonymisation does not cure, so decline and escalate rather than find a technical workaround. B and D both offer anonymisation as the fix, addressing privacy while leaving the covertness untouched. C treats ownership of the platform as settling the question. Two things are tested at once: recognising an inappropriate use, and knowing that escalation beats a workaround.

**45. C** — D5, *looking after uploaded knowledge and connected sources*. Reference material and source documents. A describes instructions. B describes personalisation. D describes automatic carry-over, which is not what a knowledge source is. *Note the distinction: deliberately uploading a decision record as a knowledge document is sound practice, and item 60 keys exactly that for durable definitions. What D describes is a log maintained for you without any upload, which is not what a knowledge source is.*

**46. B** — D2, *choosing between an artifact, inline text and structured data*. Repetitive records with consistent fields, destined for another system. A, C and D all impose prose or conversation structure on data that needs neither. This is the "structured data" leg of the objective, which candidates notice less than artifacts.

**47. D** — D4, *using Claude through solution design, build and iteration*. Claude widens the option space and stress-tests; the accountable people decide and own. A abdicates ownership. B under-uses. C exceeds scope.

**48. A** — D3, *choosing the right product feature for the job*. Producing a real .xlsx the colleague will pivot requires file creation via code execution. B and C produce in-browser content, not a spreadsheet file. D produces something copyable but not a file. **The artifact-versus-generated-file distinction is a high-yield trap** — see items 9 and 46 for the other legs of the format family.

**49. C** — D1, *iterating on a prompt to get better output*. Two rounds of "warmer" failed because "warmer" names a feeling rather than a defect. Naming the actual fault, that the draft explains instead of acknowledging, and showing one line of the target phrasing gives Claude something to act on. A repeats the failed directive with more emphasis. D substitutes a persona for a specification, which is item 1's distractor in another costume. B works but does by hand the part you are trying to delegate, and leaves the next draft with the same problem.

**50. B** — D2, *checking generated output for accuracy*. Supplying context does not guarantee adherence to it, so grounding must be verified rather than assumed. A overstates from a single conflict. C misattributes it to bias. D reaches for the tier.

**51. D** — D6, *working inside your organisation's AI policy and governance*. Work inside the policy and make the case for change through the governance channel, with the controls that would be required. **Note carefully why B is wrong**, because it is the hardest distractor in the paper: redaction is the right answer in most scenarios of this shape, including the sample item in the official guide, so the pattern is well-trained, and item 24 keys the *absence* of de-identification as the risk. Here the policy names *customer contracts* as a prohibited document class, and a redacted customer contract is still a customer contract — the control attaches to the document, not to the identifiers inside it. A routes around the control. C seeks the wrong authority, since a line manager cannot waive an organisational data policy.

**52. C,E** — D4, *explaining to stakeholders what Claude is worth and where it stops*. Handover documentation must convey where human review sits and what each review catches (C), and the known limitations and no-go conditions (E). A and D are development detail. B is a transcript, not documentation. Note the recurring pattern: **limitations are part of the deliverable**, as in items 4 and 59.

**53. A** — D5, *writing standing instructions that hold up*. Concise and durable, applying across every conversation in the Project. B sounds thorough but long instruction sets crowd out the material that matters. C confuses instructions with knowledge. D is an FAQ.

**54. C** — D7, *making a workflow more efficient and more effective*. The waste is a duplicated manual step, and the fix removes both passes by making the output conform on arrival. A removes one pass but leaves the other doing avoidable work. B addresses volume rather than the duplication. D reorganises who does the redundant work instead of eliminating it.

**55. B** — D7, *diagnosing and resolving problems*. Investigate what is different about the failing case, then adapt. A repeats a known failure to confirm it. C routes around without diagnosing. D escalates before producing the information that would make escalation useful. **Note the contrast with items 11 and 44, where escalating is right.** Escalation is correct when the matter is outside your scope or authority; it is premature when a cheap diagnosis is still available. Both directions are tested.

**56. D** — D1, *breaking a task into parts*, plus iteration. Establish and verify the findings before committing them to prose, so errors are caught while still cheap. B collapses two steps that need a checkpoint between them. C inverts the dependency. A requests the finished artefact in one step.

**57. A** — D3, *working within context limits and what carries across sessions*. Durable preferences should be deliberately persisted rather than assumed to be remembered. B is wrong on the facts. C invents a complexity limit. D reaches for the tier. *The wording is deliberately hedged — the specific mechanisms here have changed recently, so the exam is likelier to test the principle than the current interface.*

**58. C** — D6, *data sensitivity, regulation and privacy*. Data collected for one purpose being repurposed for another is the purpose-limitation question, and it is the governance issue the scenario turns on. A, B and D are all real practical considerations, which is what makes this item work — they are simply not the *most important* one. **Watch for stems asking which consideration is most important: several options can be true.**

**59. B** — D4, *explaining both the value and the limits*. Concede the real failure mode, then show the specific controls and what each catches. A is false and will not survive one counter-example. C is whataboutism. D misrepresents what a tier change does.

**60. B,D** — D5, *standing a Project up with its instructions and its knowledge*. The template and formatting rules (B) and the standing metric definitions (D) are durable. A, C and E change every cycle. The discriminator across D5 is **durable versus per-instance**, and in items 18 and 27, **what scope the configuration applies at**.

---

## Two honest caveats on your score

**Discount your raw score by 2 to 4 points before reading it against the bands above.** Roughly nine items test the same discrimination as a question in the companion drill sets, even though the scenario and wording differ. That is partly unavoidable — there are only so many ways to test "sync from the live source" — but it means those items partly measure recall rather than reasoning.

**A strong Domain 3 score here does not cover everything Domain 3 can ask.** No item in this paper names a model. Items 14 and 43 deliberately say "tier" throughout, because tier positioning is stable while version numbers move. The live exam may name Haiku, Sonnet and Opus directly. The same applies to **Skills** and **Memory** — both named in the exam guide's study list, neither tested here.

On the length cue specifically: it is closed in characters but only mostly closed in *words*, where the correct answer is top-two about 60% of the time against a 50% baseline. Reading time tracks words more than characters, so treat that as a small residual rather than nothing. The measured ceiling for a knowledge-free reader exploiting every cue in the paper is about 28/60, against a 43 cut — there is no cue-based route to a pass, which is the property that matters.

## Sort your misses before reviewing anything

Three buckets. The distribution matters more than the count.

1. **Didn't know it.** Mostly D3 and D5 — which capability does what, and what belongs where. Fixable by reading; that is what the cram sheet is for.
2. **Knew it, misread the item.** Missed a "Select TWO", missed "FIRST" or "most important", answered the question you expected instead of the one asked. Item 58 is built to catch this. Fixable by pacing discipline, not study — and it is the failure mode that most often sinks well-prepared candidates.
3. **Chose the plausible-but-soft option.** Picked the better prompt over the verification step, the technical fix over the governance step, or a tier change over a structural one. **This is your documented CCA-F miss pattern.** Items 11, 20, 41 and 51 are where it would show.

Log the bucket split in `claude-associate-cert-prep-plan.md`.

## Re-read even if you got them right

**5, 9, 31, 39, 46, 48** — the feature-and-format family, the largest single cluster in the paper. Web search, extended thinking, Research, code execution, artifact, inline, structured data, and generated file are eight distinct answers, and D2 and D3 both draw on them.

**11, 44, 55** — escalation in both directions. Escalate when the matter is outside your scope or authority (11, 44); diagnose first when it is not (55). The guide's Sections 1 and 3 make escalation an explicit Associate competency, so expect at least one live item — and expect the trap to be a plausible do-it-yourself-then-review alternative.

**3, 24, 51, 58** — the data-governance family, and the subtlest cluster here. What triggers a control: personal data (24), a contractual restriction with no personal data at all (3), a prohibited document class that redaction does not cure (51), and use beyond the purpose of collection (58). Redaction is the right answer in some of these and a trap in others. Learn *what the control attaches to*.

**14, 43** — the two items where a tier decision is correct, against thirteen where it is wrong. Be honest about what that means: on this paper "eliminate the option that changes the model" is still right about 90% of the time, and it is probably a good bet on the real exam too. Just know it is a bet, not a rule, and that items 14 and 43 are what it costs you.
