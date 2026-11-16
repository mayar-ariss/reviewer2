# Reviewer 2

**An agent skill for writing and revising research articles, and the matching chapters of theses and dissertations, in which every rule cites one named authority. It covers titles, from Hyland and Zou's study of research article titles; abstracts, from Hyland's five moves; introductions, from John M. Swales's Create-a-Research-Space (CARS) model; literature reviews, from Feak and Swales's *Telling a Research Story*; Methods sections, from Swales and Feak's condensed and extended types and Cotos, Huffman and Link's move/step model; Results, from Cotos, Huffman and Link's move/step framework; and Discussions, from Moreno and Swales's functional scheme. It checks the text that comments on figures and tables (Swales and Feak's data commentary). For any part of a paper it also checks the claims and how the text addresses the reader (Ken Hyland), the argument (Toulmin), the sentences (Gopen and Swan), cohesion: what pronouns and *this* point to, whether linking words fit, and whether key terms stay consistent (Halliday and Hasan), vague quantities (Channell), dense or empty wording (Halliday), truisms and obscure wording (Grice); for health research, it also checks completeness against reporting guidelines (EQUATOR) and spin (Boutron and Ravaud).**

```bash
npx skills add mayar-ariss/reviewer2
```

Works with Claude Code, Cursor, Codex, GitHub Copilot, Gemini CLI and any agent the [skills CLI](https://skills.sh) supports.

## What it does

The skill keeps one rules file per part of the text, plus files for checks that apply to any part, and each file draws on a single authority. `SKILL.md` tells the agent which file to read for the task.

| Part or check | File | Authority |
|---|---|---|
| Titles | `rules/titles.md` | Hyland & Zou 2022 |
| Abstracts | `rules/abstracts.md` | Hyland 2000 |
| Introductions | `rules/introduction.md` | Swales 1990, 2004; Swales & Feak 1994, 2012 |
| Literature reviews | `rules/literature-review.md` | Feak & Swales 2009 |
| Methods: detail and justification | `rules/methods.md` | Swales 1990, 2004, 2008; Swales & Feak |
| Methods: parts and order | `rules/methods-structure.md` | Cotos, Huffman & Link 2017 |
| Results | `rules/results.md` | Cotos, Huffman & Link 2015 |
| Discussions | `rules/discussion.md` | Moreno & Swales 2018 |
| Claims and reader engagement, in any part | `rules/claims.md` | Hyland 2005, 2010, 2017, 2023; Hyland & Jiang 2023 |
| Data commentary on figures and tables | `rules/data-commentary.md` | Swales & Feak 1995; AWG |
| Argument, in any part | `rules/argument.md` | Toulmin 1958 |
| Sentences, in any part | `rules/sentences.md` | Gopen & Swan 1990 |
| Cohesion, in any part | `rules/cohesion.md` | Halliday & Hasan 1976 |
| Vague quantities, in any part | `rules/vagueness.md` | Channell 1994 |
| Dense or empty wording, in any part | `rules/unpacking.md` | Halliday 1985, 1993 |
| Informativeness, in any part | `rules/informativeness.md` | Grice 1975 |
| Completeness of reporting, in Methods and Results (health research only) | `rules/reporting.md` | EQUATOR Network |
| Spin, in any part (health research only) | `rules/spin.md` | Boutron & Ravaud 2018 |

For a full review the agent applies the section's file and then every check; for a quick review it applies the section's file and the two or three checks most relevant to the draft, and says which it skipped.

### Titles

From Hyland and Zou's analysis of 5,070 titles in six disciplines: statements or questions, single or compound titles, descriptive titles or ones that also give the approach or a result, and length, all judged against the field and the target journal. It checks that the title names the paper's subject in searchable terms and adds no method or result the author has not stated.

### Abstracts

From Hyland's classification of moves in research article abstracts, drawn from 800 abstracts in eight disciplines: introduction, purpose, method, product and conclusion. It checks that the abstract states its purpose and its findings (not just that findings exist), frames the problem in proportion to the field, and claims nothing in its conclusion that the paper does not support.

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

From Swales and Feak's contrast between condensed and extended Methods sections, and Swales's observations on how Methods sections vary across disciplines: how much background to assume, shorthand versus description, subsections, saying how each step was done, justifying choices, and linking steps, all judged against what the target journal does. Swales and Feak give no fixed move structure for Methods.

### Methods structure

From Cotos, Huffman and Link's Demonstrating Rigour and Credibility (DRaC) model, built from the Methods sections of 900 articles in 30 disciplines: three moves (contextualizing the study methods, describing the study, establishing credibility) and sixteen steps. It labels each subsection by move and step, lists the steps the study needs but the draft lacks, checks that analysis follows the description it depends on, puts each rationale with its decision, and moves observations the findings rest on to Results.

### Results

From Cotos, Huffman and Link's move/step framework, built from 900 research articles in 30 disciplines: approaching the niche (orientation and study specifics), occupying it (reporting results and pointing to tables and figures), construing it (comparing, explaining and qualifying specific results) and, where discussion is integrated, expanding it. It checks that the section reports results for each question, keeps commentary within the scope of the study, and makes clear which kind of comment each sentence is.

### Discussions

From Moreno and Swales's scheme for the Discussion and other closing sections of empirical articles: five moves (background information, restating key results, commenting on them, evaluating the study, drawing implications) and their steps, labelled proposition by proposition. It checks that a Discussion interprets, compares and explains its results, states its contribution and limitations, and shows why the study matters beyond itself.

### Claims

From Ken Hyland's interpersonal model of metadiscourse and his work on hedging and stance: where each claim comes from, whether its certainty matches its evidence, why and how much fields hedge, explicit evaluation, self-mention, and the commitment carried by reporting verbs such as *show* and *suggest*. It catches sentences that sound authoritative but have no source, no stated evidence and no writer standing behind them. From Hyland's work on engagement, it also checks how the text addresses the reader: directives that impose on readers or steer their thinking, inclusive *we* that leads them to a conclusion, and "obviously" or "of course" claiming agreement the field may not share.

### Data commentary

From Swales and Feak's account of data commentary: the text that accompanies a figure or table should be a selective, interpretive commentary, not a restatement of the visual. It checks that the commentary locates the visual, highlights the results that bear on the question and says why, accounts for results that do not fit, qualifies its interpretations, and connects its statements into one account. For graphs, it checks that the axes are explained and that the commentary states the pattern or trend rather than reading off values. It also flags data shown twice, and compares the number of figures and tables with the target journal. It does not concern the design of the visual.

### Argument

From Toulmin's model of argument: for each main claim, the data it rests on, the warrant that licenses the step from data to claim, backing for warrants a reader might doubt, a qualifier stating its strength, and the exceptions under which it would not hold. Warrants are usually left unstated; the skill writes them out so the author can see which ones need support. Treating each figure and table as data, it flags visuals that support no claim and main claims whose data are shown nowhere.

### Sentences

From Gopen and Swan's "The Science of Scientific Writing": the seven structural principles for placing information where readers expect it. Whose story a sentence tells belongs in the topic position, the action in the verb, and the new information to be stressed at the end; links between sentences are stated rather than left to the reader. It catches sentences that sound like conclusions but state no relation between specific things.

### Cohesion

From Halliday and Hasan's *Cohesion in English*: personal, demonstrative and comparative reference, and the requirement that every reference item point to something the reader can recover; conjunction (additive, adversative, causal, temporal), checked against the relation that actually holds; lexical cohesion, keeping track of each key object and quantity with the same or a recognizably related word; and substitution and ellipsis, checking that what *do so* or an omitted word stands for can be recovered. It catches pronouns whose referent is missing or does not fit, a *however* with nothing to contradict, and a quantity that changes name halfway through.

### Vague quantities

From Channell's *Vague Language*: the forms vague quantities take (approximators, round numbers, quantifiers such as *many* and *how much*, vague categories) and the jobs vagueness does, from giving the right amount of information to withholding, persuading and covering missing information. It asks for the figure where vagueness withholds or persuades, and leaves approximations alone where they suffice.

### Dense or empty wording

From Halliday's work on grammatical metaphor: congruent and metaphorical wording, nominalization, and the favourite clause type of scientific English, which packs two events and a relation into "A gives B". Unpacking a sentence into congruent wording shows what it says, and whether its participants, processes and relations are there at all.

### Informativeness

From Grice's Cooperative Principle and conversational maxims: each sentence should be as informative as the point requires, true and supported, relevant and clear. It catches truisms and platitudes ("What a simulation can say depends on how real its inputs are"), asks the author what they were meant to imply, and does not replace them with claims the evidence cannot support. Under Grice's maxim of Manner, it also flags loose everyday words standing in for technical properties (inputs that are "real" rather than accurate, uncertain or representative) and lists the candidate terms for the author to choose from.

### Completeness of reporting

Health research only. From the EQUATOR Network's reporting guidelines (CONSORT, STROBE, PRISMA, STARD, SRQR, ARRIVE and others): match the study design to its guideline, then check each item against the draft. A reporting guideline is the minimum a paper must report to be understood, replicated and included in systematic reviews.

### Spin

Health research only. From Boutron and Ravaud's review of misrepresentation in biomedical research: misreported methods ("beautification", switched outcomes), selective or misleading reporting of results, interpretation beyond the results (causal language for observational data, non-significance read as equivalence, extrapolation), and rhetoric ("the first study", "strong evidence"). It checks the abstract's conclusions first, where spin is most common, and raises each instance as a question rather than an accusation.

## Try it

Once installed, ask your agent the way you normally would:

- *"Review the introduction of my paper with the reviewer2 skill."*
- *"Label the moves in this introduction and tell me what's missing."*
- *"My Move 2 is weak. How can I state the gap?"*
- *"Should my introduction announce the main findings? The paper is for a physics journal."*
- *"Review the literature review chapter of my dissertation with the reviewer2 skill."*
- *"My Methods section is for an interdisciplinary journal. Is it too condensed?"*
- *"Does my Methods section report everything CONSORT asks for?"*
- *"Label my Methods subsections by move. Is anything missing or out of order?"*
- *"Does my text around Table 2 say anything the table doesn't?"*
- *"My Results section feels like a Discussion. What should move?"*
- *"Label the moves in my Discussion. Did I state the contribution and the limitations?"*
- *"Check the claims in my Discussion: am I overstating anything?"*
- *"This paragraph is hard to follow. Check whose story each sentence tells and where the action is."*
- *"Unpack the key sentences in my abstract. Do they actually say anything?"*
- *"Are there sentences in my Discussion that just state the obvious?"*
- *"Check my clinical paper's abstract for spin."*
- *"Give my Discussion a quick review."*
- *"Review my whole manuscript, and check that the sections agree with each other."*
- *"Does my abstract actually state the findings?"*
- *"Lay out the argument behind my main conclusion. Which warrants would a reviewer question?"*

## Faithful to its sources

Every rule names its source, and no rule combines authorities. Most rules cite the work and page; an article read in a reprint without page numbers is cited by section; where the primary work was not available, the rule cites it as reported in a named open source, listed in that rules file. Where an authority gives no rule (an introduction's length, the number of citations, a required opening sentence), the skill says so instead of supplying one. The skill keeps the author's claims and citations, and asks for content a rule needs rather than inventing it.

## Planned

- **Research proposals and whole theses:** the moves of a research or grant proposal, and the organization of a thesis across chapters
- **Verification:** check page numbers taken from open texts and secondary sources against the original works, starting with the Methods table in `rules/methods.md`

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
- Cotos, E., Huffman, S., & Link, S. (2015). Furthering and applying move/step constructs: Technology-driven marshalling of Swalesian genre theory for EAP pedagogy. *Journal of English for Academic Purposes*, 19, 52–72.
- EQUATOR Network. Reporting guidelines. https://www.equator-network.org/
- Boutron, I., & Ravaud, P. (2018). Misrepresentation and distortion of research in biomedical literature. *PNAS*, 115(11), 2613–2619.
- Cotos, E., Huffman, S., & Link, S. (2017). A move/step model for methods sections: Demonstrating rigour and credibility. *English for Specific Purposes*, 46, 90–106.
- Hyland, K. (2000). *Disciplinary Discourses: Social Interactions in Academic Writing*. Longman.
- Hyland, K. (2023). Changing times; changing texts. WAC Clearinghouse. https://doi.org/10.37514/PER-B.2023.1800.2.03
- Swales, J. M., & Feak, C. B. (1995). From information transfer to data commentary. *The Journal of TESOL-France*.
- Hyland, K., & Zou, H. (2022). Titles in research articles. *Journal of English for Academic Purposes*, 56, 101094.
- Toulmin, S. (1958). *The Uses of Argument*. Cambridge University Press.

The skill paraphrases these works and cites them; it does not reproduce their text. Read the originals for the full treatment, examples and exercises.

## License

MIT; see [LICENSE](LICENSE).
