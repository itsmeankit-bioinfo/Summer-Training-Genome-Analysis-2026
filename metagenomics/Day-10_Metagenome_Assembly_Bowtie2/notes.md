# Notes

# What is Metagenome Assembly?

Metagenome assembly combines short sequencing reads obtained from a microbial community into longer DNA sequences called contigs.

Unlike genome assembly, metagenome assembly reconstructs genomes from multiple organisms simultaneously.

---

# SPAdes (--meta)

SPAdes is a genome assembler that also provides a metagenomic mode (`--meta`) for assembling shotgun metagenomic datasets.

Command used during the practical:

```bash
spades.py \
-1 module2-seq-R1-trimmed.fastq.gz \
-2 module2-seq-R2-trimmed.fastq.gz \
-o metagenome-assembly \
--meta
```

---

# MEGAHIT

MEGAHIT is a memory-efficient assembler specifically designed for large metagenomic datasets.

Command used during the practical:

```bash
megahit \
-1 module2-seq-R1-trimmed.fastq.gz \
-2 module2-seq-R2-trimmed.fastq.gz \
-o metagenome-assembly
```

Expected output:

- final.contigs.fa

---

# What is a SAM File?

SAM (Sequence Alignment/Map) is a text-based format used to store sequence alignment information.

A SAM file contains:

- Header
- Alignment section

The alignment section stores information for every sequencing read aligned to a reference sequence.

---

# Header Section

The header stores metadata such as:

- Reference sequences
- Sequencing program
- Read groups
- Sorting order

Common tags:

- @HD
- @SQ
- @RG

---

# What is a CIGAR String?

CIGAR (Compact Idiosyncratic Gapped Alignment Report) describes how each sequencing read aligns to the reference genome.

It records:

- Matches
- Insertions
- Deletions
- Soft clipping
- Hard clipping

---

# RNEXT

RNEXT stores the reference name of the paired read.

---

# PNEXT

PNEXT stores the alignment position of the paired read.

---

# TLEN

TLEN represents the observed template length between paired-end reads.

---

# What is a BAM File?

BAM is the binary version of a SAM file.

Advantages:

- Smaller file size
- Faster processing
- Efficient storage
- Compatible with downstream bioinformatics tools

---

# What is a BAM Index (BAI)?

A BAM Index allows rapid access to specific genomic regions without scanning the entire BAM file.

Benefits:

- Faster read retrieval
- Reduced computational time
- Efficient downstream analysis

---

# Bowtie2

Bowtie2 is a sequence alignment tool used to map sequencing reads against a reference genome or assembled contigs.

Typical workflow:

Reference Genome

↓

Build Index

↓

Align Reads

↓

Generate SAM File

↓

Convert to BAM

↓

Sorting

↓

Indexing

---

# Key Takeaways

- SPAdes and MEGAHIT assemble metagenomic reads.
- Bowtie2 aligns sequencing reads.
- SAM stores alignment information.
- BAM is the compressed binary version of SAM.
- BAM indexing improves downstream analysis performance.