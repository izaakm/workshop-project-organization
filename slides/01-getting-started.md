---
created: 2024-02-10T13:43:19-0500
title: Getting Started
---

# Getting Started

<!-- THIS SLIDE BLANK -->

# Getting Started
## What do you need to track?

- Data (raw, processed, etc)
- Scripts
- Lab protocols
- Lists of samples, reagents 
- Information about instruments
- ...


# Getting Started

Start with a flowchart or conceptual model.

Start from [an example online][metagenomics] ...

<img src="https://astrobiomike.github.io/images/metagenomics_overview.png" style="max-height: 10em; border: 1px solid black;" />

... But it doesn't have to be that complicated!

<!--
<a href="https://astrobiomike.github.io/genomics/">
<img src="https://astrobiomike.github.io/images/metagenomics_overview.png" style="max-height: 10em; border: 1px solid black;" />
</a>
-->

<div class="footnote">
<https://astrobiomike.github.io/genomics/>
</div>

[metagenomics]: https://astrobiomike.github.io/genomics/

# Getting Started
## Principles

- Data is immutable
- Document your project (README)
- Use version control, eg, Git
    - but *not* for data
- Notebooks (Jupyter, R markdown) are for exploration and communication
- Reproducibility includes your code and all of its dependencies

<!--
- Machine and human readable
-->

# Exercise
## Draw your conceptual model

- What are your data sources?
- What are the 'preprocessing' steps?
- What are the main software programs you anticipate using?
- Does your project require complex custom code?

<!--
# Exercise
## Conceptual model -- Example

```mermaid
%%| caption: "Start Stop"
%%| alt: "A flow chart representing the Start Stop workflow"
%%| name: "start-stop"
%%{init: {'theme': 'forest', "flowchart" : { "curve" : "basis" } } }%%

flowchart TD
    Start - -> Stop
```
-->

# Exercise
## Conceptual model -- Example

<img src="images/example-workflow.png" />

<!--
https://hbctraining.github.io/rnaseq-cb321/lessons/analysis_methods.html
-->

# *Let's get started ...*

<!-- END -->
