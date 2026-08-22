# How to practise with this repo

Reading the guide gets you familiar. It does not get you drilled, and it
cannot generate a question you haven't seen before. This file is about the
three things that do.

## a) Run it in Cowork

Clone this repo and point Claude — via Cowork, or Claude Code, or any tool
that can work against a local folder — at it as a project or working
directory. Kimi Cowork works the same way. The point is not novelty: it's
that the guide, the practice sets, and a running record of *your own* misses
are all in the same context at once.

That beats reading for one reason: a static page can't ask you anything, and
it can't remember what you got wrong last time. A tool sitting on this repo
can quiz you from `practice/`, score you, and — if you keep a running note of
your miss pattern in the same folder — start noticing before you do that your
misses cluster in one trap family rather than being random.

## b) The drill loop

This is how the guide's author actually prepared: fifteen minutes at a time,
often on a commute, one question at a time, no batching. Paste this to start
a session:

```
I'm preparing for the Claude Certified Associate – Foundations exam. Use the
practice sets in this repo's practice/ folder (frameworks.md, sequencing.md,
mock-exam-60.md) as your question bank. Run me through them one at a time:

- Ask one question, then wait for my answer.
- I'll answer with the bare letter(s) — e.g. "B" or "A,D".
- Tell me immediately whether I was right, and if not, why — name the trap
  family from practice/README.md, don't just restate the explanation.
- Keep a running score as we go.
- Then give me the next question. Don't show me the answer key up front and
  don't batch multiple questions together.

Start with frameworks.md, and skip anything I've already told you I got
right in this session.
```

Swap `frameworks.md` for `sequencing.md` or `mock-exam-60.md` depending on
what you're drilling. The reason bare-letter answers matter: on multi-response
items, a partial selection scores zero on the real exam, so answering the
same way here trains the actual discipline instead of a softer one.

## c) Generating your own questions

This is the part that makes the repo keep being useful after you've exhausted
`practice/` — and it matters more than anything already written here, because
it's how you get unlimited practice from a fixed set of published objectives.

**The tool.** `tools/check-item-quality.py` — copied into this repo from the
same tool used to audit everything in `practice/` — measures whether a set of
items has an exploitable cue: answers clustering on one letter, the correct
option systematically the longest, a punctuation tell, and a few others. See
`tools/README.md` for what each metric means.

**Why this matters, with real numbers.** Every set in this repo failed at
least once before it passed. A draft of the mock exam had the correct answer
as the longest option in **94% of items** — a reader with zero subject
knowledge could have scored roughly 51/60 by picking the longest option every
time. The same draft had a dash, colon or semicolon in the correct answer in
**89% of items**. A sequencing set was **16 of 18 answer "A"**, with a run of
13 in a row, because the author habitually wrote the correct ordering first.
None of this was visible on a normal read-through. All of it showed up the
moment someone measured it — which is exactly the risk you take on when you,
or a model on your behalf, write new items and don't check them.

**The prompt.** Paste this, naming a real objective from the exam guide's
domain list (see `SOURCES.md`) and pointing at the item format you want
matched:

```
Using only the domain/objective list in this repo's SOURCES.md, write 5 new
multiple-choice practice items testing the objective "<name the objective>".
Match this repo's existing item format exactly — see practice/frameworks.md
for the pattern: a numbered stem, lettered options, and a collapsed
<details><summary>Answer</summary> block with a rationale that names why each
wrong option is wrong.

Constraints:
- Do not use, paraphrase, or reconstruct any real exam question — write these
  from the published objective description only.
- The correct answer must not be systematically the longest option.
- No dash/colon/semicolon that appears only in correct answers.
- Vary the correct letter across the 5 items — don't cluster on one letter.

When you're done, tell me you're ready for me to run:
  python3 tools/check-item-quality.py <the file you just wrote>
and fix anything it flags before I use these to study.
```

Then actually run the check. An unaudited set is a plausible-looking set,
which is worse than an obviously incomplete one, because it feels like
knowledge and isn't.

**What's not shipped, and why.** `_workspace/tools/check-provenance.py` — the
other check this guide's own material was audited with — is deliberately not
included here. It works by comparing your text against a source corpus (the
Academy course captures and the official exam guide) to catch reproduced
phrasing, and that corpus is private material you won't have a copy of. What
it did for this guide: found and removed 48 verbatim passages and roughly 27
objective statements that had been reproduced word for word from the official
exam guide, before this guide was ever published. If you're generating items
with a model, the practical substitute is the instruction above — "from the
published objective description only" — plus your own judgement about
whether a sentence you're reading sounds like it was lifted rather than
written.
