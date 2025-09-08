
# Workflow for 16S rRNA Gene Amplicon Analysis

This workflow processes raw FASTQ data from the 16S rRNA sequencing experiment (SRR35204195) using a typical pipeline consisting of quality control, denoising, taxonomic classification, and diversity analysis. The steps are executed using tools such as FastQC, DADA2 (via QIIME2), and SILVA database alignment for taxonomy.

The MultiTax reference database and MultiTax-human database are available for download via Google Drive. The download link can be found in the README file of the associated GitHub repository (https://github.com/zwbao/MultiTax-database).

## Workflow Steps

1. **Quality Control**: Assess read quality using FastQC.
2. **Denoising**: Use DADA2 via QIIME2 to denoise reads, remove chimeras, and generate ASVs.
3. **Taxonomic Assignment**: Classify ASVs using SILVA database.
4. **Diversity Analysis**: Calculate alpha and beta diversity metrics using QIIME2.
5. **Visualization**: Create bar plots, ordination plots, and heatmaps.

---
Input: `SRR35204195.fastq` (single-end 16S rRNA read)
