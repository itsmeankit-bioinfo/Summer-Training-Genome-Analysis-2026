# Day 02 — Genome Sequencing Fundamentals

> **Training Module:** Genomics  
> **Duration:** Day 2  
> **Institution:** Department of Biosciences, Graphic Era University  
> **Training Program:** Summer Training – Genome Analysis 2026

---

# Objective

The objective of this practical was to understand the fundamental concepts of genome sequencing, Next Generation Sequencing (NGS), biological sequence file formats, sequencing quality, and the preprocessing steps required before downstream bioinformatics analysis.

This session provides the theoretical foundation for all subsequent genomics and metagenomics practicals.

---

# Topics Covered

- Introduction to Genomics
- What is a Genome?
- DNA Sequencing
- Next Generation Sequencing (NGS)
- NGS Workflow
- FASTA File Format
- FASTQ File Format
- Phred Quality Scores
- Read Quality Assessment
- Read Preprocessing
- Introduction to FastP

---

# Learning Outcomes

After completing this practical, I was able to:

- Understand the concept of a genome and genome sequencing.
- Differentiate between Sanger Sequencing and Next Generation Sequencing.
- Explain the complete NGS workflow.
- Identify the structure of FASTA and FASTQ files.
- Interpret Phred quality scores.
- Understand why sequencing reads require preprocessing.
- Explain the role of FastP in NGS data analysis.

---

# Why This Practical Matters

Genome sequencing is the foundation of modern bioinformatics.

Every downstream analysis—including genome assembly, genome annotation, comparative genomics, transcriptomics, metagenomics, variant calling, and phylogenetic analysis—begins with sequencing data.

Understanding sequencing technologies and biological sequence file formats is essential for producing reliable, reproducible, and biologically meaningful results.

---

# Practical Workflow

DNA Sample

↓

DNA Sequencing

↓

Raw Sequence Reads

↓

FASTQ Files

↓

Quality Assessment

↓

Read Preprocessing (FastP)

↓

High-Quality Reads

↓

Genome Assembly

↓

Genome Annotation

↓

Biological Interpretation

---

# Repository Navigation

| File | Description |
|------|-------------|
| README.md | Overview of the practical |
| commands.md | Commands executed during the session |
| notes.md | Concepts explained in simple language |
| workflow.md | Complete workflow of genome sequencing |
| common_errors.md | Errors encountered and troubleshooting |
| learning_reflection.md | Personal learning summary |
| software_versions.md | Software and versions used |
| resources.md | Learning resources and references |

---

# Software & Tools

- Ubuntu
- Windows Subsystem for Linux (WSL)
- Miniconda
- Conda
- Python
- FastP

---

# Skills Acquired

- Genome sequencing fundamentals
- NGS workflow understanding
- Biological sequence formats
- Quality score interpretation
- Read preprocessing concepts
- Bioinformatics workflow documentation
- Linux-based computational biology environment

---

# Real-World Applications

The concepts covered in this practical are widely used in:

- Whole Genome Sequencing (WGS)
- Metagenomic Analysis
- Microbial Genome Analysis
- Variant Calling
- Clinical Genomics
- Precision Medicine
- Agricultural Genomics
- Drug Discovery
- Evolutionary Biology

---

# Folder Structure

```text
Day-02_Genome_Sequencing_Fundamentals/

├── README.md
├── commands.md
├── notes.md
├── workflow.md
├── common_errors.md
├── learning_reflection.md
├── software_versions.md
├── resources.md
├── screenshots/
├── outputs/
└── figures/
```

---

# Key Takeaways

- Genome sequencing generates biological sequence data for computational analysis.
- FASTA stores nucleotide or protein sequences.
- FASTQ stores sequences together with quality scores.
- Phred scores indicate sequencing confidence.
- Read preprocessing improves downstream analysis accuracy.
- High-quality sequencing data is essential for reliable bioinformatics results.

---

# Author

**Ankit Raj**

M.Sc. Bioinformatics  
Department of Biosciences  
Graphic Era University

GitHub: https://github.com/itsmeankit-bioinfo

---

> **Note:** This documentation was created as part of my Summer Training in Genome Analysis (2026) to build a reproducible and well-documented bioinformatics portfolio.