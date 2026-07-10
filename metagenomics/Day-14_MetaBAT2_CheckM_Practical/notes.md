# Notes

# MetaBAT2 Practical

MetaBAT2 is an automated genome binning software used to reconstruct microbial genomes from assembled metagenomic contigs.

The software groups contigs using:

- Sequence composition
- Coverage information

---

# Input Files

MetaBAT2 requires:

- Assembly file (contigs.fasta or final.contigs.fasta)
- Sorted BAM file containing read alignment information

---

# Output

MetaBAT2 generates multiple genome bins.

Each genome bin is stored as a separate FASTA (.fa) file.

These files should be copied into a dedicated folder before quality assessment.

---

# CheckM

CheckM evaluates reconstructed genomes using lineage-specific marker genes.

It estimates:

- Genome completeness
- Genome contamination

---

# Lineage Workflow

The CheckM lineage workflow automatically identifies marker genes and estimates genome quality for every reconstructed MAG.

---

# Completeness

Higher completeness indicates that most expected marker genes are present.

---

# Contamination

Lower contamination indicates fewer sequences originating from other organisms.

---

# Importance of MAG Quality

Only high-quality MAGs should be used for:

- Genome annotation
- Comparative genomics
- Functional analysis
- Taxonomic classification

---

# Key Takeaways

- MetaBAT2 reconstructs microbial genomes.
- Genome bins are stored as FASTA files.
- CheckM evaluates genome quality before downstream analyses.