# celegans_jb2_demo

The JBrowse 2 biocuration demo used C. elegans data

This is an expanded instance loading several extra datasets including

- 14 C. elegans PacBio assemblies (manually downloaded from NCBI
  https://www.ncbi.nlm.nih.gov/bioproject/PRJNA692613)
- 14 C. elegans PacBio SRA runs (manually downloaded from NCBI and aligned
  against ce11 with minimap2
  https://www.ncbi.nlm.nih.gov/bioproject/PRJNA692613)
- The CGC1 assembly (manually downloaded from NCBI, concatenating entries from
  https://www.ncbi.nlm.nih.gov/nuccore?term=1246391%5BBioProject%5D)
- Minimap2 alignments of the above assemblies vs ce11
- A Cactus multi-way alignment of the 14 PacBio assemblies + ce11 + CGC1
- CaeNDR VCFs and short-read BAM files for C. elegans, 1,600+ samples
  (https://caendr.org/data/data-release/c-elegans/20231213)
- UCSC 26-way and 135-way alignments to other worm species
  https://hgdownload.soe.ucsc.edu/goldenPath/ce11/multiz135way/
  https://hgdownload.soe.ucsc.edu/goldenPath/ce11/multiz26way/
- NCBI RefSeq gene annotations for ce11
- RepeatMasker track

## Live demo

https://jbrowse.org/code/jb2/main/?config=/demos/ce/config.json

## Slides

A short demo of different functions as a slide deck are here

https://docs.google.com/presentation/d/1tPpwIqvQ5USPvLAuEtWmTZWCFVCizjL1BaVpTTYXeoM/edit?usp=sharing

![](img/1.png)
