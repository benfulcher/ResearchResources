---
layout: page
title: "Reproducible Science"
permalink: /ReproducibleScience/
categories: material
---

Many of us are in science because we want to drive progress.
The goals of driving scientific progress are undoubtedly enhanced by greater sharing, and modern technology gives us the mechanisms to share our science better, and for the computational analyses we do, even precisely share every step.
As the public mostly contributes to an academic scientist's salary with their taxes, you as a scientist might therefore feel a duty to use that money to give back to the community by sharing (and communicating) what you've done as freely (and clearly) as possible.

Unfortunately, sometimes in science we are pulled in one direction that is better for our careers, and another that is better for science.
If the scientific system were better structured, these two goals would be perfectly aligned.
However, practicing open science is one area where it helps both science and your own career.
People value high-quality science, and sharing your science increases its impact:
1. Your work is marked as higher quality if it is reproducible. Quality matters in a scientific literature drowning in quantity.
And a reputation for quality gets you noticed in your field.
2. You drive more attention to your science as people come across your work through the other resources you are freely making available to the world (e.g., data and code).
3. Others may build on your data/code, or use parts of it in their work, putting you a direct chain in aiding the progress of others (this is a great feeling).

If you choose not to share your work, you are simply putting on a show:

> An article about computational science in a scientific publication is not the scholarship itself, it is merely advertising of the scholarship. The actual scholarship is the complete software development environment and the complete set of instructions which generated the figures.
— David Donaho ([reproducibleresearch.net](https://reproducibleresearch.net/))

Academia is special in that it is funded with the ideal goal of being impartial with respect to commercial or other interests.
As such, trust is crucial---if we don't trust each other, then the public should not trust us.
And if the public doesn't trust its scientists (the people who have spent decades training to be impartial, honest, and trustworthy), then, well, humanity is in trouble in a world in which rhetoric beats reason.
The first step is trusting yourself and adopting reproducible science gives you greater trust in what you produce.
  - The mindset of working reproducibly forces you to work to a much higher standard that pushes your science forward.
  - It also allows you to go back to your analyses later down the track and be able to very quickly understand what you did when you want to do something new based on your past work (or direct someone else to).

## Reproducible Coding

When coding, you’re often changing bits of code incrementally, or producing results that rely on a particular version of code.
Version control, the most popular implementation of which is a system called 'git', is a way of keeping track of changes to a code repository over time.
These repositories can also be uploaded to a server to allow collaboration on code, when working together with other researchers.

### Using version control


#### Graphical Interface

Version control is much easier with a graphical interface than in the command-line.
This is the place to start--you can do everything you need, and visually see the whole history of your code base.

* I recommend the free and excellent [SourceTree](https://www.sourcetreeapp.com).
* An alternative is [Github Desktop](https://desktop.github.com).

#### Command-line git

On a server, such as for a compute cluster, you must run git in the command-line.
* Here is a quick [introduction article](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004668) to version control using Git.
* Some nice tutorials for this have been written by [Atlassian](https://www.atlassian.com/git/).

Basics:
* Commit regularly
* Focus on text files, like code, where changes can be stored efficiently.
   Avoid binary files (datasets, image files, etc.) that will bloat your repository.
   (Use the `.gitignore` file).

### Github

If you're up and using git locally, [GitHub :octocat:](github.com) is a free (for education) service that allows you to host your code.
Then you can share what you've done so others can help you develop it through collaboration, or can exactly reproduce the steps of your analysis as outlined in your code.

1. Make an [educational account](https://education.github.com/benefits) on GitHub, which provides you with unlimited public and private repositories.
2. The first time you set up git, you should generate an ssh key to bypass having to type your username and password with every push to GitHub.
Instructions are [here](https://help.github.com/articles/generating-an-ssh-key/).
This means that you should use the ssh (not http) version of the Github repository reference: `git clone git@github.com:benfulcher/TestGitRepository.git`
* You should also set up integration with a text editor for coding is perhaps the most useful.
  I recommend [Atom](https://atom.io/); [Microsoft VS Code](https://code.visualstudio.com/) is a popular alternative.

#### Workflow

Whenever you start a project that involves coding, be sure to first initialize a repository on Github, clone it to your local machine (as the `ssh` not `https` version), and then regularly commit snapshots of your code.

Whenever you produce an output figure or statistic, you should have a clear way to map back to the state of your code when you produced this (which can be done by committing the code at that point).

Code to reproduce every analysis and figure in your paper should be easy for others to access and use.
A good way to do this is to describe all your analyses in a markdown file, like the online-rendered `README.md` file, where you work through the exact steps to reproduce every analysis in your paper, and embed the outputs.

## Sharing data

* [Zenodo](https://zenodo.org/signup/) is a good way to upload scientific datasets, providing a citable DOI to your data.
* [figshare](https://figshare.com) is a poorly designed alternative, but also provides a citable DOI to your data.
* Another option is [Dryad](https://datadryad.org/stash).
* To pick the right data repository for your paper, you can use the registry of research data repositories: [re3data](https://www.re3data.org/) or [FAIRsharing](https://fairsharing.org/).
