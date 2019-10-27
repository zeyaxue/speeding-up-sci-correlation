# speeding-up-sci-correlation
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fgithub.com%2Fzeyaxue%2Fspeeding-up-sci-correlation/master)

## Summary
Visualization codes from the 2nd "speeding up science workshop". This repository contains codes to plot and calculate correlation (linear regression) between metagenomic and metatranscriptomic sequencing results acquired from the same sample.

There is an example of visualizing gene abundances (DNA) compared to their expression levels (RNA) included in the binder. The data are from one Mediterranean site from the TARA Oceans project (https://science.sciencemag.org/content/348/6237/1261359.long). The metagenomics come from sample accession SAMEA2619782, and the metatransciptomics come from SAMEA2619784.

## Quick Start
- Click the jupyter notebook file (Correlation_dna_rna.ipynb) to enter the interactive user interface
- You can either run the notebook with the example or upload new files 

## Example Input
#### 1. A count table containing genes found in both DNA and RNA sequencing results.

|       | Gene               |          DNA |           RNA |
|------:|:-------------------|-------------:|--------------:|
|     0 | TOBG-MED-1076_1101 |    3.57863   |    12.9926    |
|     1 | TOBG-MED-1076_1116 |    0.71486   |     4.03726   |
|     2 | TOBG-MED-1076_1131 |    7.72704   |     5.45492   |
|     3 | TOBG-MED-1076_1151 |    2.85944   |    15.5723    |
|     4 | TOBG-MED-1076_1195 |    8.81305   |    12.3797    |

#### 2. An annotation table. If a gene has "nan" value for KO ID, this means that this gene does not have any match within the KEGG database.

|    | Gene               | KO_ID   |
|---:|:-------------------|:--------|
|  0 | TOBG-MED-1076_1019 | nan     |
|  1 | TOBG-MED-1076_1027 | nan     |
|  2 | TOBG-MED-1076_1028 | K04084  |
|  3 | TOBG-MED-1076_1032 | nan     |
|  4 | TOBG-MED-1076_1038 | K05540  |

#### 3. A KEGG Orthology table. Each KO ID may belong to multiple pathways. Therefore, the user will need to manually curate this table.

|    | KO_ID   | Category1           |
|---:|:--------|:--------------------|
|  0 | K00360  | Nitrogen metabolism |
|  1 | K00362  | Nitrogen metabolism |
|  2 | K00363  | Nitrogen metabolism |
|  3 | K00366  | Nitrogen metabolism |
|  4 | K00367  | Nitrogen metabolism |

## Example Output
The figure below is a static example of the output figure. The actual figure generated by [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fgithub.com%2Fzeyaxue%2Fspeeding-up-sci-correlation/master) is an interactive plot. User can hover over each dot and line to see their annotation.
<img src='https://github.com/zeyaxue/speeding-up-sci-correlation/blob/master/sample_output.svg'>

## Authors
 - Zhengyao "Zeya" Xue, [Github ID](https://github.com/zeyaxue) and [ORCID](https://orcid.org/0000-0002-4930-8212) 
 - Michael D. Lee, [Github ID](https://github.com/AstrobioMike) and [ORCID](https://orcid.org/0000-0001-7750-9145)
 
## Links
Zenodo Binder, doi: LINK_TO_BINDER
Github Binder: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/git/https%3A%2F%2Fgithub.com%2Fzeyaxue%2Fspeeding-up-sci-correlation/master)
Github Repository: https://github.com/speeding-up-science-workshops/speeding-up-sci-correlation
