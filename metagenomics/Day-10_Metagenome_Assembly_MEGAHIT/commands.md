# Commands Used

## Step 1 — Activate Conda Environment

```bash
conda activate bioinfo
```

Purpose

Activates the Conda environment containing MEGAHIT.

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

Displays paired-end sequencing reads.

---

## Step 4 — Run MEGAHIT

```bash
megahit \
-1 sample_R1_trimmed.fastq.gz \
-2 sample_R2_trimmed.fastq.gz \
-o megahit_output
```

Purpose

Performs de novo metagenome assembly.

---

## Step 5 — Check Output Files

```bash
ls megahit_output
```

Purpose

Displays generated assembly files.

---

## Step 6 — View Final Contigs

```bash
head megahit_output/final.contigs.fa
```

Purpose

Displays the beginning of the assembled contigs.

---

## Step 7 — Obtain Assembly Statistics

```bash
seqkit stats megahit_output/final.contigs.fa
```

Purpose

Displays sequence statistics including:

- Number of contigs
- Total bases
- Average length
- Maximum length

---

# Expected Output

- final.contigs.fa
- log
- checkpoints
- intermediate assemblies