# Notes

## What is WSL?

Windows Subsystem for Linux (WSL) allows Linux to run directly inside Windows without creating a virtual machine or dual boot system.

Advantages

- Easy to install
- Low memory usage
- Direct access to Windows files
- Supports bioinformatics software
- Faster than a virtual machine

---

## Why Ubuntu?

Ubuntu is one of the most widely used Linux distributions in bioinformatics because it has excellent package support and compatibility with scientific software.

Advantages

- Stable operating system
- Open source
- Large community support
- Compatible with most bioinformatics tools

---

## What is Miniconda?

Miniconda is a lightweight package manager used to install Python packages and bioinformatics software without affecting the operating system.

Advantages

- Creates isolated environments
- Prevents dependency conflicts
- Easy software installation
- Reproducible workflows

---

## What is a Conda Environment?

A Conda environment is an isolated workspace containing its own Python version and installed packages.

Example

Environment A

Python 3.10

FastP

FastQC

Environment B

Python 3.12

TensorFlow

PyTorch

These environments do not interfere with each other.

---

## What is FastP?

FastP is an all-in-one FASTQ preprocessing tool used before genome assembly or downstream analysis.

Functions

- Quality filtering
- Adapter trimming
- Read trimming
- Base correction
- Quality report generation

---

## Why do we perform quality control?

Sequencing machines produce reads that may contain

- Adapter contamination
- Low-quality bases
- Sequencing errors
- Very short reads

Quality control removes these problems before analysis.

---

## Typical NGS Workflow

DNA Extraction

↓

Sequencing

↓

FASTQ Files

↓

FastP

↓

FastQC

↓

Genome Assembly

↓

Annotation

↓

Biological Interpretation

---

## Important Linux Commands

| Command | Purpose |
|----------|----------|
| pwd | Show current directory |
| ls | List files |
| cd | Change directory |
| mkdir | Create folder |
| touch | Create file |
| cp | Copy file |
| mv | Move/Rename file |
| rm | Remove file |
| rmdir | Remove directory |
| cat | Display file contents |
| clear | Clear terminal |