# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repository is

This is not a software project — it's a collection of **Claude Skills** (Markdown-based, instruction-following skill definitions) for academic reading and text study, written in Portuguese. There is no build, lint, or test tooling: the only "code" is the natural-language instructions inside each `SKILL.md`, which Claude interprets and follows at runtime when the skill is invoked.

## Repository structure

Each skill lives in its own top-level directory and is self-contained:

```
leitura-analitica-severino/
├── SKILL.md      # the skill definition (frontmatter + instructions Claude follows)
└── README.md      # human-facing description, for people browsing the repo
tutor-de-texto/
├── SKILL.md
└── README.md
leitura-guiada/
├── SKILL.md
└── README.md
```

- `SKILL.md` files start with YAML frontmatter (`name`, `description`). The `description` field is what a Claude Code instance uses to decide *when* to auto-invoke the skill — it must exhaustively cover the phrasings a user might use to trigger it, including indirect ones that don't name the skill explicitly.
- A skill is installed by copying its folder (containing `SKILL.md`) into the user's Claude skills directory, or by packaging the folder as a `.skill`/`.zip`.
- The root `README.md` is the index of skills in this kit; each skill's own `README.md` is a shorter, install-focused description of that one skill. Keep both in sync with the corresponding `SKILL.md` when a skill's behavior changes.

## The three skills

- **`leitura-analitica-severino/`** — Produces a formal analytical document (a *fichamento*) from an academic text, following Antônio Joaquim Severino's five-stage method (análise textual, temática, interpretativa, problematização, síntese pessoal). Output is always a downloadable `.md` file, with an optional CmapTools-format `.txt` concept map as an extra deliverable. Supports six output formats (bibliographic record, citations record, indicative/informative summary per NBR 6028, full review, or the full five-stage analytical record).
- **`tutor-de-texto/`** — Conducts an interactive, conversational, point-by-point tutoring session over an academic/technical text until the user can explain its core (theme, problem, thesis, conclusion) in their own words. Focused on the *process* (mandatory comprehension checks between concepts, never advancing without a real user response), not just the final document. Reorganizes the content into its own pedagogical sequence (not necessarily the text's own order). Also outputs a `.md` study roadmap at the end.
- **`leitura-guiada/`** — Accompanies the reader through a text sequentially, section by section, in the text's own original order — centered on the reader and their context, not on a method of analysis (that's `leitura-analitica-severino`) nor on a reorganized pedagogical sequence (that's `tutor-de-texto`). Runs a brief context interview, a pre-reading survey of what the reader already knows, checks comprehension section by section (explaining prerequisites on demand), and ends with a session report recommending further reading (foundational + interest-based). Always delivered as a downloadable `.md` file.

The three are designed to be complementary and are meant to work on user-supplied text only (pasted, uploaded, or linked) — all three explicitly forbid inventing content about a source text that wasn't provided.

## Working on skill definitions

When editing a `SKILL.md`:
- Preserve the distinction between the three skills' purposes: `leitura-analitica-severino` is about the *deliverable* (a structured record for later reference); `tutor-de-texto` is about the *process* of reaching comprehension via its own pedagogical reorganization of the content; `leitura-guiada` is about following the *text's own sequential order*, reader-centered rather than method- or pedagogy-centered. Don't blur them.
- The `description` frontmatter field drives auto-invocation matching — when adding new trigger phrasings or use cases to a skill's behavior, update `description` too, not just the body instructions.
- All three skills mandate delivering results as a downloadable file (never only as inline chat text) and forbid fabricating source content, biographical data, or quotes not present in the original text — preserve these constraints in any edits.
- `leitura-analitica-severino` has three distinct "modos de condução" (dialogue / in-document suggestions / direct expert mode) for stages 3–5 that change *how* content for those stages is obtained but never the final document's structure — keep this invariant intact when modifying that section.
