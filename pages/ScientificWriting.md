---
layout: page
title: "Scientific Writing"

---

### Writing well

Writing a good abstract is crucial---the vast majority of people are time-strapped and, if they get past your title, this is as much as they will read of your work.
So writing a clear statement of what you have done and how it impacts key open questions in a widely accessible way, is super important.

#### Structuring a paper

- [This article](https://doi.org/10.1371/journal.pcbi.1005619), provides a strong foundation for structuring a paper across 10 Simple Rules.

#### Writing an abstract

- [This Nature template](https://www.nature.com/documents/nature-summary-paragraph.pdf) for how to structure an abstract is very informative.

#### Writing a grant

- A nice list of tips in [this twitter thread](https://twitter.com/RohacsTibor/status/1468678482897084426?s=20).

#### Making LaTeX tables

You can more easily make tables in LaTeX using this [online editor](https://www.tablesgenerator.com/).

### Publishing

You can find suitable journals for your work using the [JournalFinder App](https://journalfinder.researcher-app.com/).

### General structure

- A general template for structuring a scientific argument is to first explain the problem, then the solution, then the results, then the implications.
Avoid going backwards, e.g., explaining what method was applied and then afterwards explaining why is more confusing than explaining the problem to be solved first and then the method that appropriately solves it.
- Distinguish between the solution and its implementation. When making a scientific argument, it will be for the theory or method to be applied and why it's appropriate. Secondary is the implementation of that theory or method (e.g., the software package or specific numerical scheme used and its version), which can be included in Methods, but clearly separated from the scientific argument made on the basis of theory/methods.

### Style

- Write clearly and without bias or hype, in a neutral tone. It's important to be interesting and compelling, but never at the expense of accuracy.
Read [this](https://elifesciences.org/articles/88654) for elaboration.

## Some 'house' rules/tips

- Use the Oxford comma.
- Don't put a reference to a figure/table in parentheses unless it's _super obvious_ what the reader is supposed to get from it. Better practice is to introduce it clearly, and tell the reader what they should expect to see there (in the case of a figure), e.g., "(this concept is illustrated in Fig. 1A)".
- Shorten "Figure" to "Fig." and "Figures" to "Figs" when not at the start of a sentence.

### Numbers

- If your measurement is a physical quantity, _always_ accompany it with the physical units it was measured in.
Separate the unit with a small-space `\,` in Latex, e.g., `3\,m`, or using option-space in a text editor.

### Precision

Think about the number of significant figures that you report your measurements to.
Do not specify a quantity to greater precision than the order of magnitude of error in the measurement of that quantity.

- If you have an error associated with a measurement, (3.421 +/- 0.5), this tells you explicitly where the precision of the measurement is irrelevant: 3.4 +/- 0.5.
- _p_-values should be reported to one significant figure (e.g., 0.04, not 0.037621). Ain't no one be caring about further precision.

### Equations

- Each variable should be clearly defined with a single symbol.
Don't use multiple symbols to define a single variable, like TN, for example, as it can be considered as the variable T multiplied by the variable N.
When using text in an equation, use `\mathrm{}` or `\text{}` to ensure it is typeset correctly, e.g., `a_\mathrm{max}` or `a_\text{max}`, not `a_{max}`.


## Text

- Don't use ampersands unless desperate for space (e.g., in tables).
- Semicolons can be used to separate list items when each item is long (and may itself contain a comma).

### Abbreviations

- Write as "e.g.," and "i.e.," (with commas) not "eg" and "ie" (without commas).
The abbreviation "cf." is used to mean "compare" and is not followed by a comma.
- When using an N-dash, do _not_ use a space either side of it, e.g., "the results---which were surprising---were published in Nature", but _do_ use a space either side of an M-dash, e.g., "the results -- which were surprising -- were published in Nature".
- Don't hyphenate after an adverb ending in -ly, e.g., "a highly significant result" not "a highly-significant result".

### Citations

- Use a consistent cite key format with the BetterBibTeX package for Zotero.
I recommend `auth+year+":"+shorttitle(3,3)`.
- Use `\citet{}` when embedding a reference in the sentence (e.g., "Following `\citet{}`, we decided to…").
