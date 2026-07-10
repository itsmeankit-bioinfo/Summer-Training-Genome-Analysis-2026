# Common Errors & Troubleshooting

## Error 1

### runMetaBat.sh: command not found

Cause

MetaBAT2 is not installed or the environment is inactive.

Solution

```bash
conda activate metabat2
```

---

## Error 2

Assembly file not found

Cause

Incorrect filename or working directory.

Solution

```bash
pwd
ls
```

Verify the assembly FASTA file.

---

## Error 3

Sorted BAM file missing

Cause

The BAM file was not generated or sorted.

Solution

Complete the Bowtie2 and SAMtools workflow before running MetaBAT2.

---

## Error 4

CheckM cannot find genome bins

Cause

The input folder does not contain `.fa` files.

Solution

Copy all generated genome bins into a dedicated folder.

---

## Best Practices

- Use sorted BAM files.
- Keep all genome bins in one folder.
- Verify the CheckM report before downstream analysis.