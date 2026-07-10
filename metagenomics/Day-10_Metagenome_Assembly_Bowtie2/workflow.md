# Workflow

## Metagenome Assembly and Alignment Workflow

Raw Metagenomic Reads

↓

FastQC

↓

FastP

↓

Trimmed Reads

↓

SPAdes (--meta)

or

↓

MEGAHIT

↓

Assembled Contigs

↓

Build Bowtie2 Index

↓

Read Alignment

↓

SAM File

↓

BAM Conversion

↓

Sorting & Indexing

↓

Genome Binning

---

# SPAdes Workflow

Trimmed Reads

↓

Error Correction

↓

Assembly Graph

↓

Contigs

---

# MEGAHIT Workflow

Trimmed Reads

↓

k-mer Graph

↓

Assembly

↓

final.contigs.fa

---

# Bowtie2 Workflow

Reference Assembly

↓

Build Index

↓

Read Alignment

↓

SAM File

↓

Downstream Analysis