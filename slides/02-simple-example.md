---
title: Example Project
---


# A minimal example

```
example
├── AUTHORS
├── README.md
├── data
│   ├── anthropogenic
│   ├── derived
│   └── raw
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

## Setup/Installation

1. Clone this repo:
    ```
    $ git clone https://github.com/GITHUB_USERNAME/example-project.git
    ```
2. Then `cd` and `pip install`:
    ```
    $ cd example-project
    $ pip install .
    ```
```

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
## Data: `data`

Data is immutable.

- Data is *not* tracked with version control
- `data/raw` : data came from a machine
- `data/anthro` : data came from a person ("anthropogenic")
    - aka `data/third-party`, `data/external`
- `data/derived` or just `derived` : data was produced by your scripts/pipeline
    - aka `outputs`, `data/interim`, `data/processed`
    - subdirectories might be, eg, `data/derived/counts`, etc.

# Top-level directories
## Documentation: `doc(s)` or `documentation`

> ... to make the results more understandable, significant effort may need to
> go into the prose descriptions of experiments in the lab notebook, rather
> than simply including a figure or table with a few lines of text summarizing
> the major conclusion. (Noble, 2009)

# Top-level directories
## Documentation: `doc(s)` or `documentation`

- This is where you keep detailed docs that explain this project.
- Most programming languages have packages for building docs automatically from
  code.
- Maybe unnecessary depending on the scale of the projet. E.g., all
  documentation might reasonably fit into the main `README`.

# Top-level directories
## Notebooks: `notebooks`

Notebooks (Jupyter, R markdown) are for exploration and communication.

- Extras, nice-to-haves; your analysis shouldn't depend on these.
- Notebooks are *not* tracked with version control.
- aka `reports`

<!-- [TODO] Does it make sense to think of this as a 'lab notebook'? -->

# Top-level directories
## Results: `results`

- As in the *results* section of your manuscript.
- Tables, plots, figures, etc. that you intend to use in your manuscript and
  presentations.
- Your code/pipeline may save files in this directory, but it should NEVER read
  files from this directory. IE, this is a *terminal* directory with respect to
  your analysis.
- aka `reports`

# Top-level directories
## Code: `src`

- As in your original *source code* (including scripts) for your analysis.
- This is *human readable* code (ie, not compiled).
- aka `scripts`, `R`

# Exercise

You create a new Excel file (workbook) starting from one of your existing data files. You add a new tab to the workbook and calculate summary statistics.

<!-- Same slide: use H2 to emphasize the question. -->

## How should you handle this Excel file?<br/>Which directory should you put it in?


# Naming files and directories
## Logical naming

> the logical structure of your final set of experiments may look drastically
> different from the form you initially designed. This is particularly true
> under the results directory, where you may not even know in advance what
> kinds of experiments you will need to perform. <mark>If you try to give your
> directories logical names, you may end up with a very long list of
> directories with names that, six months from now, you no longer know how to
> interpret.</mark> (Noble, 2009)

# Naming files and directories
## Logical naming

*Keep it simple (and obvious).*

- `sequences`
- `counts` or `read-counts`
- `survey-responses`

# Naming files and directories
## Sequential naming

- datetime: `YYYY-MM-DD`, `YYYY-MM-DD-HHMMSS`
- Unix timestamp: `ddddddddd`
- alphanumeric: `001`, `a`

Optionally include a brief (1-3 words) description as a suffix.


<!-- END -->
