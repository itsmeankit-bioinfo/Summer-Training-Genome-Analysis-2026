# Commands Used

## Check WSL

```bash
wsl --status
```

Purpose

Checks whether WSL is installed.

---

## Install Ubuntu

```bash
wsl --install -d Ubuntu
```

Purpose

Installs Ubuntu distribution.

---

## Check Ubuntu Version

```bash
lsb_release -a
```

---

## Check Conda Version

```bash
conda --version
```

---

## Check Python Version

```bash
python --version
```

---

## Create Environment

```bash
conda create -n fastp
```

---

## Activate Environment

```bash
conda activate fastp
```

---

## Install FastP

```bash
conda install bioconda::fastp
```

---

## Check FastP Version

```bash
fastp --version
```

---

## Run FastP

```bash
fastp \
-i sample_R1.fastq.gz \
-I sample_R2.fastq.gz \
-o sample_R1_trimmed.fastq.gz \
-O sample_R2_trimmed.fastq.gz \
-h report.html \
-j report.json
```

Output

- Trimmed reads
- HTML report
- JSON report