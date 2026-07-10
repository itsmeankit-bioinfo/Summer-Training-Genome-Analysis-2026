# Common Errors & Troubleshooting

## Error 1

### metaquast.py: command not found

**Cause**

MetaQUAST environment is not activated.

**Solution**

```bash
conda activate metaquast
```

---

## Error 2

### samtools: command not found

**Cause**

SAMtools is not installed.

**Solution**

```bash
conda activate samtools
```

---

## Error 3

SAM file not found

**Cause**

Incorrect working directory.

**Solution**

```bash
pwd
ls
```

---

## Error 4

BAM index not generated

**Cause**

The BAM file was not sorted before indexing.

**Solution**

Run:

```bash
samtools sort
```

before

```bash
samtools index
```

---

## Best Practices

- Always sort BAM files before indexing.
- Verify MetaQUAST reports before downstream analysis.
- Store alignment files in dedicated output folders.