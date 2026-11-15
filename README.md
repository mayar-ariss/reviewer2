# swales

**An agent skill for writing and revising research paper introductions and literature reviews, from the work of John M. Swales: his Create-a-Research-Space (CARS) model, and Feak and Swales's guidance on literature reviews. Every rule cites Swales by work and page.**

```bash
npx skills add mayar-ariss/swales
```

Works with Claude Code, Cursor, Codex, GitHub Copilot, Gemini CLI and any agent the [skills CLI](https://skills.sh) supports.

## What it does

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

**Literature reviews** (`rules/literature-review.md`, from Feak and Swales's *Telling a Research Story*): why the review is there and how it leads to your research, imposing order on the literature, describing selection criteria, metadiscourse, integral and non-integral citations, citation tense, reporting verbs and ambiguous citations, taking a stance, and paraphrasing and summarizing in your own words.

## Try it

Once installed, ask your agent the way you normally would:

- *"Review the introduction of my paper with the swales skill."*
- *"Label the moves in this introduction and tell me what's missing."*
- *"My Move 2 is weak. How can I state the gap?"*
- *"Should my introduction announce the main findings? The paper is for a physics journal."*
- *"Review the literature review chapter of my dissertation with the swales skill."*

## Faithful to Swales

Every rule names its source by work and page. Where Swales gives no rule (an introduction's length, the number of citations, a required opening sentence), the skill says so instead of supplying one. The skill keeps the author's claims and citations, and asks for content a move needs rather than inventing it.

## Based on

- Swales, J. M. (1990). *Genre Analysis: English in Academic and Research Settings*. Cambridge University Press.
- Swales, J. M. (2004). *Research Genres: Explorations and Applications*. Cambridge University Press.
- Swales, J. M., & Feak, C. B. (1994; 3rd ed. 2012). *Academic Writing for Graduate Students: Essential Tasks and Skills*. University of Michigan Press.
- Feak, C. B., & Swales, J. M. (2009). *Telling a Research Story: Writing a Literature Review*. University of Michigan Press.
- Feak, C. B., & Swales, J. M. (2011). *Creating Contexts: Writing Introductions across Genres*. University of Michigan Press.

The skill paraphrases these works and cites them; it does not reproduce their text. Read the books for the full treatment, examples and exercises.

## License

MIT; see [LICENSE](LICENSE).
