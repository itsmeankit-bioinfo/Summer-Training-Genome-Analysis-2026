# Common Errors & Troubleshooting

## Error 1: fastqc: command not found

### Cause

FastQC is not installed or the Conda environment is not activated.

### Solution

```bash
conda activate bioinfo
fastqc --version
```

---

## Error 2: fastp: command not found

### Cause

FastP is not installed in the current environment.

### Solution

```bash
conda install bioconda::fastp
```

---

## Error 3: Failed to open input file

### Cause

Incorrect file name or wrong working directory.

### Solution

Check the current directory.

```bash
pwd
ls
```

Verify the FASTQ filenames.

---

## Error 4: Permission denied

### Cause

The user does not have permission to access the file.

### Solution

```bash
chmod +r sample.fastq.gz
```

---

## Error 5: Empty FastQC Report

### Cause

The FASTQ file is corrupted or empty.

### Solution

Verify file size.

```bash
ls -lh
```

---

## Best Practices

- Verify file names before running commands.
- Activate the correct Conda environment.
- Always perform FastQC before and after FastP.
- Store reports separately for comparison.