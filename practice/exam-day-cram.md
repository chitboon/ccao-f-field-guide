# CCAO-F Exam-Day Cram Sheet
**Sat 22 Aug · 60 items · 120 min · 720/1000 to pass**

Read this Friday evening and once more before you log in. Nothing here is new — it is the decision rules, in the order you will need them.

---

## 1. The four rules that decide most items

**Structure beats cleverness.** When torn between improving the prompt and adding a verification, governance, or configuration step, the exam wants the structural mechanism. Verify the citation. De-identify before uploading. Escalate. Fix the Project instead of patching the chat. *This is your documented miss pattern from CCA-F — it is the single highest-value line on this sheet.*

**Accurate is not the same as usable.** An output can be factually correct and still unfit: it exceeds the sender's authority, omits a material conflict, is pitched at the wrong audience, or silently leaves something out. Completeness and fitness are separate criteria from accuracy.

**The model is rarely the answer.** "Use a more capable tier" is wrong perhaps nine times in ten. It is right only when the evidence points to a genuine **capability ceiling** — the task fails specifically on its harder cases and prompt refinement has already been tried. Otherwise the cause is the prompt, the configuration, a missing control, or conflicting instructions.

**Escalate when it is not yours; diagnose when it is.** Escalation is correct for API integration, fine-tuning, production architecture, and anything carrying legal or regulatory liability. It is *premature* when a cheap diagnosis is still available. Unfamiliarity is not a reason to escalate. Both directions are tested.

---

## 2. Multi-response discipline

Six to eight items. **No partial credit.** One right answer out of two scores the same as a wrong one.

- Read the stated count. It varies — TWO, THREE, sometimes more.
- After selecting, **count your letters** and read the count again. Every item, including the ones you feel sure about. Certainty is when the habit lapses.
- If you can defend only one on a Select TWO, do not leave it short. A guess costs nothing; an incomplete answer costs the same as a wrong one.
- When most options look right, elimination stops working. Evaluate each option positively.

---

## 3. Which capability — the feature decision table

| Need | Use |
|---|---|
| One current fact, straightforward lookup | **Web search** (1–2 retrievals) |
| Careful reasoning, no external information needed | **Extended thinking** |
| Multi-source synthesis with citations, a real report | **Research** (5+ retrievals, minutes) |
| Compute over a data file, or produce a real file | **Code execution / file creation** |
| Same instructions and materials across many conversations | **Project** |
| Substantial content that is iterated and reused | **Artifact** |
| A repeatable procedure Claude should follow | **Skill** |
| Durable facts about *you* and how you work | **Memory / personalisation** |

**Research + extended thinking combine** — gather thoroughly, then reason over what was gathered.

### The format family (four distinct answers, easily confused)

- **Inline** — short answers, clarifications, anything under roughly 15 lines.
- **Artifact** — substantial, self-contained, iterated, reused outside the conversation. In-browser content: documents, code, HTML, SVG, diagrams, React.
- **Structured data** — repetitive records with consistent fields, destined for another system.
- **Generated file** — a real .xlsx, .docx, .pptx, PDF or PNG the recipient opens elsewhere. **An artifact is not a downloadable Office file.** If they will pivot it in Excel, you need file creation, not an artifact containing a table.

### Model tiers

The guide names **Haiku, Sonnet, Opus**. Positioning is what matters, not version numbers:

- **Haiku** — fastest, cheapest. High-volume, well-defined, formulaic work. Classification, short routine drafting.
- **Sonnet** — balanced speed and capability. Cost-conscious general work.
- **Opus** — most capable. Complex reasoning, nuanced judgement, agentic work.

Match the tier to the task. For a **mixed** workload, route: cheap tier for the routine majority, capable tier for the flagged minority. Never "always use the best" and never "default to the middle."

---

## 4. Configuration — what goes where

The two discriminators that answer nearly every D5 item:

**Scope.** Account-level personalisation applies to *all* your conversations. Project instructions apply to *every conversation in that Project*. A prompt applies to *one conversation*. If the requirement is "always, everywhere," it is account-level — not repeated in each Project.

**Durable versus per-instance.** Configuration holds what does not change: templates, formatting rules, standing metric definitions, role and tone, reference documents. Each conversation supplies what does: this month's figures, today's question, this cycle's recipient.

| | Goes in |
|---|---|
| Rules about behaviour, tone, format, constraints | **Project instructions** |
| Reference material and source documents | **Knowledge sources** |
| Documents that change at source | **Connector**, synced from the live version |
| Facts about you, your role, your preferences | **Memory / personalisation** |

Other points worth holding:

- Project configuration is a property of the **Project, not the user**. A new team member needs no personal setup to get consistent output.
- Keep instructions **concise**. Long instruction sets crowd out what matters. "Cover every scenario" is the wrong instinct.
- Maintenance is a real objective: **replace** superseded files rather than instructing Claude around them, and prune on a defined cycle.
- Individual chats inside a shared Project stay private unless separately shared.
- Uncontrolled editing of shared instructions is a governance problem. The fix is **ownership plus a change process**.

---

## 5. Evaluation and validation — the heaviest domain at 21%

**Failure taxonomy.** Get this crisp; several items turn on it.

- **Hallucination** — something asserted is false or fabricated. Citations, statistics, section numbers, studies. The tell is a plausible specific that does not exist.
- **Bias** — a systematic skew the source material did not support. Nothing asserted is false; the *weighting or framing* was imported.
- **Incompleteness** — something is missing, and nothing signals it. The most dangerous failure because it is silent.
- **Inconsistency** — different answers to the same question. Expected behaviour, not a fault to report.

**One fabrication implicates the document.** If a citation is invented, re-check the others. Hallucinations are not locally contained.

