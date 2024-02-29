---
title: Example Project
---

# A "standard" project template

![](https://imgs.xkcd.com/comics/standards.png)

# A minimal example

```
example
├── AUTHORS
├── README.md
├── data
├── docs
├── notebooks
├── results
└── src
```

# Files

```
...
├── AUTHORS
├── README.md
...
```

# Files
## Authors file

```
$ cat AUTHORS
```

```text
Crick, Francis
Franklin, Rosalind
Watson, James
Wilkins, Maurice
```

# Files
## README(.md) file

```
$ cat README.md
```

```text
# Example Project

This is the description of my example project.
```

# Exercise

1. Create a new directory for your project
1. Create a `README.md` file with the working title and brief description of your project
1. Create an `AUTHORS` file and list the authors for the project
1. Optional: Initialize your project directory as a Git repository

# Top-level directories

```
...
├── data
├── docs
├── notebooks
├── results
└── src
```

# Top-level directories
## `data`

- Data is immutable.
- Data is *not* tracked with version control

# Top-level directories
## `docs`

Your lab notebook

> ... to make the results more understandable, significant effort may need to
> go into the prose descriptions of experiments in the lab notebook, rather
> than simply including a figure or table with a few lines of text summarizing
> the major conclusion. (Noble, 2009)

# Top-level directories
## `docs`

Your lab notebook

- Detailed documentation that explain this project.
- Most programming languages have packages for building docs automatically from
  code.
- For small projects, all documentation might reasonably fit into the main
  `README` file.
- aka: `doc`, `documentation`

# Top-level directories
## `notebooks`

Notebooks (Jupyter, R markdown) are for exploration and communication.

- Extras, nice-to-haves; your analysis shouldn't depend on these.
- Notebooks are *not* tracked with version control.
- aka `reports`

<!-- [TODO] Does it make sense to think of this as a 'lab notebook'? -->

# Top-level directories
## `results`

- As in the *results* section of your manuscript.
- Tables, plots, figures, etc. that you intend to use in your manuscript and
  presentations.
- Your code/pipeline may save files in this directory, but it should NEVER read
  files from this directory. IE, this is a *terminal* directory with respect to
  your analysis.
- aka `reports`

# Top-level directories
## `src`

- As in your original *source code* (including scripts) for your analysis.
- This is *human readable* code (ie, not compiled).
- aka `scripts`, `R`

# Exercise

1. Create the top-level directories for your project, e.g.:

    ```
    ...
    ├── data
    ├── docs
    ├── notebooks
    ├── results
    └── src
    ```

1. Add a description of each directory to your README file.


# Data Sub-directories

- Data is immutable.
- Data is *not* tracked with version control

```
data/
├── anthro
├── derived
└── raw
```

<!--
- `data/raw` : data came from a machine
- `data/anthro` : data came from a person ("anthropogenic")
    - aka `data/third-party`, `data/external`
- `data/derived` or just `derived` : data was produced by your scripts/pipeline
    - aka `outputs`, `data/interim`, `data/processed`
    - subdirectories might be, eg, `data/derived/counts`, etc.
-->

# Data Sub-directories

| Sub-directory | aka                               | Where it came from              |
| :-            | :-                                | :---                            |
| `raw`         |                                   | from a machine                  |
| `derived`     | `outputs`, `interim`, `processed` | from your scripts/pipeline      |
| `anthro`      | `third-party`, `external`         | from a person ("anthropogenic") |


# Data (Sub)Sub-directories

Logical naming examples:

- `raw/sequences`, `raw/IlluminaNovaSeq`, `raw/survey-responses`
- `derived/counts`, `derived/read-counts`
- `anthro/milleri`

<!--
*Keep it simple (and obvious).*
-->

> *There should be one--and preferably only one--obvious <!--way to do it--> place to find it.*
> 
> \~ Adapted from *The Zen of Python*


# Data (Sub)Sub-directories

> the logical structure of your final set of experiments may look drastically
> different from the form you initially designed. This is particularly true
> under the results directory, where you may not even know in advance what
> kinds of experiments you will need to perform. <mark>If you try to give your
> directories logical names, you may end up with a very long list of
> directories with names that, six months from now, you no longer know how to
> interpret.</mark> (Noble, 2009)

# Data (Sub)Sub-directories

Sequential naming

- alpha/numeric: `01`, `010`, `a`
- datetime: `YYYY-MM-DD`, `YYYY-MM-DD-HHMMSS`
- Unix timestamp: `1234567890`

# Data (Sub)Sub-directories

Sequential naming

alpha/numeric: `01`, `010`, `a`

- `pipeline/001`<br/>
  `pipeline/002`

Optionally include a brief (1-3 words) description as a suffix

- `pipeline/001-fastqc`<br/>
  `pipeline/002-multiqc`

# Data (Sub)Sub-directories

Sequential naming

datetime: `YYYY-MM-DD`, `YYYY-MM-DD-HHMMSS`

- `raw/survey-responses/2024-03-01`
- `anthro/milleri/2024-03-01`

# Data (Sub)Sub-directories

Sequential naming

Unix timestamp: `1234567890`

- `pipeline/1709214775`<br/>
  `pipeline/1709214779`
- `tmp/differential-expression/1709214775`<br/>
  `tmp/differential-expression/1709214779`

# Adding 'empty' directories to a Git repo

Git only tracks *files*. A common convention is to create empty files named
`.gitkeep` in standard directories.

# Exercise

1. Create subdirectories for your data based on your conceptual model.
1. Optional: Add these directories to your Git repository.

<!--
1. Create placeholder scripts for your analysis pipeline.
-->

<!--
.
├── data
│   ├── derived
│   │   ├── counts
│   │   ├── deseq2
│   │   └── qc
│   └── raw
│       └── reads
│           ├── Sample00_R1.fastq.gz
│           ├── Sample00_R2.fastq.gz
│           ├── Sample01_R1.fastq.gz
│           ├── Sample01_R2.fastq.gz
│           ├── Sample02_R1.fastq.gz
│           ├── Sample02_R2.fastq.gz
│           ├── Sample03_R1.fastq.gz
│           └── Sample03_R2.fastq.gz
└── src
    ├── 010-qc.sh
    ├── 020-quant.sh
    ├── 030-qc.sh
    ├── 040-diff-expr.R
    ├── 050-make-plots.R
    └── runall.sh
-->


# Exercise

You receive an Excel file via email from a collaborator.
You want to generate summary statistics for the data in this file.

How should you handle this Excel file?

1. Which directory should you put it in?
1. How do you generate summary statistics?

<!-- END -->
