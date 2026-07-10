# Common Errors & Troubleshooting

## Error 1

### fastqc: command not found

**Cause**

FastQC is not installed or the Conda environment is inactive.

**Solution**

```bash
conda activate bioinfo
fastqc --version
```

---

## Error 2

### fastp: command not found

**Cause**

FastP is not installed.

**Solution**

```bash
conda install bioconda::fastp
```

---

## Error 3

Input FASTQ files not found

**Cause**

Incorrect filename or wrong directory.

**Solution**

```bash
pwd
ls
```

Verify that the sequencing files are present.

---

## Error 4

Poor-quality reads remain after trimming

**Cause**

The trimming parameters may not remove all low-quality regions.

**Solution**

Review the FastQC report and adjust FastP parameters if necessary.

---

# Best Practices

- Always perform FastQC before and after trimming.
- Keep original FASTQ files unchanged.
- Store trimmed reads separately.