# Commands Used

This practical focused on metagenome assembly and sequence alignment using SPAdes, MEGAHIT, and Bowtie2.

---

# SPAdes Installation

## Create Environment

```bash
conda create -n spades -y
```

## Activate Environment

```bash
conda activate spades
```

## Install SPAdes

```bash
conda install bioconda::spades
```

---

# Run SPAdes (Metagenome Mode)

```bash
spades.py \
-1 module2-seq-R1-trimmed.fastq.gz \
-2 module2-seq-R2-trimmed.fastq.gz \
-o metagenome-assembly \
--meta
```

Purpose

Performs metagenome assembly using SPAdes.

---

# MEGAHIT Installation

## Create Environment

```bash
conda create -n megahit -y
```

## Activate Environment

```bash
conda activate megahit
```

## Install MEGAHIT

```bash
conda install bioconda::megahit
```

---

# Run MEGAHIT

```bash
megahit \
-1 module2-seq-R1-trimmed.fastq.gz \
-2 module2-seq-R2-trimmed.fastq.gz \
-o metagenome-assembly
```

Purpose

Assembles shotgun metagenomic reads.

---

# Bowtie2 Installation

## Create Environment

```bash
conda create -n bowtie2 -y
```

## Activate Environment

```bash
conda activate bowtie2
```

## Install Bowtie2

```bash
conda install bioconda::bowtie2
```

---

## Check Version

```bash
bowtie2 --help
```

```bash
bowtie2 --version
```

---

# Build Reference Index

```bash
bowtie2-build assembly.fasta module2-seq
```

Purpose

Creates Bowtie2 index files from the assembled genome.

---

# Align Reads

```bash
bowtie2 \
--no-unal \
-x module2-seq \
-1 module2-seq-R1-trimmed.fastq.gz \
-2 module2-seq-R2-trimmed.fastq.gz \
-S module2-seq.sam
```

Purpose

Aligns sequencing reads against the assembled reference genome.

---

# Expected Output

SPAdes

- contigs.fasta

MEGAHIT

- final.contigs.fa

Bowtie2

- module2-seq.sam