# Common Errors & Troubleshooting

## Error 1

### megahit: command not found

Cause

MEGAHIT is not installed.

Solution

```bash
conda activate bioinfo
megahit --version
```

---

## Error 2

Input FASTQ files not found

Cause

Incorrect file names or wrong directory.

Solution

```bash
pwd
ls
```

Verify input files.

---

## Error 3

Assembly terminated

Cause

Insufficient RAM or storage.

Solution

- Free memory
- Close unnecessary applications
- Allocate sufficient disk space

---

## Error 4

Very fragmented assembly

Cause

Poor read quality or insufficient sequencing depth.

Solution

Review FastQC reports and preprocessing results.

---

## Best Practices

- Use high-quality reads.
- Monitor available RAM.
- Review assembly statistics before downstream analysis.