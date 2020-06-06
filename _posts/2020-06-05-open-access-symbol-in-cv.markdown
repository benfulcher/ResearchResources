---
layout: post
title: "Adding Open Access Symbols to a LaTeX CV"
date: "2020-06-05 17:11:04 +1000"
---

Had a go at adding the Open Access symbol to links to publications in a LaTeX CV.
While all of my recent publications have at least open access preprints, verifying this and checking which of my past work is accessible was a valuable exercise.

You need the [`biblatex-ext`](https://ctan.org/pkg/biblatex-ext) package and the extra functionality of the open access options: `biblatex-ext-oa.sty`.
Actually this looks like a cool way to add these OA stamps automatically to you bibliography using the [unpaywall](https://unpaywall.org/) API.

But for a CV I just wanted to be able to tag the open access symbol.
It was as simple as adding to the preamble:

```latex
\usepackage{biblatex}
\usepackage[symbolpackage=pict2e]{biblatex-ext-oa}
```

and then you can just use the `\oasymbol` throughout your paper (defaults to the orange PLoS style symbol, but there are other options).

Pretty happy with how it worked out, in giving easy, direct access to my work for anyone reading my CV:

![Screenshot of open access symbol in CV]({{ site.url }}/assets/OAsymbol_CV.png)
