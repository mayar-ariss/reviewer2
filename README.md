# Reviewer 2

**An agent skill for writing and revising research papers, theses and proposals, in which every rule cites one named authority by work and page. It currently covers introductions, from John M. Swales's Create-a-Research-Space (CARS) model; literature reviews, from Feak and Swales's *Telling a Research Story*; and the claims in any part of a paper, from Ken Hyland's work on stance and metadiscourse.**

```bash
npx skills add mayar-ariss/reviewer2
```

Works with Claude Code, Cursor, Codex, GitHub Copilot, Gemini CLI and any agent the [skills CLI](https://skills.sh) supports.

## What it does

The skill keeps one rules file per part of the text, plus one for claims, and each file draws on a single authority. `SKILL.md` tells the agent which file to read for the task.

| Part | File | Authority |
|---|---|---|
| Introductions | `rules/introduction.md` | Swales 1990, 2004; Swales & Feak 1994, 2012 |
| Literature reviews | `rules/literature-review.md` | Feak & Swales 2009 |
| Claims, in any part | `rules/claims.md` | Hyland 2005, 2010, 2017; Hyland & Jiang 2023 |

### Introductions

John M. Swales's analysis of research article introductions found a recurring pattern of three rhetorical moves, which he called Create a Research Space (CARS):

| Move | What it does |
|---|---|
| **1. Establishing a territory** | Shows the research area and reviews previous work, from general to specific |
| **2. Establishing a niche** | Shows that the research story is not yet complete: a gap, an addition, a question, a continuation |
| **3. Presenting the present work** | States what this paper does, and, where the field expects it, its questions, methods, findings, value and structure |

The skill uses Swales's 2004 revision of the model as its default and his 1990 steps as finer options. It labels a draft sentence by sentence, checks each move, and proposes revisions citing the rule behind each one.

It also applies Swales and Feak's guidance on:

- where the purpose statement goes, and why most papers don't open with it
- integral and non-integral citations, and the three tense patterns for citing
- the signals that mark the start of Move 2, and alternatives to an outright gap
- tense in purpose statements
- which optional Move 3 elements a field expects

### Literature reviews

From Feak and Swales's *Telling a Research Story*: why the review is there and how it leads to your research, imposing order on the literature, describing selection criteria, metadiscourse, integral and non-integral citations, citation tense, reporting verbs and ambiguous citations, taking a stance, and paraphrasing and summarizing in your own words.

### Claims

From Ken Hyland's interpersonal model of metadiscourse and his work on hedging and stance: where each claim comes from, whether its certainty matches its evidence, why and how much fields hedge, explicit evaluation, self-mention, and the commitment carried by reporting verbs such as *show* and *suggest*. It catches sentences that sound authoritative but have no source, no stated evidence and no writer standing behind them.

## Try it

Once installed, ask your agent the way you normally would:

- *"Review the introduction of my paper with the reviewer2 skill."*
- *"Label the moves in this introduction and tell me what's missing."*
- *"My Move 2 is weak. How can I state the gap?"*
- *"Should my introduction announce the main findings? The paper is for a physics journal."*
- *"Review the literature review chapter of my dissertation with the reviewer2 skill."*
- *"Check the claims in my Discussion: am I overstating anything?"*

## Faithful to its sources

Every rule names its source by work and page, and no rule combines authorities. Where an authority gives no rule (an introduction's length, the number of citations, a required opening sentence), the skill says so instead of supplying one. The skill keeps the author's claims and citations, and asks for content a rule needs rather than inventing it.

## Planned

Each part will be added only once its rules can be cited by page from the source:

- **Methods, Results and Discussion:** Swales & Feak, *Academic Writing for Graduate Students*
- **Claims, extended:** the engagement side of Hyland's stance and engagement model, once his *Discourse Studies* article (2005) can be cited by page
- **Empty sentences:** unpacking abstract wording into its congruent form, from M.A.K. Halliday

## Based on

- Swales, J. M. (1990). *Genre Analysis: English in Academic and Research Settings*. Cambridge University Press.
- Swales, J. M. (2004). *Research Genres: Explorations and Applications*. Cambridge University Press.
- Swales, J. M., & Feak, C. B. (1994; 3rd ed. 2012). *Academic Writing for Graduate Students: Essential Tasks and Skills*. University of Michigan Press.
- Feak, C. B., & Swales, J. M. (2009). *Telling a Research Story: Writing a Literature Review*. University of Michigan Press.
- Feak, C. B., & Swales, J. M. (2011). *Creating Contexts: Writing Introductions across Genres*. University of Michigan Press.
- Hyland, K. (2005). Prudence, precision, and politeness: Hedges in academic writing. *Quaderns de Filologia. Estudis Lingüístics*, X, 99–112.
- Hyland, K. (2010). Metadiscourse: Mapping interactions in academic writing. *Nordic Journal of English Studies*, 9(2), 125–143.
- Hyland, K. (2017). Metadiscourse: What is it and where is it going? *Journal of Pragmatics*, 113, 16–29.
- Hyland, K., & Jiang, F. K. (2023). Talking to the literature: Stance taking in citing others' work. In R. Wette (Ed.), *Teaching and learning source-based writing*. Routledge.

The skill paraphrases these works and cites them; it does not reproduce their text. Read the books for the full treatment, examples and exercises.

## License

MIT; see [LICENSE](LICENSE).
