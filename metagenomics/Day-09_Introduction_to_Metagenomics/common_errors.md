# Common Errors & Troubleshooting

## Error 1

### fastqc: command not found

Cause

FastQC is not installed or the Conda environment is inactive.

Solution

```bash
conda activate bioinfo
fastqc --version
```

---

## Error 2

### fastp: command not found

Cause

FastP is not installed.

Solution

```bash
conda install bioconda::fastp
```

---

## Error 3

Input FASTQ file not found

Cause

Incorrect file path.

Solution

```bash
pwd
ls
```

Verify the filenames.

---

## Error 4

Poor-quality reads remain after trimming

Cause

The trimming parameters may not be appropriate for the dataset.

Solution

Review FastQC reports and adjust FastP settings if necessary.

---

## Best Practices

- Perform FastQC before and after trimming.
- Keep original FASTQ files unchanged.
- Review HTML reports before continuing.