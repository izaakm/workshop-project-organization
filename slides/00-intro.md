---
created: 2024-02-10T13:22:12-0500
zuid: 65c7bed4
title: Outline
---

# Project Organization & Data Management

<!-- blank -->


# Plugs

- Office Hours (Tue, 11-12 Zoom and Thu, 1-2 in Min Kao 639)
- UT Bioinformatics Monthly Newsletter<br/>
  <https://tiny.utk.edu/BioinformaticsNewsletter>
- Bioinformatics Computing Support<br/>
  <https://tiny.utk.edu/BCS>

# <!-- SLIDE: FLYER -->

<img src="images/workshop-flyer/flyer-150dpi.jpg" style="border: 1px solid grey" />

<!--
![][img-workshop-flyer]
-->

[img-workshop-flyer]: images/workshop-flyer/flyer-150dpi.jpg


# Motivation

<div style="font-size: 0.8em;">
> The core guiding principle is simple: Someone unfamiliar with your project
> should be able to look at your computer files and understand in detail what
> you did and why.
>
> This “someone” could be any of a variety of people ...
>
> **Most commonly, however, that “someone” is you.** A few months from now, you
> may not remember why you created a particular set of files or conclusions you
> drew. You will then have to either spend time reconstructing your previous
> experiments or lose whatever insights you gained from those experiments.
> (Noble, 2009)
</div>


<!--
- > someone who read your published article and wants to try to reproduce your work
- > a collaborator who wants to understand the details of your experiments
- > a future student working in your lab who wants to extend your work after you have moved on to a new job
- > your research advisor, who may be interested in understanding your work or who may be evaluating your research skills.
-->

# Motivation

<div style="font-size: 0.8em;">
> Ever tried to reproduce an analysis that you did a few months ago (or years)
> ago? You wrote the code, but now you can't remember if you should use
> `make_figures_final.R`, `make_figures_working.R` or `new_make_figures.R`.
> 
> Here are some questions we've learned to ask with a sense of existential
> dread:
> 
> - Are we supposed join the column X to the data before we get started or did
>   that come from one of the notebooks?
> - Which notebook do we have to run first before running the plotting code:
>   was it "process-data" or "clean-data"?
> - Where did the shapefiles get downloaded from for the geographic plots?
> - Etc., times infinity.
</div>

~ Cookiecutter Data Science

# Project Organization & Data Management

## Objectives

- identify day-to-day organizational challenges associated with computational experiments
- suggest strategies for managing computational experiments

## Outcome

- develop a logical, reasonably standardized, but flexible project structure

# Project Organization & Data Management
## Benefits

- A newcomer can begin to understand your project without digging in to extensive documentation.
- A newcomer doesn't have to read 100% of the code to know where to look for specific things.

<!--
> A good example can be found in major web development frameworks like
> Django or Ruby on Rails. Nobody sits around before creating a new Rails
> project to figure out where they want to put their data; they just run `rails
> new` to get a standard project skeleton like everybody else.
>
> Another great example is the Filesystem Hierarchy Standard for Unix-like
> systems. System directories have specific purposes and everybody (more or
> less) agrees to honor that social contract. That means a user knows roughly
> where to look for certain types of files, even when using each another
> person's system.
-->


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


<!-- END -->
