# Common Errors & Troubleshooting

## Error 1

### spades.py: command not found

Cause

SPAdes environment is not activated.

Solution

```bash
conda activate spades
```

---

## Error 2

### megahit: command not found

Cause

MEGAHIT is not installed.

Solution

```bash
conda activate megahit
```

---

## Error 3

### bowtie2: command not found

Cause

Bowtie2 environment is inactive.

Solution

```bash
conda activate bowtie2
```

---

## Error 4

Reference index missing

Cause

bowtie2-build was not executed.

Solution

Build the index before alignment.

---

## Error 5

Input FASTQ files not found

Solution

```bash
pwd
ls
```

Verify filenames before running commands.

---

# Best Practices

- Use trimmed reads for assembly.
- Verify the reference index before alignment.
- Store SAM files separately from FASTQ files.