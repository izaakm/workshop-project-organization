---
title: Example Project
---


# A minimal example

```
example
├── AUTHORS
├── CITATION.cff
├── README.md
├── data
│   ├── anthropogenic
│   ├── derived
│   └── raw
├── docs
├── results
└── src
```

# Files

```
example
├── AUTHORS
├── CITATION.cff
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
## Citation file (including authors)

```
$ cat CITATION.cff
```

```text
cff-version: 1.2.0
message: "If you use this software, please cite it as below."
authors:
  - family-names: Crick
    given-names: James
    orcid: https://orcid.org/0000-0000-0000-0001
  - family-names: Franklin
    given-names: Rosalind
    orcid: https://orcid.org/0000-0000-0000-0002
title: "Example Project"
version: 2.0.4
identifiers:
  - type: doi
    value: 10.5281/zenodo.1234
date-released: 2021-08-11
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
├── results
└── src
```

# Top-level directories
## Data: `data`

- Data is immutable.

# Top-level directories
## Documentation: `docs`

- This is where you keep detailed docs that explain this project.
- Most programming languages have packages for building docs automatically from code.

# Top-level directories
## Results: `results`

- As in the *results* section of your manuscript.
- Tables, plots, figures, etc. that you intend to use in your manuscript and
  presentations.
- Your code/pipeline may save files in this directory, but it should NEVER read
  files from this directory. IE, this is a *terminal* directory with respect to
  your analysis.

# Top-level directories
## Code: `src`

- As in your original *source code* (including scripts) for your analysis.



















































<!-- END -->
