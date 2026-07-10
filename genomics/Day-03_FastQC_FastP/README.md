# Day 03 — FastQC & FastP Quality Control

> **Training Module:** Genomics  
> **Duration:** Day 3  
> **Tools Used:** FastQC, FastP, Ubuntu WSL, Conda

---

# Objective

The objective of this practical was to assess the quality of raw Next Generation Sequencing (NGS) reads using FastQC and improve read quality using FastP before downstream genome assembly and annotation.

---

# Topics Covered

- Introduction to NGS Quality Control
- Understanding FASTQ quality scores
- FastQC quality assessment
- FastP read preprocessing
- Adapter trimming
- Quality filtering
- HTML and JSON report generation

---

# Learning Outcomes

After completing this practical, I was able to:

- Perform quality assessment of raw sequencing reads
- Interpret FastQC reports
- Remove low-quality reads using FastP
- Generate cleaned FASTQ files
- Compare raw and cleaned sequencing data

---

# Why This Practical Matters

Quality control is the first computational step in every sequencing project.

Poor-quality sequencing reads can negatively affect:

- Genome assembly
- Variant calling
- Gene prediction
- Genome annotation
- Biological interpretation

Performing quality control improves the accuracy of downstream analyses.

---

# Practical Workflow

Raw FASTQ Files

↓

FastQC Analysis

↓

Quality Report

↓

FastP Preprocessing

↓

Trimmed FASTQ Files

↓

FastQC (After Trimming)

↓

Improved Quality Report

↓

Ready for Genome Assembly

---

# Repository Navigation

| File | Description |
|------|-------------|
| README.md | Practical overview |
| notes.md | Theory and concepts |
| commands.md | Commands executed |
| workflow.md | Complete workflow |
| common_errors.md | Troubleshooting |
| learning_reflection.md | Personal learning |
| resources.md | Learning resources |
| case_study.md | Real-world application |

---

# Software Used

- Ubuntu (WSL)
- Conda
- FastQC
- FastP

---

# Skills Acquired

- Quality assessment
- Read preprocessing
- Adapter trimming
- FASTQ interpretation
- Bioinformatics workflow understanding

---

# Real-world Applications

- Whole Genome Sequencing
- Metagenomics
- RNA-Seq
- Clinical Genomics
- Microbial Genome Analysis

---

# Folder Structure

```
Day-03_FastQC_FastP/

README.md
commands.md
notes.md
workflow.md
common_errors.md
learning_reflection.md
resources.md
case_study.md

screenshots/
outputs/
figures/
```

---

# Key Takeaways

- FastQC identifies sequencing quality issues.
- FastP improves read quality through trimming and filtering.
- High-quality reads produce better downstream analyses.

---

# Author

**Ankit Raj**

M.Sc. Bioinformatics

Graphic Era University

GitHub: itsemeankit-bioinfo