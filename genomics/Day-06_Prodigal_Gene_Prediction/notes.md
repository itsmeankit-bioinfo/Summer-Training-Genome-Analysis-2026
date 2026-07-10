# Notes

# What is Gene Prediction?

Gene prediction is the process of identifying protein-coding genes within a DNA sequence.

It determines which regions of the genome are likely to encode functional proteins.

---

# What is an ORF?

An Open Reading Frame (ORF) is a continuous stretch of DNA that begins with a start codon and ends with a stop codon without interruption.

An ORF represents a potential protein-coding region.

---

# Start Codons

Common start codons:

- ATG
- GTG
- TTG

---

# Stop Codons

Common stop codons:

- TAA
- TAG
- TGA

---

# Coding Sequence (CDS)

A Coding Sequence (CDS) is the portion of a gene that is translated into protein.

---

# Difference Between ORF and Gene

| ORF | Gene |
|------|------|
| Potential coding region | Functional DNA sequence |
| Identified computationally | Confirmed biologically |
| May or may not encode protein | Encodes a functional product |

---

# What is Prodigal?

Prodigal (PROkaryotic DYnamic programming Gene-finding ALgorithm) is a software tool used to predict protein-coding genes in bacterial and archaeal genomes.

---

# Features of Prodigal

- Fast
- Accurate
- Designed for prokaryotes
- Predicts coding sequences
- Generates protein sequences
- Produces annotation files

---

# Prodigal Output Files

## GFF

Genome annotation coordinates.

---

## FAA

Predicted protein sequences.

---

## FNA

Predicted nucleotide coding sequences.

---

## GBK

Genome annotation in GenBank format (optional).

---

# Typical Workflow

Genome Assembly

↓

Contigs

↓

Prodigal

↓

ORFs

↓

Protein Sequences

↓

Genome Annotation

---

# Key Takeaways

- ORFs are predicted coding regions.
- Prodigal predicts genes in bacterial genomes.
- Gene prediction is essential before genome annotation.