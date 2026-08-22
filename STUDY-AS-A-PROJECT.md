# Run This as a Project

The most effective way to use this repo is not to read it. It is to turn it into a **personalised study partner** that knows your weak spots and drills them.

There is a nice circularity to this. Setting up standing context so Claude can work on a recurring task without being re-briefed *is* **Agency mode** — one of the three engagement modes the exam tests. Configuring the Project teaches you the objective while you use it.

---

## Why this beats reading

A static guide gives everyone the same thing. Your miss pattern is not everyone's.

The candidate this repo is built from had **essentially no knowledge gaps** — every miss came from misreading a stated count or choosing a plausible-but-soft option. Reading more would have fixed nothing. What fixed it was targeted drilling on those two specific failures, and the final session — ten items built entirely from their own logged misses — scored ten out of ten.

You cannot get that from a document. You can get it from a Project that remembers what you keep getting wrong.

---

## Setup

### Global instructions · who you are

These apply to every session, in Cowork and in chat. Settings → Cowork → Global instructions, or the personalisation settings in Claude.ai.

Keep it to what is durable about you:

```
I work in [role] at [organisation type]. I am preparing for the Claude
Certified Associate – Foundations exam (CCAO-F).

When you quiz me, present one item at a time and wait for my answer before
revealing anything. Tell me right or wrong, give a one-line reason, then go
straight to the next item. Keep a running score in the form "N/M · item X of M".

Never show me an answer before I have committed to one.
```

That last line matters more than it looks. The whole mechanism depends on attempting before reading, and it is easy to let slip.

### Project · what you are working on

Create a Project called something like *CCAO-F prep*. Add as **context** or **knowledge sources**:

- `index.html` from this repo, or the published guide page
- `practice/frameworks.md`
- `practice/sequencing.md`
- `practice/mock-exam-60.md` and its key
- The official CCAO-F exam guide PDF
- **Your own miss log** — the single most valuable file in the Project

Then the project instructions. This is where the personalisation lives:

```
This project is for preparing me for the CCAO-F exam.

Draw questions from the practice files in this project's knowledge. Never
invent questions about actual exam content, and never ask me to recall exam
items — everything comes from the published objectives.

When I get an item wrong, do three things:
  1. Name the trap family, not just the correct answer
  2. Add it to my miss log with the date and the bucket
  3. Later in the same session, give me a different item testing the same
     discrimination in an unrelated scenario

Track my misses in three buckets: didn't know it / misread the item / chose
the plausible-but-soft option. When I ask how I am doing, report the bucket
distribution before the score — the distribution matters more.

On multi-response items, score content and count separately. If I give fewer
letters than the item asked for, say so explicitly as a procedural error
rather than a knowledge error.

For sequencing items, always begin your explanation by naming the engagement
mode — Automation, Augmentation or Agency.
```

---

## How to work in it

**Day one, cold.** "Quiz me on the framework items, one at a time." Do not read the guide first. The point is to find out what you do not know, and reading first destroys the measurement.

**Then let it drive.** "What are my weakest three areas?" It has the miss log. It knows.

**Same discrimination, new scenario.** "Give me another item testing that, in a different domain." This is the antidote to the failure that catches prepared candidates — a rule learned correctly and then defeated by an unfamiliar surface.

**Ask for the bucket split, not the score.** "How am I doing?" should return the distribution. A 70% with every miss in *didn't know it* is a better position than a 90% with three in *chose the soft option*, because the first is a reading list and the second is a habit.

**Build your final session from the log.** Near the end: "Give me ten items drawn only from my bucket-three misses." That is the highest-value hour available, and it exists only because the log does.

---

## Why a Project and not just a long chat

Because context does not carry across conversations on its own. That is a testable fact about the product and also the practical reason this works.

Away from a Project, every session begins from nothing except your global instructions — so your miss log lives nowhere and each session re-teaches from zero. Inside one, each conversation adds to what Claude holds about your preparation. Academy draws the line simply: **global instructions describe *you*, and a Project describes *the work*.**

The Project *is* the standing context. Which is the point being examined.

---

## Cowork or chat?

Either works. The distinction is the documented one:

- **Chat** if you want a quizzing partner, present for every turn.
- **Cowork** if you want it working on your files — maintaining the miss log as a real document, generating fresh item sets, producing a readiness summary you can look at between sessions.

Cowork suits the log-keeping better because the log is a file that should persist and grow. Chat suits the drilling. Using both, for the jobs they fit, is itself an answer to a D3 objective.

---

## One warning

**Do not ask Claude to recall or reconstruct exam questions**, and be sceptical of any study partner that offers to. Exam content is confidential, anything presenting itself as real items is either fabricated or a breach, and using it puts your credential at risk.

Everything in this repo is written from published objectives. Keep it that way in your own Project.
