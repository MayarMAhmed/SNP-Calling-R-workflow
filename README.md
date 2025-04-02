
## SNP Calling R Workflow

This project provides an R-based workflow for identifying and analyzing Single Nucleotide Polymorphisms (SNPs) in specific human genes using variant data from the 1000 Genomes Project. The focus is on variants within the **TRPV gene family (TRPV1, TRPV2, TRPV3)** and the **BRCA1/2 genes**, which are associated with sensory processing and breast/ovarian cancer risk, respectively.

### Project Goals

- Detect SNPs in selected genes from a VCF file.
- Determine the **genomic location** of each SNP (e.g., coding region, intron, splice site).
- Assess the **functional consequences** of each SNP (e.g., synonymous, missense, frameshift).
- Predict **amino acid changes** caused by non-synonymous mutations.

### Tools & Technologies

- **R v4.0+**
- **Bioconductor packages**: `VariantAnnotation`, `TxDb.Hsapiens.UCSC.hg19.knownGene`
- **Input data**: VCF files from the [1000 Genomes Project](https://www.internationalgenome.org/)
- Custom R scripts to:
  - Extract genomic ranges
  - Locate variants
  - Predict protein-level effects

### Results Summary

- **TRPV Genes**:
  - TRPV1: 51 SNPs (28 non-synonymous)
  - TRPV2: 32 SNPs (18 non-synonymous)
  - TRPV3: 49 SNPs (28 non-synonymous)
- **BRCA Genes**:
  - BRCA1: 97 SNPs (63 non-synonymous)
  - BRCA2: 173 SNPs (90+ protein-impacting)

 Most of the variants were located in **coding regions**, suggesting potential functional impact on protein products, especially for **BRCA1/2**, known to influence cancer susceptibility.

### 📄 Report

See the full report [`BMS 320 Bioinformatics - MA -201700072.pdf`](https://github.com/MayarMAhmed/SNP-Calling-R-workflow/blob/main/BMS%20320%20Bioinformatics%20-%20MA%20-201700072.pdf) for detailed methodology, code snippets, data sources, and evaluation results.
