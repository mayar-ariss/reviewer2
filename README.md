# Reviewer 2

**An agent skill for writing and revising research papers, theses and proposals, in which every rule cites one named authority. It covers introductions, from John M. Swales's Create-a-Research-Space (CARS) model; literature reviews, from Feak and Swales's *Telling a Research Story*; Methods sections, from Swales and Feak's condensed and extended types; and Discussions, from Moreno and Swales's functional scheme. For any part of a paper it also checks the claims (Ken Hyland), the sentences (Gopen and Swan), what pronouns and *this* point to (Halliday and Hasan), vague quantities (Channell), dense or empty wording (Halliday), truisms and uninformative sentences (Grice) and vague or abstract word choice (Strunk).**

```bash
npx skills add mayar-ariss/reviewer2
```

Works with Claude Code, Cursor, Codex, GitHub Copilot, Gemini CLI and any agent the [skills CLI](https://skills.sh) supports.

## What it does

The skill keeps one rules file per part of the text, plus files for checks that apply to any part, and each file draws on a single authority. `SKILL.md` tells the agent which file to read for the task.

| Part or check | File | Authority |
|---|---|---|
| Introductions | `rules/introduction.md` | Swales 1990, 2004; Swales & Feak 1994, 2012 |
| Literature reviews | `rules/literature-review.md` | Feak & Swales 2009 |
| Methods | `rules/methods.md` | Swales 1990, 2004, 2008; Swales & Feak |
| Discussions | `rules/discussion.md` | Moreno & Swales 2018 |
| Claims, in any part | `rules/claims.md` | Hyland 2005, 2010, 2017; Hyland & Jiang 2023 |
| Sentences, in any part | `rules/sentences.md` | Gopen & Swan 1990 |
| Reference, in any part | `rules/reference.md` | Halliday & Hasan 1976 |
| Vague quantities, in any part | `rules/vagueness.md` | Channell 1994 |
| Dense or empty wording, in any part | `rules/unpacking.md` | Halliday 1985, 1993 |
| Informativeness, in any part | `rules/informativeness.md` | Grice 1975 |
| Precision of wording, in any part | `rules/precision.md` | Strunk 1918 |

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

### Methods

From Swales and Feak's contrast between condensed and extended Methods sections, and Swales's observations on how Methods sections vary across disciplines: how much background to assume, shorthand versus description, subsections, saying how each step was done, justifying choices, and linking steps, all judged against what the target journal does. Swales and Feak give no fixed move structure for Methods, and neither does the skill.

### Discussions

From Moreno and Swales's scheme for the Discussion and other closing sections of empirical articles: five moves (background information, restating key results, commenting on them, evaluating the study, drawing implications) and their steps, labelled proposition by proposition. It checks that a Discussion interprets, compares and explains its results, states its contribution and limitations, and shows why the study matters beyond itself.

### Claims

From Ken Hyland's interpersonal model of metadiscourse and his work on hedging and stance: where each claim comes from, whether its certainty matches its evidence, why and how much fields hedge, explicit evaluation, self-mention, and the commitment carried by reporting verbs such as *show* and *suggest*. It catches sentences that sound authoritative but have no source, no stated evidence and no writer standing behind them.

### Sentences

From Gopen and Swan's "The Science of Scientific Writing": the seven structural principles for placing information where readers expect it. Whose story a sentence tells belongs in the topic position, the action in the verb, and the new information to be stressed at the end; links between sentences are stated rather than left to the reader. It catches sentences that sound like conclusions but state no relation between specific things.

### Reference

From Halliday and Hasan's *Cohesion in English*: personal, demonstrative and comparative reference, and the requirement that every reference item point to something the reader can recover. It catches pronouns and possessives whose referent is missing, ambiguous, or does not make sense in the clause.

### Vague quantities

From Channell's *Vague Language*: the forms vague quantities take (approximators, round numbers, quantifiers such as *many* and *how much*, vague categories) and the jobs vagueness does, from giving the right amount of information to withholding, persuading and covering missing information. It asks for the figure where vagueness withholds or persuades, and leaves approximations alone where they suffice.

### Dense or empty wording

From Halliday's work on grammatical metaphor: congruent and metaphorical wording, nominalization, and the favourite clause type of scientific English, which packs two events and a relation into "A gives B". Unpacking a sentence into congruent wording shows what it says, and whether its participants, processes and relations are there at all.

### Informativeness

From Grice's Cooperative Principle and conversational maxims: each sentence should be as informative as the point requires, true and supported, relevant and clear. It catches truisms and platitudes ("What a simulation can say depends on how real its inputs are"), asks the author what they were meant to imply, and does not replace them with claims the evidence cannot support.

### Precision

From Strunk's *The Elements of Style* (1918): prefer the specific to the general, the definite to the vague and the concrete to the abstract; make definite assertions; omit needless words. It catches loose everyday words standing in for technical properties (inputs that are "real" rather than accurate, uncertain or representative) and general classes where a particular case is meant, and lists the candidate terms for the author to choose from.

## Try it

Once installed, ask your agent the way you normally would:

- *"Review the introduction of my paper with the reviewer2 skill."*
- *"Label the moves in this introduction and tell me what's missing."*
- *"My Move 2 is weak. How can I state the gap?"*
- *"Should my introduction announce the main findings? The paper is for a physics journal."*
- *"Review the literature review chapter of my dissertation with the reviewer2 skill."*
- *"My Methods section is for an interdisciplinary journal. Is it too condensed?"*
- *"Label the moves in my Discussion. Did I state the contribution and the limitations?"*
- *"Check the claims in my Discussion: am I overstating anything?"*
- *"This paragraph is hard to follow. Check whose story each sentence tells and where the action is."*
- *"Unpack the key sentences in my abstract. Do they actually say anything?"*
- *"Are there sentences in my Discussion that just state the obvious?"*

## Faithful to its sources

Every rule names its source, and no rule combines authorities. Most rules cite the work and page; an article read in a reprint without page numbers is cited by section; where the primary work was not available, the rule cites it as reported in a named open source, listed in that rules file. Where an authority gives no rule (an introduction's length, the number of citations, a required opening sentence), the skill says so instead of supplying one. The skill keeps the author's claims and citations, and asks for content a rule needs rather than inventing it.

## Planned

- **Results:** Swales & Feak, *Academic Writing for Graduate Students*
- **Claims, extended:** the engagement side of Hyland's stance and engagement model (*Discourse Studies*, 2005)

## Based on

- Swales, J. M. (1990). *Genre Analysis: English in Academic and Research Settings*. Cambridge University Press.
- Swales, J. M. (2004). *Research Genres: Explorations and Applications*. Cambridge University Press.
- Swales, J. M., & Feak, C. B. (1994; 3rd ed. 2012). *Academic Writing for Graduate Students: Essential Tasks and Skills*. University of Michigan Press.
- Feak, C. B., & Swales, J. M. (2009). *Telling a Research Story: Writing a Literature Review*. University of Michigan Press.
- Feak, C. B., & Swales, J. M. (2011). *Creating Contexts: Writing Introductions across Genres*. University of Michigan Press.
- Swales, J. M. (2008). Variation in methods sections of research articles. Talk abstract, METM08, Mediterranean Editors and Translators.
- Moreno, A. I., & Swales, J. M. (2018). Strengthening move analysis methodology towards bridging the function-form gap. *English for Specific Purposes*, 50, 40–63.
- Hyland, K. (2005). Prudence, precision, and politeness: Hedges in academic writing. *Quaderns de Filologia. Estudis Lingüístics*, X, 99–112.
- Hyland, K. (2010). Metadiscourse: Mapping interactions in academic writing. *Nordic Journal of English Studies*, 9(2), 125–143.
- Hyland, K. (2017). Metadiscourse: What is it and where is it going? *Journal of Pragmatics*, 113, 16–29.
- Hyland, K., & Jiang, F. K. (2023). Talking to the literature: Stance taking in citing others' work. In R. Wette (Ed.), *Teaching and learning source-based writing*. Routledge.
- Gopen, G. D., & Swan, J. A. (1990). The science of scientific writing. *American Scientist*, 78(6), 550–558.
- Halliday, M. A. K., & Hasan, R. (1976). *Cohesion in English*. Longman.
- Channell, J. (1994). *Vague Language*. Oxford University Press.
- Halliday, M. A. K. (1985). *An Introduction to Functional Grammar*. Edward Arnold.
- Halliday, M. A. K. (1993). Some grammatical problems in scientific English. In M. A. K. Halliday & J. R. Martin, *Writing Science: Literacy and Discursive Power*. Falmer.
- Grice, H. P. (1975). Logic and conversation. Reprinted in *Studies in the Way of Words* (1989). Harvard University Press.
- Strunk, W., Jr. (1918). *The Elements of Style*. Public domain.

The skill paraphrases these works and cites them; it does not reproduce their text. Read the originals for the full treatment, examples and exercises.

## License

MIT; see [LICENSE](LICENSE).
