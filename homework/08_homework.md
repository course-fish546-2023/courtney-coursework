---
title: "week-08"
output: html_document
date: "2023-05-14"
---

a.  **What is a genomic range and what 3 types of information do you need for a range?**

A genomic range is a way to represent regions of a genome. Usually, ranges include the start and end of specific features like genes, exons, or regulatory regions. 3 types of information are needed for a range:

-   Chromosome: The chromosome on which the feature is located.

-   Start position: The position on the chromosome where the feature begins.

-   End position: The position on the chromosome where the feature ends.

b.  **What does 0-based and 1-based refer to? What are the advantages and disadvantages of each?**

0-based refers to a system in which the first base of a sequence is numbered as 0 and the last base's position is the length of the sequence - 1. This is used in Python and BED file format.

1-based is a system in which the first base of a sequence is numbered as 1. This is used commonly GenBank, Ensembl, and R.

Advantages and disadvantages:

-   Initially, 1-based is a more intuitive system because we naturally count the first element of a sequence as 1, so a range defined as 1:5 would include 1,2,3,4 and 5. In contrast, 0-based counts the first element as the 0th place, so if we call the range as 0:5, it would include 0,1,2,3 and 4 (not 5).

-   advantage of 0-based: more intuitive for counting the length of the range: end base - first base.

-   disadvantage of 1-based: to calculate length of a range, need to add 1 to end base - first base (unintuitive)

-   advantage of 0-based: supports zero-width features, whereas with a 1-based system the smallest supported width is 1 base. Zero-width features are useful for representing features between bases.

The distinction between 1-based and 0-based is important because it can lead to off-by-one errors if not accounted for.

b.  **What is the value of BEDtools over the bioconductor package GenomicRange?**

While GenomicRange allows us to work more interactively with range data, it requires loading large amounts of data into memory at once, which can be time-consuming. Instead, BEDtools a command line tool that makes it easier to quickly analyze lots of data. 

c.  **Describe one subcommand of the BEDtools suite as well as a practical use case.**

bedtools sort is a useful tool to set up our analysis because some subcommands, like genomecov, required a sorted input. This sorts a BED file by chromosome and then by start position:  

bedtools sort -i input.BED 
