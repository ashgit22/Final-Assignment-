Final Assignment SLE 777

Author: Ashith Sujay Kumar
Course: SLE 777
Format: R Markdown (.Rmd)
Output: HTML with Table of Contents (ToC), Cosmo theme

Overview

This report is the final assignment for the SLE 777 course and is structured into two main parts:

Gene Expression and Tree Growth Analysis

Biological Sequence Diversity (Comparative Genomics)

Each section includes detailed data analysis, visualization, and interpretation. The code is written in R and uses publicly available datasets from GitHub and Ensembl.

Part 1: Gene Expression and Tree Growth Analysis
Gene Expression Analysis

Dataset: gene_expression.tsv (sourced from GitHub)

Key Steps:

Loaded gene expression data and calculated mean expression per gene

Identified top 10 most highly expressed genes

Counted genes with low expression (mean < 10)

Visualized expression distribution using histogram (log scale)

Tree Growth Analysis

Dataset: growth_data.csv (tree circumference data, 2005–2020)

Key Steps:

Cleaned dataset and extracted relevant fields (Start, End, Site)

Calculated site-specific summary statistics (mean, SD)

Created boxplots for circumference at start and end

Computed mean 10-year growth per site

Performed a t-test to assess site differences in growth

Part 2: Biological Sequence Diversity
Organisms Analyzed

Escherichia coli (E. coli) — Str. K-12 MG1655

Anaerococcus tetradius

Datasets

Coding sequences (CDS) in FASTA format from Ensembl Bacteria (release 62)

Key Analyses

CDS Statistics

Counted total number of coding sequences

Calculated total coding DNA length per organism

Length Distributions

Compared CDS lengths using boxplots

Calculated mean and median lengths

Amino Acid Frequencies

Translated CDS to protein sequences

Visualized amino acid usage for each organism

Codon Usage

Computed codon frequencies per organism

Compared side-by-side in a grouped barplot

K-mer Analysis

Analyzed over- and under-represented k-mers (k = 3, 4, 5)

Visualized frequency differences in barplots

How to Run This Analysis

Required Libraries:

seqinr

R.utils

knitr

Execution:

Open the .Rmd file in RStudio

Click Knit to produce the HTML report

Ensure internet access for downloading data from GitHub and Ensembl FTP servers

Note: The script downloads and decompresses FASTA files (CDS) and may take a few minutes depending on connection speed.

Interpretation & Key Findings

Gene Expression: Most genes have low expression; only a small number are highly expressed.

Tree Growth: Trees at the Northeast site showed greater growth on average, although the difference is marginally non-significant.

Comparative Genomics:

E. coli has more CDS and a longer total coding length than Anaerococcus tetradius.

Codon and amino acid usage varies between the two species, reflecting different genomic and translational preferences.

K-mer profiles reveal species-specific DNA motifs and potential regulatory patterns.

License

This analysis is intended for academic purposes under the scope of SLE 777 coursework.
