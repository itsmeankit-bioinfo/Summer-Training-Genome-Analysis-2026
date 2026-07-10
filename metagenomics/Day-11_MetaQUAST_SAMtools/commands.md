# Commands Used

This practical focused on evaluating metagenome assemblies using MetaQUAST and processing alignment files using SAMtools.

---

# MetaQUAST Installation

## Create Environment

```bash
conda create -n metaquast -y
```

## Activate Environment

```bash
conda activate metaquast
```

## Install MetaQUAST

```bash
conda install bioconda::quast
```

---

# Run MetaQUAST

```bash
metaquast.py \
metagenome-assembly/final.contigs.fa \
-o metaquast_output
```

**Purpose**

Evaluates the quality of the metagenome assembly and generates summary reports.

---

# SAMtools Installation

## Create Environment

```bash
conda create -n samtools -y
```

## Activate Environment

```bash
conda activate samtools
```

## Install SAMtools

```bash
conda install bioconda::samtools
```

---

# Check Version

```bash
samtools --version
```

---

# View SAM File

```bash
samtools view module2-seq.sam
```

**Purpose**

Displays alignment records stored in the SAM file.

---

# Convert SAM to BAM

```bash
samtools view \
-bS module2-seq.sam \
> module2-seq.bam
```

**Purpose**

Converts the text-based SAM file into the compressed BAM format.

---

# Sort BAM File

```bash
samtools sort \
module2-seq.bam \
-o module2-seq.sorted.bam
```

**Purpose**

Sorts alignments by genomic coordinates.

---

# Index BAM File

```bash
samtools index module2-seq.sorted.bam
```

**Purpose**

Creates an index (.bai) file for rapid random access.

---

# View BAM Statistics

```bash
samtools flagstat module2-seq.sorted.bam
```

**Purpose**

Displays alignment statistics including mapped and unmapped reads.

---

# Expected Output

MetaQUAST

- report.html
- report.tsv
- transposed_report.tsv

SAMtools

- module2-seq.bam
- module2-seq.sorted.bam
- module2-seq.sorted.bam.bai