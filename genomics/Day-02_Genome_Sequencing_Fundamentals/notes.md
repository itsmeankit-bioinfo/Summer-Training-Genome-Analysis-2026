# Notes

# What is a Genome?

A genome is the complete set of genetic material (DNA) present in an organism. It contains all the information required for the growth, development, reproduction, and functioning of that organism.

Examples:

- Human Genome ≈ 3.2 billion base pairs
- E. coli Genome ≈ 4.6 million base pairs

---

# What is Genomics?

Genomics is the branch of biology that studies the complete genome of an organism, including its structure, function, evolution, mapping, and sequencing.

Applications:

- Disease diagnosis
- Drug discovery
- Agriculture
- Personalized medicine
- Evolutionary studies

---

# What is DNA Sequencing?

DNA sequencing is the process of determining the exact order of nucleotides (A, T, G, and C) in a DNA molecule.

Example:

ATGCTAGCTAGCGATCG

---

# What is Next Generation Sequencing (NGS)?

Next Generation Sequencing (NGS) is a high-throughput sequencing technology capable of sequencing millions of DNA fragments simultaneously.

Advantages:

- High speed
- High accuracy
- Cost-effective
- Massive data generation

Applications:

- Whole Genome Sequencing
- Metagenomics
- RNA Sequencing
- Variant Analysis
- Cancer Genomics

---

# DNA Sequencing Workflow

DNA Extraction

↓

Library Preparation

↓

DNA Sequencing

↓

FASTQ Generation

↓

Quality Control

↓

Read Trimming

↓

Genome Assembly

↓

Genome Annotation

↓

Biological Interpretation

---

# FASTA Format

FASTA is a text-based format used to store biological sequences.

Structure:

>Sequence_ID

ATGCGTAGCTAGCTAGCTA

Characteristics:

- Stores sequence only
- No quality information
- Used for genome and protein sequences

---

# FASTQ Format

FASTQ stores both sequence data and sequencing quality scores.

Structure:

@Sequence_ID

ATGCGTAGCTA

+

IIIIIIIIIII

Characteristics:

- Stores nucleotide sequence
- Stores quality scores
- Standard format for NGS data

---

# Difference Between FASTA and FASTQ

| FASTA | FASTQ |
|--------|--------|
| Sequence only | Sequence + Quality |
| Smaller size | Larger size |
| Used after processing | Generated directly from sequencing |

---

# Phred Quality Score

Phred Score measures the confidence of each nucleotide identified during sequencing.

Higher score = Better sequencing quality.

Common Values:

Q20 → 99% accuracy

Q30 → 99.9% accuracy

Q40 → 99.99% accuracy

---

# Why Read Preprocessing is Important

Raw sequencing data may contain:

- Adapter sequences
- Low-quality bases
- Duplicate reads
- Short reads
- Sequencing errors

Preprocessing improves data quality before downstream analysis.

---

# FastP

FastP is an all-in-one FASTQ preprocessing tool.

Functions:

- Adapter trimming
- Quality filtering
- Length filtering
- Base correction
- HTML report generation
- JSON report generation

---

# Key Takeaways

✔ Genome = Complete DNA of an organism

✔ Genomics = Study of genomes

✔ FASTA stores sequences

✔ FASTQ stores sequences + quality

✔ Phred score measures sequencing quality

✔ FastP improves sequencing data quality