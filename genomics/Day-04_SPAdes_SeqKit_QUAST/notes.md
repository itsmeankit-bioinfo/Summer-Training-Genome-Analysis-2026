# Notes

# What is Genome Assembly?

Genome assembly is the process of reconstructing a complete genome by joining millions of short sequencing reads into longer continuous sequences called contigs.

---

# Why is Genome Assembly Needed?

Sequencing platforms generate short DNA fragments rather than complete genomes.

Assembly combines these fragments to reconstruct the original genome.

Applications:

- Genome Annotation
- Comparative Genomics
- Variant Analysis
- Evolutionary Studies

---

# What is a Contig?

A contig is a continuous DNA sequence produced by assembling overlapping sequencing reads.

Longer contigs generally indicate better assembly quality.

---

# What is a Scaffold?

A scaffold consists of multiple contigs connected using paired-end sequencing information.

Scaffolds provide a more complete genome representation.

---

# De novo Genome Assembly

De novo assembly reconstructs a genome without using a reference genome.

Advantages:

- Suitable for novel organisms
- Detects structural variations
- Independent of reference bias

---

# What is SPAdes?

SPAdes (St. Petersburg Genome Assembler) is a genome assembler designed primarily for bacterial genomes and single-cell sequencing data.

Features:

- De novo assembly
- Multi-k-mer assembly
- Error correction
- Supports paired-end reads

---

# What is SeqKit?

SeqKit is a toolkit for FASTA and FASTQ file manipulation.

Functions:

- Sequence statistics
- Sequence extraction
- Filtering
- File conversion

---

# What is QUAST?

QUAST (Quality Assessment Tool for Genome Assemblies) evaluates assembled genomes using various statistical metrics.

---

# Important Assembly Statistics

## Number of Contigs

Lower values generally indicate better assembly.

---

## Largest Contig

Length of the longest assembled contig.

---

## Total Assembly Length

Total length of all assembled contigs.

---

## N50

N50 is the contig length such that 50% of the total assembly length is contained in contigs of that length or longer.

Higher N50 generally indicates better assembly.

---

## L50

L50 is the minimum number of contigs required to cover 50% of the assembled genome.

Lower L50 is preferred.

---

# Typical Assembly Pipeline

Quality Reads

↓

SPAdes

↓

Contigs

↓

SeqKit

↓

QUAST

↓

Assembly Evaluation

↓

Genome Annotation

---

# Key Takeaways

- Genome assembly reconstructs genomes from sequencing reads.
- SPAdes is widely used for bacterial genome assembly.
- QUAST measures assembly quality.
- N50 and L50 are important assembly statistics.