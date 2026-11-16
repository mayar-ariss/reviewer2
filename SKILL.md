---
name: reviewer2
description: >-
  Review, critique or revise a research paper the way a demanding peer reviewer
  would, with every comment tied to a named authority on academic writing. Use this
  skill whenever the user asks to review, check, edit, tighten or improve any part
  of a research article, manuscript, thesis or dissertation chapter: the title,
  abstract, introduction, literature review, Methods, Results, Discussion or
  conclusion, the text around figures and tables, or a whole manuscript before
  submission. Also use it when the user asks whether a sentence or claim is vague,
  generic, unsupported, overstated or hard to follow, or how a reviewer would read
  the draft, even if they never say "review". Rules come from Swales, Feak, Hyland,
  Cotos and colleagues, Moreno, Toulmin, Gopen and Swan, Halliday and Hasan,
  Channell and Grice; reporting-guideline and spin checks apply to health research
  only.
---

# Reviewer 2: research writing, rule by cited rule

This skill reviews and revises parts of a research article, and the matching chapters of a thesis or dissertation. It does not model the structure of a whole thesis or of a research proposal, although the literature-review file covers their reviews. Its rules come from published analyses of academic writing and research reporting, kept in rules files that each draw on one authority: one file per part of the text, plus files for checks that apply to any part.

**Every rule names its source.** Most rules cite the work and page; an article read in a reprint without page numbers is cited by section; where the primary work was not available, the rule cites it as reported in a named open source. Each rules file names its authority at the top and draws only on that authority; no rule combines authorities. Where an authority gives no rule, the file says so rather than supplying one. Nothing here is a general writing preference.

## Which file to read

**Parts of the text**

| The user is working on | Read | Authority |
|---|---|---|
| The title | `rules/titles.md` | Hyland & Zou 2022 |
| The abstract | `rules/abstracts.md` | Hyland 2000 |
| The introduction of a research article | `rules/introduction.md` | Swales (CARS model) |
| A literature review: a review chapter, a proposal's review, or a review section | `rules/literature-review.md` | Feak & Swales 2009 |
| A review of previous work inside an introduction | `rules/introduction.md` (rules 3–5) together with `rules/literature-review.md` | Swales; Feak & Swales 2009 |
| The Methods section (Materials and Methods, Methodology, Experimental Procedures): detail, background and justification | `rules/methods.md` | Swales; Swales & Feak |
| The Methods section: which parts it contains, and in what order | `rules/methods-structure.md` | Cotos, Huffman & Link 2017 |
| The Results section (Findings) | `rules/results.md` | Cotos, Huffman & Link 2015 |
| The Discussion of a research article, including a combined Results and Discussion or a closing Conclusion | `rules/discussion.md` | Moreno & Swales 2018 |

**Checks for any part**

| The user wants checked | Read | Authority |
|---|---|---|
| Claims: their sources, how strongly they are stated, evaluation, self-mention, reporting verbs, and how the text addresses the reader | `rules/claims.md` | Hyland |
| Data commentary: the text around each figure or table, which results it highlights, how it interprets them; data shown twice; the number of figures and tables against the journal | `rules/data-commentary.md` | Swales & Feak |
| Argument: whether each main claim has data, a warrant the reader would accept, backing, a stated strength and stated exceptions; whether each figure and table supports a claim | `rules/argument.md` | Toulmin 1958 |
| Sentences and paragraphs: whose story each sentence tells, where the action and the emphasis fall, the links between sentences | `rules/sentences.md` | Gopen & Swan 1990 |
| Cohesion: what pronouns, *this*, *the*, comparatives and substitutes point to; whether linking words signal the relation that holds; whether key terms are used consistently | `rules/cohesion.md` | Halliday & Hasan 1976 |
| Vague quantities and categories: *about*, *many*, *how much*, *and so on* | `rules/vagueness.md` | Channell 1994 |
| Dense or empty wording: nominalizations, relations packed into one verb, sentences that sound weighty but say little | `rules/unpacking.md` | Halliday |
| Informativeness: truisms, platitudes, sentences that tell the reader nothing new or have no clear point, and loose words for technical properties | `rules/informativeness.md` | Grice |
| Completeness (health research only): whether Methods and Results report the minimum information for the study design | `rules/reporting.md` | EQUATOR Network |
| Spin (health research only): misreported methods or results, interpretation beyond the results, conclusions stronger than the evidence | `rules/spin.md` | Boutron & Ravaud 2018 |

