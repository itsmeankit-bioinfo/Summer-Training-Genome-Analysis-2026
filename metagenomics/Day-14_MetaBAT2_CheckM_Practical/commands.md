# Commands Used

This practical focused on genome binning using MetaBAT2 and evaluating the resulting genome bins with CheckM.

---

# MetaBAT2 Installation

## Create Environment

```bash
conda create -n metabat2
```

## Activate Environment

```bash
conda activate metabat2
```

## Install MetaBAT2

```bash
conda install bioconda::metabat2
```

---

# Run MetaBAT2

```bash
runMetaBat.sh module2-seq-assembly.fasta sorted-module2-seq.bam
```

Purpose

Performs automated genome binning using:

- Assembly file
- Sorted BAM alignment file

---

# Organize Output Bins

After MetaBAT2 finishes, copy all generated `.fa` files into a separate folder for easier downstream analysis.

Purpose

Organizes all genome bins before quality assessment.

---

# CheckM Installation

## Create Environment

```bash
conda create -n checkm
```

## Activate Environment

```bash
conda activate checkm
```

## Install CheckM

```bash
conda install bioconda::checkm-genome
```

---

# Display Help

```bash
checkm -h
```

Purpose

Displays available CheckM commands.

---

# Run CheckM Lineage Workflow

```bash
checkm lineage_wf \
-x fa \
-t 16 \
module2-seq-bins \
checkm-results
```

Purpose

Evaluates completeness and contamination for each reconstructed genome bin.

---

# Generate Quality Assessment Report

```bash
checkm qa \
checkm-results/lineage.ms \
checkm-results \
-f quality_assessment.txt \
--tab_table
```

Purpose

Creates a tab-delimited quality assessment report.

---

# Expected Output

MetaBAT2

- Genome bins (.fa)

CheckM

- checkm-results/
- quality_assessment.txt