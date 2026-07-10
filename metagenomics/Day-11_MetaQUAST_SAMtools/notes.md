# Notes

# What is MetaQUAST?

MetaQUAST is a quality assessment tool specifically designed for evaluating metagenome assemblies.

It compares assembled contigs against reference genomes and reports multiple assembly quality statistics.

---

# Why is MetaQUAST Important?

MetaQUAST helps researchers:

- Evaluate assembly completeness
- Compare different assemblies
- Identify misassemblies
- Measure assembly accuracy

---

# Assembly Statistics

Common statistics include:

- Number of contigs
- Total assembly length
- Largest contig
- N50
- L50
- GC content

---

# What is SAMtools?

SAMtools is a software package used to manipulate SAM and BAM alignment files.

It performs operations such as:

- Viewing alignments
- Converting formats
- Sorting
- Indexing
- Filtering

---

# SAM to BAM Conversion

SAM files are text-based and relatively large.

BAM files are compressed binary versions of SAM files.

Advantages of BAM:

- Smaller size
- Faster processing
- Efficient storage

---

# BAM Sorting

Sorting organizes alignments according to genomic coordinates.

Sorted BAM files are required by many downstream bioinformatics tools.

---

# BAM Indexing

Indexing creates a `.bai` file that allows rapid access to specific genomic regions without reading the complete BAM file.

---

# Typical Workflow

SAM File

↓

BAM Conversion

↓

Sorting

↓

Indexing

↓

Downstream Analysis

---

# Key Takeaways

- MetaQUAST evaluates metagenome assembly quality.
- SAMtools efficiently processes alignment files.
- BAM sorting and indexing improve downstream analyses.