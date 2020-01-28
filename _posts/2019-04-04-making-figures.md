---
layout: post
title: "Making figures"
categories: material
---

### General
* Generate figures algorithmically as much as possible, as clear scripts in an open code repository.
* Know the difference between vector and bitmap graphics, and output your figures appropriately.
* Aesthetic touch-ups can be made after exporting your figure, for vector graphics ([Adobe Illustrator](https://www.adobe.com/products/illustrator.html), [Affinity Designer](https://affinity.serif.com/en-gb/), or the free [Inkscape](https://inkscape.org/)) or bitmap graphics ([Adobe Photoshop](https://www.adobe.com/au/products/photoshop.html), or the free [GIMP](https://www.gimp.org/)).

### Color palettes
You should select the color palette for your figures carefully, being especially wary of common forms of [colorblindness](https://davidmathlogic.com/colorblind/), and giving some thought to how readable figures are in greyscale.
When using a continuous color scale, avoiding the colormap [`jet`](https://jakevdp.github.io/blog/2014/10/16/how-bad-is-your-colormap/) will prevent incurring the wrath of passionate [jet fighters](https://github.com/smsaladi/jetfighter), who will direct you to [automatically 'fix'](https://fixthejet.ecrlife.org/) your colormap.

* Pick from some [classics](http://colorbrewer2.org/).
* Algorithmically [make your own](http://vrl.cs.brown.edu/color).
* Another [algorithmic one](https://medialab.github.io/iwanthue/).
* Another way to [make your own](https://jdherman.github.io/colormap/).

### Plotting distributions
For data exploration, you should always avoid plots that make assumptions about the distribution of values (like those that plot the mean plus/minus standard deviation).
Alternatives include violin plots:

* Violin Plots: [Matlab Code](https://github.com/bastibe/Violinplot-Matlab).
