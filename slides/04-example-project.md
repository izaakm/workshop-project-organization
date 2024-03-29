---
title: More project features
---


# Back to the example ...

```text
example
├── AUTHORS
├── README.md
├── data
├── docs
├── results
└── src
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
## ~~Authors~~ CITATION.cff file


```text
example
├── CITATION.cff  *
├── README.md
├── data
├── docs
├── results
└── src
```

# Files
## Citation File Format (CFF)

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
    value: 10.1038/171737a0
date-released: 1953-04-25
```

# Files
## Citation File Format (CFF)

<!--
![](https://docs.github.com/assets/cb-223106/mw-1440/images/help/repository/citation-link.webp)
-->

<img src="https://docs.github.com/assets/cb-223106/mw-1440/images/help/repository/citation-link.webp" class="shadow" style="border: 1px solid lightgrey;" />


# Files
## Register a DOI for software w/ Zenodo

```
$ cat CITATION.cff
```

```text
...
identifiers:
  - type: doi
    value: 10.5281/zenodo.1234  *
...
```

<https://docs.github.com/en/repositories/archiving-a-github-repository/referencing-and-citing-content>

# Exercise
## Create a CITATION.cff file

<!--
<https://citation-file-format.github.io/cff-initializer-javascript/#/>
-->

1. Go to <https://bit.ly/cffinit> and create a CITATION.cff file for your project.

# Files
## Environment file(s)

Reproducibility includes your code *and all of its dependencies*.

<!--
- environments.yml, requirements.txt
- Docker, Singularity, Apptainer
-->

```text
example
├── CITATION.cff
├── README.md
├── environment.yml    *
├── data
├── docs
├── results
└── src
```


# Optional directories

- `bin`          : binaries and scripts\*
    <div class="footnote">
    \* Scripts that are *not* compiled should be in `src` and then be symlinked into `bin`.
    </div>
- `config`       : configuration files with settings e.g., for NextFlow
- `lib`          : for external code
- `logs`         : for messages from your scripts
- `tests`        : scripts to run tests on your code
- `tmp`, `cache` : temporary data directory to use during development



<!-- END -->
