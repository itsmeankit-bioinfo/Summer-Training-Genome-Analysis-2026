# Commands Used

## Step 1 — Activate Conda Environment

```bash
conda activate bioinfo
```

Purpose

Activates the Conda environment containing the required bioinformatics tools.

---

## Step 2 — Check Working Directory

```bash
pwd
```

Displays the current working directory.

---

## Step 3 — List Input Files

```bash
ls
```

Verifies that paired-end FASTQ files are present.

---

## Step 4 — Run FastQC

```bash
fastqc sample_R1.fastq.gz sample_R2.fastq.gz
```

Purpose

Performs quality assessment on raw metagenomic reads.

---

## Step 5 — Run FastP

```bash
fastp \
-i sample_R1.fastq.gz \
-I sample_R2.fastq.gz \
-o sample_R1_trimmed.fastq.gz \
-O sample_R2_trimmed.fastq.gz \
-h fastp_report.html \
-j fastp_report.json
```

Purpose

Removes adapters and low-quality bases before metagenomic assembly.

---

## Step 6 — Run FastQC Again

```bash
fastqc sample_R1_trimmed.fastq.gz sample_R2_trimmed.fastq.gz
```

Purpose

Verifies the quality improvement after trimming.

---

## Expected Output

- Trimmed FASTQ files
- FastQC HTML reports
- FastQC ZIP reports
- FastP HTML report
- FastP JSON report