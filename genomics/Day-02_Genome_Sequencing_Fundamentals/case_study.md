# Case Study

# Why Poor Quality Reads Can Affect Genome Assembly

## Background

Genome assembly combines millions of short DNA reads into longer continuous sequences called contigs.

The quality of the final assembly depends heavily on the quality of the sequencing reads.

---

## Problem

Raw sequencing reads often contain:

- Adapter contamination
- Low-quality bases
- Sequencing errors
- Short reads

If these reads are assembled directly, they may produce:

- Incorrect contigs
- Fragmented assemblies
- Misassemblies
- Incorrect biological interpretation

---

## Solution

Before assembly, preprocessing tools such as FastP remove low-quality regions and adapters.

This results in:

- Cleaner reads
- Better assemblies
- Higher confidence analyses

---

## Real-World Example

Whole-genome sequencing projects, metagenomic studies, and clinical genomics pipelines routinely perform read preprocessing before assembly to ensure accurate downstream analysis.

---

## Conclusion

High-quality sequencing reads are essential for producing reliable genome assemblies and meaningful biological insights.