# Commands Used

This practical focused on sequence manipulation using SeqKit and understanding the concepts of genome binning using MetaBAT2.

---

# SeqKit Installation

## Create Environment

```bash
conda create -n seqkit -y
```

## Activate Environment

```bash
conda activate seqkit
```

## Install SeqKit

```bash
conda install bioconda::seqkit
```

---

# Check SeqKit Version

```bash
seqkit version
```

Purpose

Verifies successful installation.

---

# Generate Sequence Statistics

```bash
seqkit stats final.contigs.fa
```

Purpose

Displays:

- Number of sequences
- Total sequence length
- Minimum length
- Maximum length
- Average length
- GC content

---

# Sample Sequences

```bash
seqkit sample \
-p 0.1 \
final.contigs.fa \
> sampled_contigs.fa
```

Purpose

Randomly samples 10% of sequences from the FASTA file.

---

# View FASTA File

```bash
seqkit head final.contigs.fa
```

Purpose

Displays the first few sequences.

---

# Count Sequences

```bash
seqkit stats sampled_contigs.fa
```

Purpose

Confirms the sampled dataset.

---

# Expected Output

- sampled_contigs.fa
- Sequence statistics
- FASTA summary