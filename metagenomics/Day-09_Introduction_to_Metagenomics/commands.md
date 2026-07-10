# Commands Used

This practical introduced quality control tools used in metagenomic analysis.

---

# Step 1 — Activate Conda Environment

```bash
conda activate bioinfo
```

**Purpose**

Activates the Conda environment containing FastQC and FastP.

---

# Step 2 — Check Working Directory

```bash
pwd
```

**Purpose**

Displays the current working directory.

---

# Step 3 — List Input Files

```bash
ls
```

**Purpose**

Displays the paired-end FASTQ files.

---

# Step 4 — Run FastQC

```bash
fastqc module2-seq-R1.fastq.gz module2-seq-R2.fastq.gz
```

**Purpose**

Performs quality assessment of raw sequencing reads before trimming.

---

# Step 5 — Run FastP

```bash
fastp \
-i module2-seq-R1.fastq.gz \
-I module2-seq-R2.fastq.gz \
-o module2-seq-R1-trimmed.fastq.gz \
-O module2-seq-R2-trimmed.fastq.gz
```

**Purpose**

Removes adapter sequences and low-quality bases from sequencing reads.

---

# Step 6 — Run FastQC on Trimmed Reads

```bash
fastqc module2-seq-R1-trimmed.fastq.gz module2-seq-R2-trimmed.fastq.gz
```

**Purpose**

Evaluates the quality of reads after preprocessing.

---

# Expected Output

- module2-seq-R1-trimmed.fastq.gz
- module2-seq-R2-trimmed.fastq.gz
- FastQC HTML reports
- FastQC ZIP reports