**Never accept self-assessment.** "Ask Claude how confident it is" and "have Claude check its own accuracy" are wrong answers every time. The official guide says so explicitly.

**Human review is required when** output goes out externally under the organisation's name, informs a decision with legal, financial, or regulatory consequence, affects an individual materially, or reaches someone who cannot evaluate its accuracy. It is *not* required for internal brainstorming or reformatting. **A better model never substitutes for a review control.**

**Audience adaptation: same facts, different framing.** Change what leads and how much technical depth. Do *not* change the substance, omit unwelcome findings, or present tentative conclusions as settled. That is where adaptation becomes misrepresentation.

**Supplied context does not guarantee adherence to it.** If output conflicts with a document you provided, grounding must be verified, not assumed.

---

## 6. Governance — what the control attaches to

The subtlest family on the exam. Redaction is sometimes the answer and sometimes a trap. **Ask what the control attaches to:**

| Trigger | Correct response |
|---|---|
| Personal or regulated identifiers | De-identify before providing (this is the official Sample 3 answer) |
| A **document class** named as prohibited | Redaction does **not** cure it — a redacted customer contract is still a customer contract |
| A contractual restriction, even with no personal data at all | Check the agreement, obtain approval. Sensitivity is not only about PII |
| Use beyond the purpose the data was collected for | Purpose limitation applies, needs review |
| Legal or regulatory liability | Escalate to the owners; do not draft first and route later |

Also hold:

- **Policy is not outcome-dependent.** A skipped review is a violation even when the result was fine. Good outcomes do not retroactively authorise anything.
- **Scope calibrates the depth of review, never whether it applies.** "It's only a pilot" is not an exemption.
- **Work material on a personal account** sits outside the organisation's controls, regardless of who pays for it.
- **Improperly obtained input** stays improper whatever tool analyses it, and however the output is anonymised.
- **Covert monitoring of staff** is an ethics and legal problem that anonymisation does not solve.
- **Judgement stays human.** Claude helps structure and word a performance document, an assessment, a recommendation. It does not form the judgement.
- **Answer client questions about AI use honestly**, and explain the review applied.
- Blocked by policy but the case is good? **Work within it and raise it through the governance channel with the controls that would be needed.** Do not seek a workaround, and do not ask a line manager to waive an organisational policy.

---

## 7. Workflow and stakeholders

**Augment** inserts Claude into existing steps. **Redesign** reconsiders which steps need to exist at all — higher value, higher change cost. Both are in Associate scope; process redesign is named in the intended audience.

**Segment before recommending.** Good candidates are high-volume, text-heavy, rule-based. Poor candidates need judgement, system access, or authority.

**Limitations are part of the deliverable.** Presenting to a sceptical stakeholder, name the failure mode, then show the specific controls and what each one catches. Never lead with time saved alone. Never claim Claude outperforms the team.

**"It feels faster" is not a measurement.** Check against the measures set at the outset, error rates included — a workflow can save time while degrading quality.

**Claude supports; accountable people decide and own.** Surface options, stress-test assumptions, draft alternatives, model effects. It does not select, approve, authorise, or implement.

---

## 8. Prompting and troubleshooting

**Effective prompts specify** the audience, the decision the output must support, the constraints, and success criteria. For voice or format consistency, **supply exemplars** — describing a voice does not reproduce it.

**Adapt to the task type.** Brainstorming wants divergent volume with feasibility filtering deferred. Analysis wants criteria and comparisons. Research wants scope, sourcing, and visible uncertainty. Drafting wants audience and constraints.

**Decompose** by sequencing sub-tasks with checkpoints: establish findings, review them, *then* write from the confirmed findings. A longer preamble is not decomposition.

**Iterate by naming the defect**, not by intensifying the request. "Be more concise" fails; a word ceiling and a required structure succeed. "Make it warmer" fails; naming what is wrong and showing one line of the target succeeds. Keep what worked.

**Diagnostic order for bad output:**

1. Is a requirement buried, vague, or unmeasurable? Make it explicit and structured.
2. Do two instruction layers **conflict** — prompt against Project instructions? Reconcile them; do not re-prompt around it.
3. Has the **configuration** changed — edited instructions, a superseded knowledge source?
4. Is context **crowded** by a long conversation? Carry forward what still stands and start fresh.
5. Does it fail only on **harder cases** after real refinement? Now consider the tier.
6. Is it outside your **scope**? Escalate.

**Optimise by removing work, not speeding it up.** If a step is duplicated, eliminate it — put the template in the configuration so output arrives conforming, rather than reformatting twice.

---

## 9. Pacing

**2:00 per item.** At 60 minutes you should be at or past item 30.

- Flag and return. Over ~2:30 on an item, best guess, mark it, move on.
- **Never leave a blank.** No penalty for wrong.
- Read the qualifier: **FIRST**, **most appropriate**, **most important**, **independently**. Several options can be true — the question is which is *most*.
- Beware the option that is a real, sensible practice but not what was asked. Those are the good distractors.
- When two options look equally right, pick the one that adds a control or fixes a structure over the one that improves a prompt or changes a model.

---

## Friday checklist

- Confirm the Pearson VUE appointment, the start time, and whether it is online-proctored or a test centre.
- ID name must match the registration exactly.
- If online-proctored: run the system test, check camera and microphone, clear the desk, arrange a quiet room.
- **Reschedule cut-off is 24 hours before.** If you are going to move it, decide by Friday 9:00 AM.
- Log in 30 minutes early.
- Nothing new Friday. Read this sheet, then stop.

**On the day:** business judgement, not technical depth. You are the Associate who recognises limits and escalates — not the Architect who builds the integration.
