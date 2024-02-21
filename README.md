Project Organization and Data Management
========================================

Based on:

- [Project Organization and Management for Genomics][_d]
- [Cookiecutter Data Science][_g]
- [A Quick Guide to Organizing Computational Biology Projects][_i]


Topics
=======

1. What do you want your project directory to store?
    - Lab protocols
    - Primary data, including images 
    - Lists of specimens and reagents 
    - Information about instruments
    - data
    - code
    - documentation
    - tests
1. Conceptual model of your project
    - Where do things go? ... GTD Archive - Use the most obvious "identifier",
      eg, you should be able to find it by looking in at most 2 places.
1. README
1. Project Directory structure
    - an example project directory
    - talk about the files and directories ...
        - README.md
        - .git
        - data
        - code (src)
        - documentation (docs)
        - tests
1. Data categories
    - metadata (data about the experiment; machine or human generated, immutable)
    - raw data (machine generated, immutable)
    - third-party (human generated, immutable)
    - derived (outputs)
    - data dictionaries
1. Data best practices
    - machine generated vs human generated (eg, Excel spreadsheets)
    - naming conventions: unique identifiers for samples
        - see "making-the-right-moves-second-edition.pdf" p 149 for examples
    - unique identifiers for samples
    - about spreadsheets
1. Example: Genomics Core Sequencing data
1. Example: NCBI SRA Data
1. Example: Something more stats/data-science oriented

Test diagram
============

```mermaid
flowchart LR

A[Hard] -->|Text| B(Round)
B --> C{Decision}
C -->|One| D[Result 1]
C -->|Two| E[Result 2]
```



Attribution
===========

Portions of this workshop are derived from the [Data Carpentries'][_c]
workshop "[Project Organization and Management for Genomics][_d]"
(Copyright (c) The Carpentries) which is made available under the [Creative
Commons Attribution license 4.0][_a].



<!-- LINKS -->

[_a]: https://creativecommons.org/licenses/by/4.0/
[_b]: https://creativecommons.org/licenses/by/4.0/legalcode
[_c]: https://datacarpentry.org/
[_d]: https://datacarpentry.org/organization-genomics
[_e]:
    https://datacarpentry.org/organization-genomics/01-tidiness.html#data-about-the-experiment
    "Data about the experiment [metadata]"
[_f]:
    https://datacarpentry.org/organization-genomics/01-tidiness.html#structuring-data-in-spreadsheets
    "Structuring data in spreadsheets"
[_g]: https://drivendata.github.io/cookiecutter-data-science/
[_h]:
    https://sciencehistory.org/education/scientific-biographies/james-watson-francis-crick-maurice-wilkins-and-rosalind-franklin/
[_i]:
    https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1000424
    "A Quick Guide to Organizing Computational Biology Projects"

<!-- END -->
