---
title: Example Project
---


# Back to the example ...

```text
example
├── AUTHORS
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

<https://citation-file-format.github.io/cff-initializer-javascript/#/>


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
    value: 10.5281/zenodo.1234
date-released: 2021-08-11
```

# Files
## Citation File Format (CFF)

<!--
![](https://docs.github.com/assets/cb-223106/mw-1440/images/help/repository/citation-link.webp)
-->

<img src="https://docs.github.com/assets/cb-223106/mw-1440/images/help/repository/citation-link.webp" class="shadow" style="border: 1px solid lightgrey;" />


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
├── environment.yml
├── data
│   ├── anthropogenic
│   ├── derived
│   └── raw
├── docs
├── results
└── src
```


# Optional directories

- `cache`, `tmp` : kind of like `derived` but emphasis on short-term storage
- `config`       : for, e.g., NextFlow
- `lib`          : for external code
- `logs`         : for messages from your scripts
- `test`         : test your code
- `bin`          : binaries and scripts\*
    <div class="footnote">
    \* Scripts that are *not* compiled should be in `src` and then be symlinked into `bin`.
    </div>


# Exercise
## Create a CITATION.cff file

<https://citation-file-format.github.io/cff-initializer-javascript/#/>



<!-- END -->
