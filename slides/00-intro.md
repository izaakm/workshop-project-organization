---
created: 2024-02-10T13:22:12-0500
zuid: 65c7bed4
title: Outline
---

# Outline

1. What should you keep in your project directory?
1. Project Directory structure (example)
1. README files and markdown
1. Git
1. data directory
1. src directory
1. docs directory
1. Exercise: conceptual model of your project, data flow
1. Exercise: clean up a spreasheet
1. Exercise: create a project directory
1. Exercise: create a script to automate setup
1. Exercise: create a project template on github
1. Cookiecutter

# Benefits

- Start with a logical structure and then stick to it.
- A newcomer can begin to understand an analysis without digging in to extensive documentation.
- A newcomer doesn't have to read 100% of the code to know where to find specific things.

# Benefits

> A good example can be found in major web development frameworks like
> Django or Ruby on Rails. Nobody sits around before creating a new Rails
> project to figure out where they want to put their data; they just run `rails
> new` to get a standard project skeleton like everybody else.

> Another great example is the Filesystem Hierarchy Standard for Unix-like
> systems. System directories have specific purposes and everybody (more or
> less) agrees to honor that social contract. That means a user knows roughly
> where to look for certain types of files, even when using each another
> person's system.

# Benefits

Ever tried to reproduce an analysis that you did a few months ago or even a few
years ago?

You wrote the code, but now you can't remember if you should use
`make_figures_final.py`, `make_figures_working.py` or `new_make_figures.py`.

Here are some questions we've learned to ask with a sense of existential dread:

- Are we supposed to go in and join the column X to the data before we get
  started or did that come from one of the notebooks?
- Come to think of it, which notebook do we have to run first before running
  the plotting code: was it "process data" or "clean data"?
- Where did the shapefiles get downloaded from for the geographic plots?
- Et cetera, times infinity.

# Principles

> The core guiding principle is simple: Someone unfamiliar with your project
> should be able to look at your computer files and understand in detail what
> you did and why. (Noble, 2009)

# Principles

> This “someone” could be any of a variety of people:

- > someone who read your published article and wants to try to reproduce your work
- > a collaborator who wants to understand the details of your experiments
- > a future student working in your lab who wants to extend your work after you have moved on to a new job
- > your research advisor, who may be interested in understanding your work or who may be evaluating your research skills.

(Noble, 2009)


# Principles

> This “someone” could be any of a variety of people:

- > **Most commonly, however, that “someone” is you.** A few months from now, you may not remember what you were up to when you created a particular set of files, or you may not remember what conclusions you drew. You will either have to then spend time reconstructing your previous experiments or lose whatever insights you gained from those experiments.

(Noble, 2009)


# Principles

- Start with a flowchart or conceptual model
    - Start from an example online ...

        <img src="https://astrobiomike.github.io/images/metagenomics_overview.png" style="max-height: 10em; border: 1px solid black;" />

        ... But it doesn't have to be that complicated!

# Principles

- Documentation (README)
- Use version control, eg, Git
- Be obvious
- Be explicit
- Data is immutable
- Notebooks (Jupyter, R markdown) are for exploration and communication
- Reproducibility includes your code and all of its dependencies

<!--
- Machine and human readable
-->


<!-- END -->
