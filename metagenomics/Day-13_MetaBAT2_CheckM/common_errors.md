# Common Errors & Troubleshooting

## Error 1

### metabat2: command not found

Cause

MetaBAT2 is not installed or the Conda environment is inactive.

Solution

```bash
conda activate metabat2
metabat2 --help
```

---

## Error 2

Depth file not found

Cause

The depth file was not generated before running MetaBAT2.

Solution

Run:

```bash
jgi_summarize_bam_contig_depths
```

before MetaBAT2.

---

## Error 3

No genome bins generated

Cause

Assembly quality is poor or contigs are too short.

Solution

Improve assembly quality and verify coverage information.

---

## Error 4

CheckM fails to run

Cause

Genome bins are missing or incorrectly specified.

Solution

Verify the input directory containing genome bins.

---

# Best Practices

- Use sorted BAM files.
- Generate accurate depth files.
- Verify MAG quality before downstream analyses.