# Notes

# What is Metagenomics?

Metagenomics is the study of the collective genetic material obtained directly from environmental samples without isolating or culturing microorganisms.

Unlike traditional microbiology, metagenomics enables researchers to analyze all microorganisms present in a sample simultaneously.

---

# Why is Metagenomics Important?

Many microorganisms cannot be cultured under laboratory conditions.

Metagenomics allows researchers to investigate microbial diversity directly from natural environments.

---

# Applications of Metagenomics

- Human gut microbiome
- Soil microbiology
- Marine ecosystems
- Wastewater monitoring
- Agriculture
- Environmental surveillance

---

# Genomics vs Metagenomics

| Genomics | Metagenomics |
|-----------|--------------|
| Studies one organism | Studies microbial communities |
| Pure culture required | Direct environmental samples |
| Single genome | Mixed genomes |
| Easier assembly | More complex assembly |

---

# Environmental DNA (eDNA)

Environmental DNA (eDNA) refers to DNA collected directly from environmental samples such as:

- Soil
- Water
- Sediment
- Air
- Wastewater

without isolating individual organisms.

---

# Typical Metagenomic Workflow

Sample Collection

↓

DNA Extraction

↓

Library Preparation

↓

NGS Sequencing

↓

Quality Control

↓

Assembly

↓

Genome Binning

↓

Taxonomic Classification

↓

Functional Annotation

---

# Quality Control

Quality control is the first computational step after sequencing.

Its purpose is to remove:

- Adapter sequences
- Low-quality bases
- Short reads
- Sequencing artifacts

---

# FastQC

FastQC is a quality assessment tool used to evaluate raw sequencing reads.

It provides reports on:

- Per base quality
- GC content
- Sequence length distribution
- Adapter contamination
- Overrepresented sequences

---

# FastP

FastP is an all-in-one FASTQ preprocessing tool.

It performs:

- Adapter trimming
- Quality filtering
- Base correction
- Length filtering
- HTML report generation

---

# Key Takeaways

- Metagenomics enables culture-independent microbial analysis.
- Quality control is essential before downstream analyses.
- FastQC identifies sequencing problems.
- FastP improves sequencing read quality.