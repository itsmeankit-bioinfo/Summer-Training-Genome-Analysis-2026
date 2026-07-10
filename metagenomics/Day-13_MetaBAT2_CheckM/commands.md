# Commands Used

This practical focused on genome binning using MetaBAT2 and evaluating the quality of Metagenome-Assembled Genomes (MAGs) using CheckM.

---

# MetaBAT2 Installation

## Create Environment

```bash
conda create -n metabat2 -y
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

# Check MetaBAT2 Version

```bash
metabat2 --help
```

Purpose

Verifies successful installation.

---

# Generate Depth File

```bash
jgi_summarize_bam_contig_depths \
--outputDepth depth.txt \
module2-seq.sorted.bam
```

Purpose

Calculates contig coverage from the sorted BAM file.

---

# Run MetaBAT2

```bash
metabat2 \
-i final.contigs.fa \
-a depth.txt \
-o bins/bin
```

Purpose

Groups assembled contigs into genome bins based on sequence composition and coverage.

---

# Check Generated Bins

```bash
ls bins/
```

Purpose

Displays all reconstructed genome bins.

---

# CheckM Installation

## Create Environment

```bash
conda create -n checkm -y
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

# Run CheckM Lineage Workflow

```bash
checkm lineage_wf \
bins/ \
checkm_output
```

Purpose

Evaluates genome completeness and contamination of reconstructed MAGs.

---

# View Results

```bash
checkm qa
```

Purpose

Displays MAG quality statistics.

---

# Expected Output

MetaBAT2

- bins/

CheckM

- Completeness report
- Contamination report
- Genome quality summary