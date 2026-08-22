# Changelog

This repository has no git history before 22 August 2026. The container the
guide was originally developed in does not survive on this machine, and its
six commit messages could not be recovered — what follows for that period is
a summary of what happened, not a reproduction of the original commits.

## Pre-restructure history

Before this repository existed, the guide went through six commits in a
separate, now-unrecoverable container, covering (summarised, not quoted):

- Initial draft of the guide from the exam objectives and Academy course
  material.
- A cue-quality audit of the practice sets, which found and fixed a
  sequencing set that was 16 of 18 answer A with a 13-item run, a frameworks
  set with zero A answers at all, and a mock exam beatable by picking the
  longest option in 94% of items.
- A provenance audit against the captured Academy material, which found and
  removed 48 verbatim passages and roughly 27 objective statements reproduced
  word for word from the official exam guide.
- Packaging into the tarball this guide was later extracted from.

## 2026-08-22 — Extracted into a structured workspace

The guide was extracted from its tarball into a shared workspace alongside
material for the other three Claude certification credentials, under a
structure where everything publishable lived in one place and everything
sensitive — captured course material, official exam guides, third-party
study guides — was excluded by construction rather than by `.gitignore`
pattern alone. An independent review of that workspace found and fixed
several defects in the quality-gate scripts this guide's own material had
already been checked against (line-based scanning that a hard-wrap could
defeat, two fail-open paths, a licence-detection gap in the fetch tool) —
this guide's own audited state was unaffected, but the tools that had done
the auditing were made more trustworthy for what came after.

## 2026-08-23 — Split into its own repository

The shared workspace held material for four credentials and was reorganised
into four independent repositories, one per credential, rather than a single
monorepo — simpler, and it means nothing sensitive from the other three
credentials' working material ever shares a repository boundary with this
guide. This repository is the result: the Associate – Foundations guide,
its practice sets, and the tooling it needs to stay auditable, with no
dependency on anything outside it.

Also added in the split: `HOW-TO-PRACTISE.md` and `tools/check-item-quality.py`
(copied in from the shared workspace, with `tools/README.md` documenting what
it checks) — the guide had good content and no instructions for turning that
content into a study habit. That gap mattered more than anything else
missing at the time.
