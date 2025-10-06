# Final Assignment SLE 777

**Author:** Ashith Sujay Kumar  
**Course:** SLE 777  
**Output Format:** HTML (via R Markdown)  
**Features:** Table of Contents, Cosmo Theme

---

## Overview

This project is the final assignment for the SLE 777 course. It is divided into two major parts:

1. **Gene Expression and Tree Growth Analysis**
2. **Biological Sequence Diversity (Comparative Genomics)**

Each section performs data analysis, visualization, and interpretation using R and real biological datasets.

---

## Part 1: Gene Expression and Tree Growth Analysis

### Gene Expression

- **Data Source:** `gene_expression.tsv` (from GitHub)
- **Objectives:**
  - Load and inspect gene expression data
  - Calculate mean gene expression across samples
  - Identify top expressed genes
  - Count genes with low expression (<10)
  - Visualize distribution with a histogram

### Tree Growth Analysis

- **Data Source:** `growth_data.csv` (tree circumference data from 2005 and 2020)
- **Objectives:**
  - Clean and process tree data
  - Compare start and end circumferences by site
  - Visualize with boxplots
  - Calculate 10-year growth and perform t-tests between sites

---

## Part 2: Biological Sequence Diversity

### Organisms Compared

- **Escherichia coli (E. coli)** – K-12 MG1655
- **Anaerococcus tetradius**

### Data Sources

- Coding Sequences (CDS) from [Ensembl Bacteria Release 62](https://ftp.ensemblgenomes.ebi.ac.uk/pub/bacteria/release-62/)

### Analyses Performed

- **CDS Count and Total Coding Length**
- **CDS Length Distribution**
  - Boxplots of CDS lengths
  - Mean and median length comparison
- **Amino Acid Frequency**
  - Protein translation of CDS
  - Barplots showing amino acid usage
- **Codon Usage**
  - Frequency calculation and comparison
- **K-mer Analysis**
  - Identification of over- and under-represented DNA motifs (k = 3, 4, 5)

---

##How to Run the Analysis


1. **Open the `.Rmd` file** in RStudio.
2. Click the **Knit** button to generate the HTML output.
3. Ensure **internet access** is available — all datasets are downloaded during runtime.
4. **Output:** An HTML report with embedded results, plots, and interpretation.

---

## Key Insights

### Gene Expression
- Gene expression is **highly skewed** — the majority of genes have low expression.
- A small number of genes show **very high activity**.

### Tree Growth
- Trees in the **Northeast site** showed greater growth on average over 10 years.
- The difference is **marginally non-significant** (*p* ≈ 0.059).

### Genomic Comparisons
- **E. coli** has **more CDS** and a **larger total coding genome** than *Anaerococcus tetradius*.
- **Codon** and **amino acid** usage profiles show **clear species-specific patterns**.
- **K-mer analysis** highlights **distinct sequence motif preferences** between the two organisms.

---

## License

This analysis is submitted as **academic coursework** for **SLE 777**.  
It is intended strictly for **educational purposes**.

