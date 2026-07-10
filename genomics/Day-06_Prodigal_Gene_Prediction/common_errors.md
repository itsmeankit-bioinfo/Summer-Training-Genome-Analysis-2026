# Common Errors & Troubleshooting

## Error 1

### prodigal: command not found

Cause

Prodigal is not installed or the Conda environment is inactive.

Solution

```bash
conda activate bioinfo
prodigal -v
```

---

## Error 2

Input FASTA file not found

Cause

Incorrect filename or wrong directory.

Solution

```bash
pwd
ls
```

Verify the input genome file.

---

## Error 3

Empty output files

Cause

Input assembly is empty or corrupted.

Solution

Check the assembly file before running Prodigal.

---

## Error 4

Very few predicted genes

Cause

Poor-quality genome assembly or incomplete contigs.

Solution

Improve assembly quality before gene prediction.

---

## Best Practices

- Use high-quality assembled genomes.
- Verify output files after execution.
- Keep GFF, FAA, and FNA files together for downstream analysis.