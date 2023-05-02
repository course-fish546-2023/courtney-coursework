---
title: "week-06"
output: html_document
date: "2023-05-02"
---

### a. What are SAM/BAM files? What is the difference between to the two?

Sequence Alignment/Mapping (SAM) files are plain text files that contain alignment sequences. BAM is the binary analog of this data, meaning that it is not readable by humans. BAM files are smaller and can be processed more quickly and efficiently.

### b. samtools is a popular program for working with alignment data. What are three common tasks that this software is used for?

-   Samtools Sort and Index (samtools sort, samtools index)- allows us to sort and index a BAM file so that we can get faster random access to aligned reads.

-   Convert between SAM and BAM (samtools view)- certain samtools only work on BAM files, so it is useful to be able to switch between the two formats

-   Extracting and filtering alignments (samtools view)- allows us to clean up and manipulate SAM/BAM files

### c. Why might you want to visualize alignment data and what are two program that can be used for this?

It is useful to visualize alignment data because it can allow us to scroll over chromosomes, look at specific regions, and learn more about our sequences (like mapping and base qualities). To do this, we can visualize alignments using either samtools tview or the Integrated Genomics Viewer (IGV).

### d. Describe what VCF file is?

VCF files are tab-delimited that have a metadata header (denoted with \##), a header line with the eight fields, and data lines. The data lines have information for a variant at a particular position as well as all the individuals' genotypes for that variant.
