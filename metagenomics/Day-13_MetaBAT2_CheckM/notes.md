# Notes

# What is Genome Binning?

Genome binning is the process of grouping assembled contigs that originate from the same microorganism.

The resulting genome is called a Metagenome-Assembled Genome (MAG).

---

# Why is Genome Binning Important?

Metagenomic assemblies contain DNA fragments from multiple organisms.

Binning separates these fragments into individual genomes for downstream analysis.

---

# What is MetaBAT2?

MetaBAT2 is an automated genome binning software designed for metagenomic assemblies.

It groups contigs based on:

- Sequence composition
- Coverage profiles

---

# Coverage Information

Coverage represents the number of sequencing reads aligned to a contig.

Contigs with similar coverage patterns are likely to belong to the same organism.

---

# Depth File

MetaBAT2 requires a depth file containing coverage information for every contig.

The depth file is generated using:

- jgi_summarize_bam_contig_depths

---

# What is a MAG?

A MAG (Metagenome-Assembled Genome) is a reconstructed microbial genome obtained directly from metagenomic sequencing data.

MAGs enable researchers to study microorganisms without culturing them.

---

# What is CheckM?

CheckM is a software package used to evaluate the quality of microbial genomes.

It estimates:

- Genome completeness
- Genome contamination
- Genome heterogeneity

---

# Genome Completeness

Completeness measures how much of the expected genome has been recovered.

Higher completeness indicates a more complete genome.

---

# Genome Contamination

Contamination measures unwanted sequences originating from other microorganisms.

Lower contamination is preferred.

---

# Typical Workflow

Assembly

↓

Read Mapping

↓

Coverage Calculation

↓

MetaBAT2

↓

MAGs

↓

CheckM

↓

Quality Assessment

---

# Key Takeaways

- Genome binning reconstructs microbial genomes.
- MetaBAT2 performs automated binning.
- CheckM evaluates MAG quality.
- High-quality MAGs are essential for downstream analyses.