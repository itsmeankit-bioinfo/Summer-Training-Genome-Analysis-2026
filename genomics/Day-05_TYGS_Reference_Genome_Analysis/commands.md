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

## Step 3 — List Available Files

```bash
ls
```

Displays genome assembly files and reference genome.

---

## Step 4 — Run QUAST with Reference Genome

```bash
quast.py \
-r reference_genome.fasta \
contigs.fasta
```

Purpose

Evaluates the assembled genome by comparing it against a known reference genome.

---

## Step 5 — Open TYGS

Visit:

https://tygs.dsmz.de/

Upload the assembled genome for taxonomic identification.

---

## Step 6 — Review QUAST Results

Generated files include:

- report.html
- report.tsv
- transposed_report.tsv

---

## Expected Output

- Assembly statistics
- Genome fraction
- Number of misassemblies
- GC content
- N50
- L50
- Alignment statistics