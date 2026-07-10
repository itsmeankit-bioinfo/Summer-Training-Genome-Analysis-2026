# Common Errors & Troubleshooting

## Error 1

### seqkit: command not found

Cause

SeqKit is not installed or the environment is inactive.

Solution

```bash
conda activate seqkit
seqkit version
```

---

## Error 2

Input FASTA file not found

Cause

Incorrect file path.

Solution

```bash
pwd
ls
```

Verify that the FASTA file exists.

---

## Error 3

Empty output file after sampling

Cause

Incorrect sampling percentage or invalid input.

Solution

Verify the FASTA file and sampling parameters.

---

## Error 4

Unexpected sequence statistics

Cause

The input FASTA file may be incomplete or corrupted.

Solution

Validate the assembly before analysis.

---

# Best Practices

- Always inspect FASTA files before analysis.
- Verify sequence statistics after every major step.
- Keep original assembly files unchanged.