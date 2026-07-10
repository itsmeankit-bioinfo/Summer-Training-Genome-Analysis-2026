# Common Errors & Troubleshooting

## Error 1

### spades.py: command not found

Cause

SPAdes is not installed or the Conda environment is inactive.

Solution

```bash
conda activate bioinfo
spades.py --version
```

---

## Error 2

Input FASTQ file not found

Cause

Incorrect file path.

Solution

```bash
pwd
ls
```

Verify filenames.

---

## Error 3

Assembly terminated unexpectedly

Cause

Insufficient RAM or disk space.

Solution

- Close unnecessary applications.
- Allocate more memory.
- Ensure sufficient storage.

---

## Error 4

QUAST report not generated

Cause

Assembly file missing or corrupted.

Solution

Verify

```bash
ls spades_output
```

---

## Best Practices

- Use high-quality reads.
- Check assembly statistics before annotation.
- Compare assemblies using QUAST.