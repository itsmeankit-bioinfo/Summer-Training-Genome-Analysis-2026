# Commands Used

This document contains the Linux commands and bioinformatics tools used during the Day 3 practical session.

---

# Step 1 — Activate Conda Environment

```bash
conda activate bioinfo
```

## Purpose

Activates the bioinformatics Conda environment containing the required software.

---

# Step 2 — Move to Working Directory

```bash
cd /path/to/practical_directory
```

Example

```bash
cd ~/Genome_Practical
```

## Purpose

Moves into the directory containing sequencing files.

---

# Step 3 — Check Input Files

```bash
ls
```

## Purpose

Displays all files in the current directory.

---

# Step 4 — Run FastQC

```bash
fastqc sample_R1.fastq.gz sample_R2.fastq.gz
```

## Purpose

Performs quality assessment of paired-end sequencing reads.

---

# Step 5 — Run FastP

```bash
fastp \
-i sample_R1.fastq.gz \
-I sample_R2.fastq.gz \
-o sample_R1_trimmed.fastq.gz \
-O sample_R2_trimmed.fastq.gz \
-h fastp_report.html \
-j fastp_report.json
```

## Purpose

Removes low-quality bases and adapter contamination from sequencing reads.

---

# Step 6 — Run FastQC on Trimmed Reads

```bash
fastqc sample_R1_trimmed.fastq.gz sample_R2_trimmed.fastq.gz
```

## Purpose

Evaluates the quality improvement after preprocessing.

---

# Step 7 — Verify Generated Files

```bash
ls
```

Expected Output

```
sample_R1.fastq.gz
sample_R2.fastq.gz
sample_R1_trimmed.fastq.gz
sample_R2_trimmed.fastq.gz
fastp_report.html
fastp_report.json
```

---

# Useful Linux Commands

Display current directory

```bash
pwd
```

Create folder

```bash
mkdir outputs
```

Copy file

```bash
cp file1 file2
```

Move file

```bash
mv old_name new_name
```

Remove file

```bash
rm filename
```

Remove directory

```bash
rm -r directory_name
```

---

# Summary

FastQC was used before and after FastP preprocessing to compare sequencing quality.

FastP generated cleaned FASTQ files together with HTML and JSON reports for downstream analysis.