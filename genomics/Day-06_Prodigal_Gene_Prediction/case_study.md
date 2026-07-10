# Case Study

# Predicting Genes in a Newly Assembled Bacterial Genome

## Background

A bacterial genome was assembled successfully, but no information about its genes was available.

---

## Problem

Without identifying coding regions, the assembled genome cannot be functionally annotated or used for downstream biological studies.

---

## Solution

Prodigal was used to predict Open Reading Frames (ORFs) and generate coding sequences, protein sequences, and annotation files.

These outputs were then used for genome annotation.

---

## Real-world Example

Genome annotation pipelines such as Prokka use Prodigal internally to predict genes before assigning biological functions.

---

## Conclusion

Gene prediction is a critical step that transforms a raw genome assembly into biologically meaningful information.