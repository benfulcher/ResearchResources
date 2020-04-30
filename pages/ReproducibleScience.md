---
layout: page
title: "Reproducible science"
permalink: /ReproducibleScience/
categories: material
---

> An article about computational science in a scientific publication is not the scholarship itself, it is merely advertising of the scholarship. The actual scholarship is the complete software development environment and the complete set of instructions which generated the figures.
— David Donaho

## Reproducible coding

### Why is reproducible coding important?

When coding, you’re often changing bits of code incrementally, or producing results that rely on a particular version of code.
Version control, the most popular implementation of which is a system called 'git', is a way of keeping track of changes to a code repository over time.
These repositories can also be uploaded to a server to allow collaboration on code, when working together with other researchers.

### Setting yourself up for reproducible coding

* Make an educational account on [GitHub](github.com), which provides you with unlimited public and private repositories.
* The first time you set up git, you should generate an ssh key to bypass having to type your username and password with every push to GitHub.
Instructions are [here](https://help.github.com/articles/generating-an-ssh-key/).
This means that you should use the ssh (not http) version of the Github repository reference: `git clone git@github.com:BMHLab/TestGitRepository.git`
* Version control is much easier with a graphical interface than in the command-line.
  I recommend the free and excellent [SourceTree](https://www.sourcetreeapp.com).
  An alternative is the [Github Desktop](https://desktop.github.com) application.
* You should also set up integration with a text editor for coding is perhaps the most useful. I recommend [Atom](https://atom.io/).

### Learning git
On a server, such as for a compute cluster, you must run git in the command-line.
* Here is a quick [introduction article](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004668) to version control using Git.
* Some nice tutorials for this have been written by [Atlassian](https://www.atlassian.com/git/).

### Basic tips

* Commit regularly
* Focus on text files, like code, where changes can be stored efficiently.
Avoid binary files (datasets, image files, etc.) that will bloat your repository.

### Workflow

Whenever you start a project that involves coding, be sure to first initialize a repository on Github, clone it to your local machine (as the `ssh` not `https` version), and then regularly commit snapshots of your code.
Whenever you produce an output figure or statistic, you should have a clear way to map back to the state of your code when you produced this (which can be done by committing the code at that point).

* Code to reproduce every analysis and figure in your paper should be easy for others to access and use.

## Sharing data

* [Zenodo](https://zenodo.org/signup/) is my favorite way to upload scientific datasets, providing a citable DOI to your data.
* [figshare](https://figshare.com) is a poorly designed alternative, but also provides a citable DOI to your data.
* Another option is [Dryad](https://datadryad.org/stash).
* To pick the right data repository for your paper, you can use the registry of research data repositories: [re3data](https://www.re3data.org/) or [FAIRsharing](https://fairsharing.org/).
