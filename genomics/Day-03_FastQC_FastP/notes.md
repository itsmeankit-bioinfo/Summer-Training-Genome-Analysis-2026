# Notes

# What is Quality Control (QC)?

Quality Control (QC) is the process of evaluating the quality of raw sequencing data before downstream analysis.

The objective is to identify sequencing errors, adapter contamination, low-quality bases, duplicated reads, and other issues that may affect biological interpretation.

---

# Why is Quality Control Important?

Poor-quality sequencing data can lead to:

- Incorrect genome assembly
- False variant detection
- Poor genome annotation
- Increased computational time
- Incorrect biological conclusions

Performing QC ensures reliable and reproducible results.

---

# What is FastQC?

FastQC is an open-source quality assessment tool used to evaluate FASTQ sequencing files.

It provides graphical reports that help identify quality issues before preprocessing.

FastQC does not modify sequencing data; it only analyzes and reports quality metrics.

---

# Features of FastQC

- Per base sequence quality
- Per sequence quality score
- Per base GC content
- Adapter content detection
- Sequence duplication analysis
- Overrepresented sequences
- Sequence length distribution
- N content analysis

---

# FastQC Output Files

Running FastQC generates:

1. HTML Report
2. ZIP Archive

The HTML report is used for visual inspection of sequencing quality.

---

# Understanding Phred Quality Score

Phred score measures the confidence of each base call during sequencing.

Higher Phred score indicates higher sequencing accuracy.

| Phred Score | Accuracy |
|-------------|----------|
| Q20 | 99% |
| Q30 | 99.9% |
| Q40 | 99.99% |

Generally, reads with Q30 or higher are considered high quality.

---

# Major FastQC Modules

## 1. Per Base Sequence Quality

Shows quality score across every base position.

Good quality is represented by high green box plots.

Poor quality usually appears toward the end of sequencing reads.

---

## 2. Per Sequence Quality Scores

Displays average quality for every sequencing read.

A good dataset contains most reads with high quality.

---

## 3. Per Base Sequence Content

Shows percentage of A, T, G, and C at every base position.

Large fluctuations may indicate sequencing bias.

---

## 4. Per Sequence GC Content

Shows GC percentage distribution.

Unexpected peaks may indicate contamination.

---

## 5. Per Base N Content

Represents unidentified nucleotides (N).

High N percentage indicates poor sequencing quality.

---

## 6. Sequence Length Distribution

Displays distribution of read lengths.

Most Illumina datasets have uniform read length.

---

## 7. Sequence Duplication Levels

Measures duplicate sequencing reads.

High duplication may result from PCR amplification.

---

## 8. Adapter Content

Detects adapter contamination.

Adapters should be removed before downstream analysis.

---

## 9. Overrepresented Sequences

Identifies sequences occurring more frequently than expected.

Possible reasons:

- Adapter contamination
- PCR bias
- Biological contamination

---

# What is FastP?

FastP is an all-in-one FASTQ preprocessing tool.

Unlike FastQC, FastP modifies sequencing reads to improve quality.

---

# Functions of FastP

- Adapter trimming
- Quality filtering
- PolyG trimming
- PolyX trimming
- Length filtering
- Base correction
- Duplicate removal (optional)
- HTML report generation
- JSON report generation

---

# FastP Output

FastP produces:

- Trimmed FASTQ files
- HTML quality report
- JSON report

---

# Adapter Trimming

Adapter sequences originate from library preparation.

If adapters remain in sequencing reads, they may interfere with genome assembly and alignment.

FastP automatically detects and removes adapters.

---

# Quality Filtering

Low-quality bases are removed according to user-defined quality thresholds.

This improves downstream analysis.

---

# Difference Between FastQC and FastP

| FastQC | FastP |
|---------|--------|
| Quality assessment | Read preprocessing |
| Generates reports | Modifies reads |
| No trimming | Performs trimming |
| No filtering | Performs filtering |
| Analysis only | Analysis + preprocessing |

---

# Typical Quality Control Pipeline

Raw FASTQ

↓

FastQC

↓

Quality Report

↓

FastP

↓

Trimmed FASTQ

↓

FastQC

↓

Improved Quality Report

↓

Genome Assembly

---

# Key Takeaways

- FastQC evaluates sequencing quality.
- FastP improves sequencing data.
- Adapter trimming is essential.
- Quality filtering increases data reliability.
- Clean sequencing reads improve downstream analyses.