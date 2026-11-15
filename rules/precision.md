# Precision: Strunk on definite, specific, concrete language

Load this file when the user wants a draft checked for words that are vaguer, more general or more abstract than the point needs: a loose everyday word where a precise term is meant ("how *real* its inputs are"), a general class where a particular case is meant ("*a* simulation"), and noncommittal or padded phrasing. It applies to any part of a research article, thesis, dissertation or proposal.

**Every rule below is Strunk's.** His book is in the public domain and was read in full; rules cite it by rule number. Where he gives no rule, this file says so rather than supplying one. Nothing here is a general writing preference.

## Source and how it is cited

| Short form | Work |
|---|---|
| Strunk 1918 | Strunk, W., Jr. *The Elements of Style*. New York: Harcourt, Brace and Company (copyright 1918, 1919, 1920). Public domain: https://www.gutenberg.org/files/37134/37134-h/37134-h.htm |

Rules cite Strunk's numbered principles of composition (chapter III). Strunk wrote for general composition, not for research papers; where a rule applies his principle to a research text, the file says so.

## How to apply this file

*Procedure, not a rule of Strunk.*

1. **Mark the words that carry each claim:** the nouns naming what is measured or compared, the adjectives and adverbs of degree, and the subjects of the main clauses.
2. **For each, ask whether a more definite, specific or concrete word exists** for what the author means (rule 1).
3. **Mark noncommittal and padded phrasing** (rules 2–3).
4. **Propose changes citing the rule.** Do not choose the technical term yourself where several could be meant; list them and ask the author which.
5. **Run the checklist** at the end.

## Rules

### 1. Prefer the specific to the general, the definite to the vague, the concrete to the abstract

*Source: Strunk 1918, rule 12, "Use definite, specific, concrete language."*

Strunk asks writers to prefer the specific to the general, the definite to the vague and the concrete to the abstract. Specific language holds the reader's attention. Even when writing about general principles, the writer should give particular instances of them. Following Herbert Spencer, he notes that abstract words make the reader stop to supply a concrete image, which costs effort. His example: "A period of unfavorable weather set in" becomes "It rained every day for a week."

- Where a word names a loose property (*real*, *good*, *important*, *significant* used non-statistically), ask the author which definite property is meant, and offer the candidates.
- Where a sentence states a general principle, ask for the particular instance in this study.
- Where the subject is a general class (*a simulation*, *studies*, *models*), ask whether a particular one is meant.

### 2. Make definite assertions; use *not* to deny, not to evade

*Source: Strunk 1918, rule 11, "Put statements in positive form."*

Strunk asks for definite assertions, and warns against tame, colourless, hesitating, noncommittal language. Readers are dissatisfied with being told only what something is not, and *not* should be used for denial or antithesis, never as a means of evasion. His examples: "He was not very often on time" becomes "He usually came late"; "did not remember" becomes "forgot".

- Flag hesitant or evasive phrasing that leaves the reader guessing what is claimed.
- Strunk's rule is about evasion, not about calibrated caution. Where a hedge marks the real limit of the evidence, keep it; `rules/claims.md` covers how strongly claims should be stated.

### 3. Omit needless words

*Source: Strunk 1918, rule 13, "Omit needless words."*

Vigorous writing is concise: a sentence should contain no unnecessary words. This does not require short sentences, only that every word tell. Strunk singles out *the fact that* as an expression to revise out of nearly every sentence. His examples: "the question as to whether" becomes "whether"; "His story is a strange one" becomes "His story is strange."

- Flag words and phrases that add nothing to the claim, and propose the shorter wording.

## Where Strunk gives no rule

Strunk wrote a short guide to general composition in 1918. He does not discuss technical terminology, definitions, units or field conventions, so choosing between precise terms (accuracy, uncertainty, resolution, validity) is the author's decision, which the agent supports by listing the candidates. He sets no limit on sentence length (rule 3). His other rules on paragraphs, voice and emphasis are not used here; emphasis is covered by `rules/sentences.md`. This file adds nothing where Strunk is silent.

## Example

*An illustration of this file's procedure, not Strunk's.* Draft sentence: "What a simulation can say depends on how real its inputs are."

- **Vague property (rule 1):** inputs are not more or less *real*. Ask which definite property is meant: the accuracy of measured inputs, the uncertainty of estimated parameters, the resolution of spatial data, or how representative the boundary conditions are of the case studied.
- **General class (rule 1):** *a simulation* and *its inputs* name no particular model or input. Ask whether the sentence is about the authors' own model, and which inputs.
- **Abstract wording (rule 1):** *what a simulation can say* stands for something concrete: which outputs, or which conclusions drawn from them. Ask which.
- **Revision:** once the author has chosen the property and named the model, inputs and outputs, the sentence can state a particular case, with its evidence (see `rules/claims.md` and `rules/informativeness.md`).

## Validation checklist

- [ ] Loose words for properties were flagged, with candidate precise terms offered (rule 1)
- [ ] General principles were matched with a particular instance from the study, or the author was asked for one (rule 1)
- [ ] General classes used where a particular case is meant were flagged (rule 1)
- [ ] Evasive or hesitant phrasing was flagged, and calibrated hedges were kept (rule 2)
- [ ] Needless words were flagged (rule 3)
- [ ] No technical term was chosen for the author where several could be meant
