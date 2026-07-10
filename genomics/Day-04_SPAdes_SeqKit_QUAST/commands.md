# Commands Used

## Step 1 — Activate Conda Environment

```bash
conda activate bioinfo
```

Purpose

Activates the Conda environment containing SPAdes, SeqKit, and QUAST.

---

## Step 2 — Check Working Directory

```bash
pwd
```

Displays the current working directory.

---

## Step 3 — List Files

```bash
ls
```

Displays available sequencing files.

---

## Step 4 — Run SPAdes

```bash
spades.py \
-1 sample_R1_trimmed.fastq.gz \
-2 sample_R2_trimmed.fastq.gz \
-o spades_output
```

Purpose

Performs de novo genome assembly using paired-end sequencing reads.

---

## Step 5 — Check Assembly Output

```bash
ls spades_output
```

Displays generated assembly files.

---

## Step 6 — View Assembly Statistics Using SeqKit

```bash
seqkit stats spades_output/contigs.fasta
```

Purpose

Displays statistics such as number of sequences, total length, minimum length, maximum length, and average sequence length.

---

## Step 7 — Run QUAST

```bash
quast.py spades_output/contigs.fasta
```

Purpose

Evaluates genome assembly quality.

---

## Step 8 — QUAST with Reference Genome

```bash
quast.py \
-r reference.fasta \
spades_output/contigs.fasta
```

Purpose

Compares assembled genome against a reference genome.

---

## Expected Output

- contigs.fasta
- scaffolds.fasta
- assembly_graph.fastg
- QUAST HTML Report
- Assembly Statistics