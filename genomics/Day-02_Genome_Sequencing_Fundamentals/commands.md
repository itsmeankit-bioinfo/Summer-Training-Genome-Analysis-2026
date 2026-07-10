# Commands Used

## Display FASTA File

```bash
cat sequence.fasta
```

Displays the contents of a FASTA file.

---

## Display FASTQ File

```bash
cat sample.fastq
```

Displays the contents of a FASTQ file.

---

## Count Number of Sequences

```bash
grep "^>" sequence.fasta | wc -l
```

Counts sequences in a FASTA file.

---

## View First Few Reads

```bash
head sample.fastq
```

Displays the first few sequencing reads.

---

## Count Lines

```bash
wc -l sample.fastq
```

Counts the total number of lines in a FASTQ file.