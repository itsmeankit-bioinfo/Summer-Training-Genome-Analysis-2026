# Commands Used

## Step 1 — Activate Conda Environment

```bash
conda activate bioinfo
```

Purpose

Activates the Conda environment containing Prodigal.

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

Displays the assembled genome files.

---

## Step 4 — Run Prodigal

```bash
prodigal \
-i contigs.fasta \
-a proteins.faa \
-d genes.fna \
-o annotation.gff
```

Purpose

Predicts protein-coding genes (ORFs) from the assembled genome.

---

## Step 5 — View Output Files

```bash
ls
```

Expected Output

```
proteins.faa
genes.fna
annotation.gff
```

---

## Step 6 — Count Predicted Genes

```bash
grep ">" proteins.faa | wc -l
```

Purpose

Counts the total number of predicted protein sequences.

---

## Step 7 — View First Protein Sequence

```bash
head proteins.faa
```

Purpose

Displays the first predicted protein sequence.

---

# Summary

Prodigal predicts protein-coding genes from assembled genomes and generates nucleotide, protein, and annotation files for downstream genome annotation.