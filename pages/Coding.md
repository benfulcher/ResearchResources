---
layout: page
title: "Coding"
permalink: /Coding/
---

### Writing code
You must use [version control](pages/ReproducibleScience.md).

Full-featured text editors are necessary for efficient coding.
I use [Atom](https://atom.io/) which has some nice features:
* [Hydrogen](https://nteract.gitbooks.io/hydrogen/) and a python kernel for interactively running python code.
* [Markdown previews](https://atom.io/packages/markdown-preview) are essential for writing markdown.
* Natural git and github integration mean that you never need to leave the editor to do your basic git. There are also some nice keyboard shortcuts in [git+](https://atom.io/packages/git-plus).
* [Time machine](https://atom.io/packages/git-time-machine) lets you interactively view the history of each file in your repository.
* The pain of merge conflicts is eased by [this package](https://atom.io/packages/merge-conflicts).

### Cluster computing
* ***ALL*** code on a cluster should be a clone of a git repository on Github.
  You should have another clone on a local computer that you can edit, and keep all versions synchronized through push/pull.
  You never want to have any risk of versions of the same code becoming out of synch.
* You should have a nice interactive way of getting data/outputs to/from the server.
  The best is [Transmit](https://panic.com/transmit/); free alternatives are [Cyberduck](https://cyberduck.io/), or [FileZilla](https://filezilla-project.org/).

## Languages

### Python
Python is a free and flexible coding environment.
It is open source and is used by a large and supportive scientific community.
Being a substantial general coding language, the act of coding in python encourages good practice.

### Matlab
Matlab is great for science, because of the ease of turning data into interactive plots through just a few simple commands.
This allows you to quickly get a deep feel for your data, and the documentation and depth of functionality through toolboxes is excellent.
Unfortunately, it is not open source (you don't know what's happening under the hood) and you have to pay to use it (only those who have paid access can use your code if you share it).
This is a major limitation for science, as it impinges on one's ability to share their work, and can also lead to the strange phenomenon in which you yourself are locked out of running software that you created (e.g., if you leave a University which gave you Matlab access).

### Julia
[Julia](https://github.com/JuliaLang/julia) is an insanely fast high-level programming language.
You can download Julia [here](https://julialang.org/downloads/).

* A good introductory tutorial is [here](https://intersectaustralia.github.io/training/JULIA101/index).
* You can run for free on [JuliaBox](https://www.juliabox.com/).