Read only the files the task needs. `rules/index.md` lists every rule in one line each; use it to choose which checks to run, then open only the files whose checks you need.

- **Full review** of a title, abstract, introduction, literature review, Methods, Results or Discussion: read the draft once, note the problems most visible in it, and match them to checks in `rules/index.md`; apply the section's file first (for Methods, both `rules/methods.md` and `rules/methods-structure.md`), then the checks in this order: `rules/data-commentary.md` (for sections that comment on figures or tables), `rules/claims.md`, `rules/argument.md` (for argued sections such as the Discussion), `rules/spin.md` (health research only), `rules/reporting.md` (health research only; Methods and Results), `rules/sentences.md`, `rules/cohesion.md`, `rules/vagueness.md`, `rules/unpacking.md`, `rules/informativeness.md`. Run first the checks that address the problems you noted, then the rest in this order.
- **Whole manuscript:** review each section in the paper's order, as a full review, then check the sections against each other:
  - any result the title states is supported by the paper (`rules/titles.md`, rule 4);
  - every finding in the abstract appears in the Results (`rules/abstracts.md`, rule 5);
  - each question, hypothesis or purpose set out in the introduction (`rules/introduction.md`, rule 9) has its results reported (`rules/results.md`, rule 1);
  - the Discussion restates and interprets the results the Results section reports, and each of its main claims rests on them (`rules/discussion.md`, rules 5–6; `rules/argument.md`, rule 1);
  - each figure and table supports a claim (`rules/argument.md`, rule 6), and their number has been compared with the target journal (`rules/data-commentary.md`, procedure).
- **Quick review:** apply the section file, then only the two or three checks in `rules/index.md` that address the problems most visible in the draft, and say which checks were not run.

**Parts this skill does not cover yet:** the structure of a whole thesis and of a research proposal, apart from the checks for any part. If the user asks about one of these, say that this skill has no rules for its structure. Do not stretch the rules above to cover it, and do not supply rules of your own.

## How to apply any rules file

*Procedure for this skill, not a rule from any authority.*

1. **Establish the context.** Ask for the field, the target journal or degree, the genre and, for empirical work, the study design, or read them from the draft. Many rules depend on them. If they cannot be found and the user is not there to ask, state your assumption once at the top of the review, and mark the findings that depend on the field or journal as conditional on it.
2. **Follow the procedure at the top of the rules file.** Where it asks you to label each sentence and the draft is long, label paragraphs first, then label sentences only in the paragraphs where a check finds a problem. Keep every question for the author for the end of the review (see *How to present a review*), rather than stopping at each one.
3. **Cite the rule behind every proposed change**, by file and number (for example, "introduction, rule 7").
4. **Keep the author's content.** Keep the author's claims, data and citations. Never invent findings, gaps, references, figures or evaluations; where a rule needs content the draft does not have, ask the author for it. Check that the numbers in the draft agree with each other and with its tables and figures; where a value does not, or looks copied from another row, column or place, ask the author to confirm it rather than correcting it.
5. **Finish with the rules file's checklist.** Run it every time; show it in the review only when the draft is longer than a paragraph or the user asks for it.

## How to present a review

*Procedure for this skill, not a rule from any authority.*

1. **Group findings by passage**, not by rules file, so the author sees everything about one sentence or paragraph in one place.
2. **Merge findings that make the same point.** Where several files flag the same problem (for example, a claim stronger than its data, flagged by the claims, argument and data commentary files), report it once and cite every rule behind it.
3. **Order by consequence:** problems of structure and argument first (missing moves, unsupported claims, results that do not answer the questions), then interpretation and stance, then sentences and words.
4. **Separate what to change from what to ask.** List proposed revisions apart from the questions only the author can answer: missing content, intended referents, explanations.
5. **Say what was not covered:** the checks not run, and any part of the draft this skill has no rules for.
6. **Fit the length of the review to the draft.** For a draft of a sentence or a short paragraph, give the findings, the proposed revisions and the questions; say in one line which checks were run and which were not, and leave out the labelled outline, the checklists and the assumptions beyond one line. Expand only for longer drafts or when the user asks.

## Sources

Each rules file lists its sources, and how it cites them, at its end. The README lists every work the skill draws on.
