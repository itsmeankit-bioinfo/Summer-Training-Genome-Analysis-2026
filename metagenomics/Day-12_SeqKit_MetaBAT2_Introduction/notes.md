# Notes

# What is SeqKit?

SeqKit is a fast command-line toolkit used for manipulating FASTA and FASTQ files.

It provides multiple utilities for filtering, sampling, searching, converting, and generating sequence statistics.

---

# Features of SeqKit

- FASTA manipulation
- FASTQ manipulation
- Sequence statistics
- Sampling
- Searching
- Filtering
- File conversion

---

# Sequence Statistics

SeqKit reports information such as:

- Number of sequences
- Total sequence length
- Minimum length
- Maximum length
- Average length
- GC content

---

# FASTA Sampling

Sampling selects a subset of sequences from a larger FASTA file.

This is useful when testing pipelines or reducing computational requirements.

---

# Mapped Reads

Mapped reads successfully align to a reference sequence.

They provide information about:

- Genome coverage
- Species abundance
- Gene presence

---

# Unmapped Reads

Unmapped reads do not align to the reference sequence.

Possible reasons include:

- Novel organisms
- Poor-quality reads
- Sequencing errors
- Missing reference genomes

---

# What is Genome Binning?

Genome binning groups assembled contigs that likely originate from the same microorganism.

The result is a Metagenome-Assembled Genome (MAG).

---

# What is MetaBAT2?

MetaBAT2 is an automated genome binning software designed for metagenomic datasets.

It groups contigs using:

- Sequence composition
- Coverage information

---

# Sequence Composition

Sequence composition refers to characteristics such as:

- GC content
- Tetranucleotide frequencies
- K-mer frequencies

These features help distinguish genomes from different microorganisms.

---

# Coverage-based Binning

Coverage measures how many sequencing reads align to each contig.

Contigs with similar coverage profiles are likely to originate from the same organism.

---

# Typical Workflow

Assembly

↓

Alignment

↓

Coverage Calculation

↓

Genome Binning

↓

MAG Reconstruction

---

# Key Takeaways

- SeqKit is useful for sequence processing.
- Genome binning reconstructs genomes from mixed communities.
- MetaBAT2 combines sequence composition and coverage for accurate binning.