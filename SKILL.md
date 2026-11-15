---
name: reviewer2
description: >-
  Use when writing, reviewing or revising a research article, thesis, dissertation
  or proposal. Section rules: abstracts (Hyland), introductions (Swales's CARS
  model), literature reviews (Feak and Swales), Methods (Swales and Feak; Cotos,
  Huffman and Link), Results (Link), Discussions (Moreno and Swales). Checks for
  any part: claims, hedging and
  reader engagement, argument (Toulmin), sentence structure, reference, vague
  quantities, dense or empty wording, truisms, word precision, completeness against
  reporting guidelines, and spin. Every rule cites one named authority.
---

# Reviewer 2: research writing, rule by cited rule

This skill reviews and revises parts of a research article, thesis, dissertation or proposal. Its rules come from published analyses of academic writing and research reporting, kept in rules files that each draw on one authority: one file per part of the text, plus files for checks that apply to any part.

**Every rule names its source.** Most rules cite the work and page; an article read in a reprint without page numbers is cited by section; where the primary work was not available, the rule cites it as reported in a named open source. Each rules file names its authority at the top and draws only on that authority; no rule combines authorities. Where an authority gives no rule, the file says so rather than supplying one. Nothing here is a general writing preference.

## Which file to read

**Parts of the text**

| The user is working on | Read | Authority |
|---|---|---|
| The abstract | `rules/abstracts.md` | Hyland 2000 |
| The introduction of a research article | `rules/introduction.md` | Swales (CARS model) |
| A literature review: a review chapter, a proposal's review, or a review section | `rules/literature-review.md` | Feak & Swales 2009 |
| A review of previous work inside an introduction | `rules/introduction.md` (rules 3–5) together with `rules/literature-review.md` | Swales; Feak & Swales 2009 |
| The Methods section (Materials and Methods, Methodology, Experimental Procedures): detail, background and justification | `rules/methods.md` | Swales; Swales & Feak |
| The Methods section: which parts it contains, and in what order | `rules/methods-structure.md` | Cotos, Huffman & Link 2017 |
| The Results section (Findings) | `rules/results.md` | Link 2023 |
| The Discussion of a research article, including a combined Results and Discussion or a closing Conclusion | `rules/discussion.md` | Moreno & Swales 2018 |

**Checks for any part**

| The user wants checked | Read | Authority |
|---|---|---|
| Claims: their sources, how strongly they are stated, evaluation, self-mention, reporting verbs, and how the text addresses the reader | `rules/claims.md` | Hyland |
| Argument: whether each main claim has data, a warrant the reader would accept, backing, a stated strength and stated exceptions | `rules/argument.md` | Toulmin 1958 |
| Sentences and paragraphs: whose story each sentence tells, where the action and the emphasis fall, the links between sentences | `rules/sentences.md` | Gopen & Swan 1990 |
| Reference: what pronouns, possessives, *this*, *the* and comparatives point to | `rules/reference.md` | Halliday & Hasan 1976 |
| Vague quantities and categories: *about*, *many*, *how much*, *and so on* | `rules/vagueness.md` | Channell 1994 |
| Dense or empty wording: nominalizations, relations packed into one verb, sentences that sound weighty but say little | `rules/unpacking.md` | Halliday |
| Informativeness: truisms, platitudes and sentences that tell the reader nothing new or have no clear point | `rules/informativeness.md` | Grice |
| Precision: loose words for technical properties, general classes where a particular case is meant, noncommittal or padded phrasing | `rules/precision.md` | Strunk 1918 |
| Completeness: whether Methods and Results report the minimum information for the study design | `rules/reporting.md` | EQUATOR Network |
| Spin: misreported methods or results, interpretation beyond the results, conclusions stronger than the evidence | `rules/spin.md` | Boutron & Ravaud 2018 |

Read only the files the task needs.

- **Full review** of an abstract, introduction, literature review, Methods, Results or Discussion: apply its file first (for Methods, both `rules/methods.md` and `rules/methods-structure.md`), then the checks in this order: `rules/claims.md`, `rules/argument.md` (for argued sections such as the Discussion), `rules/spin.md`, `rules/reporting.md` (for Methods and Results), `rules/sentences.md`, `rules/reference.md`, `rules/vagueness.md`, `rules/unpacking.md`, `rules/informativeness.md`, `rules/precision.md`.
- **Quick review:** apply the section file, then only the two or three checks that address the problems most visible in the draft, and say which checks were not run.

**Parts this skill does not cover yet:** titles, apart from the checks for any part. If the user asks about one of these, say that this skill has no rules for its structure. Do not stretch the rules above to cover it, and do not supply rules of your own.

## How to apply any rules file

*Procedure for this skill, not a rule from any authority.*

