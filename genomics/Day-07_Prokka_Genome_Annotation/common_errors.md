# Common Errors & Troubleshooting

## Error 1

### prokka: command not found

Cause

Prokka is not installed or the Conda environment is inactive.

Solution

```bash
conda activate bioinfo
prokka --version
```

---

## Error 2

Input FASTA file not found

Cause

Incorrect file name or path.

Solution

```bash
pwd
ls
```

Verify the input genome file.

---

## Error 3

BLAST+ dependency missing

Cause

Required dependency is not installed.

Solution

Install BLAST+ in the Conda environment.

---

## Error 4

No genes predicted

Cause

Poor-quality assembly or incorrect input genome.

Solution

Verify the assembly quality before annotation.

---

## Best Practices

- Use high-quality assembled genomes.
- Verify Prokka dependencies.
- Review annotation files before downstream analysis.