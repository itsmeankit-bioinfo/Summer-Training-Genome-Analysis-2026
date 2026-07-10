# Common Errors & Troubleshooting

## Error 1

Reference genome not found

### Cause

Incorrect file path.

### Solution

```bash
ls
pwd
```

Verify the reference genome location.

---

## Error 2

QUAST report not generated

### Cause

Assembly file is missing or corrupted.

### Solution

Check

```bash
ls contigs.fasta
```

---

## Error 3

TYGS upload failed

### Cause

Incorrect file format or unstable internet connection.

### Solution

Upload a valid FASTA assembly file.

---

## Error 4

Poor genome fraction

### Cause

Low-quality assembly.

### Solution

Improve read quality and repeat genome assembly.

---

## Best Practices

- Always use the latest reference genome.
- Validate assemblies before annotation.
- Compare multiple assembly metrics.