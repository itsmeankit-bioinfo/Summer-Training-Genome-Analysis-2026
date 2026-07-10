# Day 10 — Metagenome Assembly, Bowtie2 Alignment & SAM/BAM File Formats

> **Training Module:** Metagenomics
> **Duration:** Day 10
> **Tools Used:** SPAdes (--meta), MEGAHIT, Bowtie2

---

# Objective

The objective of this practical was to assemble metagenomic sequencing reads using SPAdes and MEGAHIT, understand sequence alignment using Bowtie2, and learn the structure and purpose of SAM and BAM files generated during read mapping.

---

# Topics Covered

- Metagenome Assembly
- SPAdes (--meta)
- MEGAHIT
- SAM File
- BAM File
- BAM Index (BAI)
- CIGAR String
- Bowtie2
- Reference Index Building
- Read Mapping

---

# Learning Outcomes

After completing this practical, I was able to:

- Perform metagenome assembly using SPAdes.
- Assemble metagenomic reads using MEGAHIT.
- Understand the structure of SAM and BAM files.
- Build Bowtie2 reference indexes.
- Align sequencing reads to assembled contigs.

---

# Why This Practical Matters

Metagenome assembly reconstructs longer DNA fragments from mixed microbial communities.

Read alignment allows sequencing reads to be mapped back to assembled contigs, enabling downstream analyses such as coverage estimation and genome binning.

---

# Practical Workflow

Trimmed Reads

↓

SPAdes (--meta)

↓

MEGAHIT

↓

Assembly

↓

Bowtie2 Index

↓

Read Mapping

↓

SAM File

↓

BAM File

↓

Genome Binning

---

# Software Used

- Ubuntu (WSL)
- Conda
- SPAdes
- MEGAHIT
- Bowtie2

---

# Skills Acquired

- Metagenome Assembly
- Sequence Alignment
- Read Mapping
- Understanding Alignment File Formats

---

# Real-world Applications

- Environmental Metagenomics
- Human Microbiome Studies
- Marine Metagenomics
- Genome Binning
- Comparative Metagenomics

---

# Key Takeaways

- SPAdes and MEGAHIT assemble metagenomic reads.
- Bowtie2 aligns sequencing reads to reference sequences.
- SAM and BAM files store alignment information.
- Alignment data are required for downstream analyses such as binning.

---

# Author

**Ankit Raj**

M.Sc. Bioinformatics

Graphic Era University