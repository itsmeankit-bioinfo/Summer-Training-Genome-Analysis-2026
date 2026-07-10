# Common Errors & Troubleshooting

## Error 1: FASTA file not displaying correctly

### Cause

The FASTA header line (`>`) is missing.

### Solution

Ensure every sequence begins with a header line.

Example

```text
>Sequence_1
ATGCGTAGCTAG
```

---

## Error 2: FASTQ file format is incorrect

### Cause

A FASTQ record must contain exactly four lines.

### Correct Format

```text
@Sequence_ID
ATGCGTAGCTA
+
IIIIIIIIIII
```

---

## Error 3: Low Quality Reads

### Cause

Poor sequencing quality or adapter contamination.

### Solution

Perform read preprocessing using FastP before downstream analysis.

---

## Error 4: FASTA and FASTQ confusion

### Cause

Many beginners assume both formats are identical.

### Difference

FASTA stores only biological sequences.

FASTQ stores sequences together with quality scores.

---

# Lessons Learned

- Always verify sequence file format.
- Perform quality assessment before analysis.
- Never skip preprocessing.
- High-quality reads produce better genome assemblies.