1. **Establish the context.** Ask for the field, the target journal or degree, the genre and, for empirical work, the study design, or read them from the draft. Many rules depend on them.
2. **Follow the procedure at the top of the rules file.**
3. **Cite the rule behind every proposed change**, by file and number (for example, "introduction, rule 7").
4. **Keep the author's content.** Keep the author's claims, data and citations. Never invent findings, gaps, references, figures or evaluations; where a rule needs content the draft does not have, ask the author for it.
5. **Finish with the rules file's checklist.**

## Sources

| Short form | Work | Used in |
|---|---|---|
| Swales 1990 | *Genre Analysis: English in Academic and Research Settings*. Cambridge University Press. | `rules/introduction.md` |
| Swales 2004 | *Research Genres: Explorations and Applications*. Cambridge University Press. | `rules/introduction.md` |
| Swales & Feak 1994 | *Academic Writing for Graduate Students* (AWG), 1st ed. University of Michigan Press. | `rules/introduction.md` |
| Swales & Feak 2012 | *Academic Writing for Graduate Students*, 3rd ed. University of Michigan Press. | `rules/introduction.md` |
| Feak & Swales 2009 | *Telling a Research Story: Writing a Literature Review*. University of Michigan Press. | `rules/literature-review.md` |
| Feak & Swales 2011 | *Creating Contexts: Writing Introductions across Genres*. University of Michigan Press. | `rules/introduction.md` (scope note) |
| Swales 1990, 2004; AWG (Methods) | Swales's and Swales & Feak's accounts of Methods sections. Cited as reported in open sources. | `rules/methods.md` |
| Swales 2008 | Variation in methods sections of research articles. Talk abstract, METM08. | `rules/methods.md` |
| CHL 2017 | Cotos, E., Huffman, S., & Link, S. A move/step model for methods sections. *English for Specific Purposes* 46. Accepted manuscript. | `rules/methods-structure.md` |
| Link 2023 | Link, S. *Writing for Publication* (open textbook, CC BY 4.0), with *Preparing to Publish* (Iowa State University, open textbook). | `rules/results.md` |
| M&S 2018 (MS) | Moreno, A. I., & Swales, J. M. Strengthening move analysis methodology towards bridging the function-form gap. *English for Specific Purposes*, 50, 40–63. Authors' preprint. | `rules/discussion.md` |
| Hyland 2010 | Metadiscourse: Mapping interactions in academic writing. *Nordic Journal of English Studies*, 9(2), 125–143. | `rules/claims.md` |
| Hyland 2005 | Prudence, precision, and politeness: Hedges in academic writing. *Quaderns de Filologia. Estudis Lingüístics*, X, 99–112. | `rules/claims.md` |
| Hyland 2017 (MS) | Metadiscourse: What is it and where is it going? *Journal of Pragmatics*, 113, 16–29. Author's manuscript. | `rules/claims.md` |
| Hyland & Jiang 2023 (MS) | Talking to the literature: Stance taking in citing others' work. In R. Wette (Ed.), *Teaching and learning source-based writing*. Routledge. Authors' manuscript. | `rules/claims.md` |
| G&S 1990 | Gopen, G. D., & Swan, J. A. The science of scientific writing. *American Scientist*, 78(6), 550–558. Cited by section. | `rules/sentences.md` |
| H&H 1976 | Halliday, M. A. K., & Hasan, R. *Cohesion in English*. Longman. Cited as reported in open sources. | `rules/reference.md` |
| Channell 1994 | Channell, J. *Vague Language*. Oxford University Press. Cited from its table of contents and as quoted in open sources. | `rules/vagueness.md` |
| Halliday 1985, 1993 | Halliday, M. A. K. *An Introduction to Functional Grammar* (1985); "Some grammatical problems in scientific English", in Halliday & Martin, *Writing Science* (1993). Cited as reported in open sources. | `rules/unpacking.md` |
| Grice | Grice, H. P. Logic and conversation (1975), in *Studies in the Way of Words* (1989). Cited as reported in open sources. | `rules/informativeness.md` |
| Strunk 1918 | Strunk, W., Jr. *The Elements of Style*. Public domain; cited by rule number. | `rules/precision.md` |
| EQUATOR | EQUATOR Network, key reporting guidelines and "What is a reporting guideline?". | `rules/reporting.md` |
| Hyland 2000 | Hyland, K. *Disciplinary Discourses*. Longman. Cited as reported in an open source. | `rules/abstracts.md` |
| Hyland 2023 | Hyland, K. Changing times; changing texts. WAC Clearinghouse, open access. | `rules/claims.md` (engagement) |
| Toulmin 1958 | Toulmin, S. *The Uses of Argument*. Cambridge University Press. Cited as reported in open sources. | `rules/argument.md` |
| B&R 2018 | Boutron, I., & Ravaud, P. Misrepresentation and distortion of research in biomedical literature. *PNAS*, 115(11), 2613–2619. Open access; cited by section. | `rules/spin.md` |

Page numbers refer to these editions. Each rules file gives its own citation conventions and lists its reporting sources.
