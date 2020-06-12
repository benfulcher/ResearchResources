---
layout: post
title: "Open-Pimping Your LaTeX CV"
date: "2020-06-05 17:11:04 +1000"
---

Are you community minded and have been doing lots of open science but also a little career minded and want some recognition?
Well, you're not alone!
I recently had a go presenting a wider variety of (e.g., code and data) contributions to the community in my CV.
<!-- the Open Access symbol to links to publications in a LaTeX CV. -->

It was valuable to go back and see how many of my older publications (and those from collaborations) that have no publicly available versions, and also to watch the trend towards making science more easily reproducible (an ongoing journey).
<!-- While all of my recent publications have at least open access preprints, verifying this and checking which of my past work is accessible was a valuable exercise. -->

### Adding the open-access symbol

It's nice to tag the open access symbol on open publications, and when closed, to have a direct link to an open preprint (e.g., that services like [unpaywall](https://unpaywall.org/) would point people to, who don't have access to a closed version).

You need the [`biblatex-ext`](https://ctan.org/pkg/biblatex-ext) package and the extra functionality of the open access options: `biblatex-ext-oa.sty`.
Actually this looks like a cool way to add these OA stamps automatically to you bibliography using the  API.

It was as simple as adding to the preamble:

```latex
\usepackage{biblatex}
\usepackage[symbolpackage=pict2e]{biblatex-ext-oa}
```

and then you can just use the `\oasymbol` throughout your paper (defaults to the orange PLoS style symbol, but there are other options).

### Adding other symbols

You can also use [fontawesome](https://fontawesome.com/) to mark other outputs such as code posted to Github or datasets.

This is very easy. Adding to the preamble: `\usepackage{fontawesome}`, gives you access to all the symbols.

You can also modify the color of your hyperlinks as `\usepackage[colorlinks=true,urlcolor=cyan]{hyperref}`.

Then you can use commands like

```
\href{https://github.com/benfulcher/Empirical1000_LowDimProj}{Reproducible code \faGithub}
```

You'll see example of how this sort of thing renders:

![Screenshot of open access symbol in CV]({{ site.url }}/{{ site.baseurl }}/assets/OAsymbol_CV.png)

Pretty happy with how it worked out, in giving easy, direct access to my papers for anyone reading my CV, and also pointing them to non-publication outputs such as datasets or code repositories
