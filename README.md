# celegans_jb2_demo

This is a JBrowse 2 instance for C. elegans that includes a variety of
'population' data for exploring

## Datasets loaded

### 14 PacBio Assemblies

I downloaded 14 C. elegans PacBio assembly FASTA files from
https://www.ncbi.nlm.nih.gov/bioproject/PRJNA692613 and also downloaded the
PacBio reads from the SRA and manually aligned them to ce11 using minimap2 -x
map-pb. I also got SV calls on these PacBio reads from https://github.com/kyleLesack/sv_analysis_cendr_pacbio

### CGC1 assembly

I manually downloaded the CGC1 assembly
(https://www.biorxiv.org/content/10.1101/2024.12.04.626850v2) from NCBI,
concatenating entries from
https://www.ncbi.nlm.nih.gov/nuccore?term=1246391%5BBioProject%5D to produce a single FASTA file for the assembly

### "Synteny tracks"

I ran Minimap2 alignments of all the above assemblies vs ce11. These can be used
to compare all assemblies to ce11

### Multi-way whole genome alignment

I created a Cactus multi-way alignment of the 14 PacBio assemblies + ce11 + CGC1

### CaeNDR - C. elegans natural diversity resource

I loaded CaeNDR VCFs and short-read BAM files for C. elegans, 1,600+ samples
(https://caendr.org/data/data-release/c-elegans/20231213)

I also manually downloaded all the BAI files to get a coarse level of coverage
across all samples using "indexcov"
(https://pmc.ncbi.nlm.nih.gov/articles/PMC5737511/)

### UCSC datasets

I loaded a number of UCSC datasets for ce11

- UCSC 26-way and 135-way alignments to other worm species
  https://hgdownload.soe.ucsc.edu/goldenPath/ce11/multiz135way/
  https://hgdownload.soe.ucsc.edu/goldenPath/ce11/multiz26way/
- NCBI RefSeq gene annotations for ce11
- RepeatMasker track

### Live demo

https://jbrowse.org/code/jb2/main/?config=/demos/ce/config.json

## Slides

A short demo of different functions as a slide deck are here

https://docs.google.com/presentation/d/1tPpwIqvQ5USPvLAuEtWmTZWCFVCizjL1BaVpTTYXeoM/edit?usp=sharing

![](img/image1.png)

![](img/image2.png)

![](img/image3.png)

![](img/image4.png)

![](img/image5.png)

![](img/image6.png)

![](img/image7.png)

![](img/image8.png)

## Footnote

Created following biocuration tutorial
https://github.com/GMOD/2025-biocuration-tutorial

Thanks to Kyle Lesack for sharing the SV calls and data resource at
https://github.com/kyleLesack/sv_analysis_cendr_pacbio
(https://www.biorxiv.org/content/10.1101/2025.01.07.631790v2)
