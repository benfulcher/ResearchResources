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

### General structure

- A general template for structuring a scientific argument is to first explain the problem, then the solution, then the results, then the implications.
Avoid going backwards, e.g., explaining what method was applied and then afterwards explaining why is more confusing than explaining the problem to be solved first and then the method that appropriately solves it.
- Distinguish between the solution and its implementation. When making a scientific argument, it will be for the theory or method to be applied and why it's appropriate. Secondary is the implementation of that theory or method (e.g., the software package or specific numerical scheme used and its version), which can be included in Methods, but clearly separated from the scientific argument made on the basis of theory/methods.

### Style

- Write clearly and without bias or hype, in a neutral tone. It's important to be interesting and compelling, but never at the expense of accuracy.
Read [this](https://elifesciences.org/articles/88654) for elaboration.
- Give clear context and motivation for what you are doing and why.
For example, opening a section with "We first outline X" assumes that the reader knows why X is important and how it relates to the rest of the paper.
- Whenever you write "this" or "these", make sure it's crystal clear to the reader what "it" refers to, and clarify/spell it out if in doubt.

## Some 'house' rules/tips

- Use the Oxford comma.
- Avoid somewhat vague words like 'framework'.
- Use active voice. E.g., instead of "we provide a detailed description of X", it's much clearer to write: "we describe X in detail".

### Figures and Captions

- Shorten "Figure" to "Fig." and "Figures" to "Figs" when not at the start of a sentence.
- Don't put a reference to a figure/table in parentheses unless it's _super obvious_ what the reader is supposed to get from it.
Better practice is to introduce it clearly, and tell the reader what they should expect to see there (in the case of a figure), e.g., "(this concept is illustrated in Fig. 1A)".
- The reader will not look at the figure unless told to—the main text should introduce the figure and all of its panels in the appropriate context of drawing on the evidence shown there to build/support your scientific argument.

- The first line of a caption should (where possible) be a short, descriptive take-away message from the figure (e.g., a scientific claim that the figure supports).
Relative to a neutral, descriptive title, this can be very helpful for the reader to know what the results in the figure are being used as evidence for.
- The rest of the caption should describe what is shown in the figure, and contain enough information to be able to understand the axes and plot elements, etc.
But it is not a place to describe the results or their implications---this is what the main text is for.


### Numbers

- If your measurement is a physical quantity, _always_ accompany it with the physical units it was measured in.
Separate the unit with a small-space `\,` in Latex, e.g., `3\,m`, or using option-space in a text editor.

### Precision

- Phrase ideas precisely, avoiding ambiguity. For example, "we conducted experiments on __various__ simulated dynamical processes" (clearer as "we conducted experiments on three simulated processes: (i) …"). Look out for words like "various" or "around" or "like" of "few" or "small" or "low" or "high" and check whether they could be made more precise.
- Avoid words like "would" or "could" or "can" when talking about what was done.
Instead, use "we did X" or "we applied Y" or "we used Z".
- Think about the number of significant figures that you report your measurements to.
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
