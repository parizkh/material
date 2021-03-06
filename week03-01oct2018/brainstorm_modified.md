
# Part 1 - Brainstorm: Statistics

## Distributions
## Statistical Models
## Methods for Estimation
## Methods for Hypothesis Testing

# Part 2 - Brainstorm: Technologies in Biology

## Microarray
## ...

## In-class exercise 1 (15 minutes)

### Technologies: 

```{r}
techs <- c("microarray", "rna-seq", "dna-seq", 
           "bisulphite-seq", "cytometry", "mass-spec", 
           "10x-chromium", "oxford-nanopore")

s <- sample(length(techs))
data.frame(row=s, techs)
```

### Task: 
#### produce a 2-3 point summary of "how it works"
#### links to a few (<5) good resources
#### create a markdown file for it and upload to README.me in "group assignment" repo

# Part 3 - Brainstorm: Applications in genomics 

# Part 4 - Brainstorm: Linking Technologies to Applications to Statistics

## e.g., microarray -> gene expression -> normally distributed (log intensities)

# Part 5 - Brainstorm: Methods/algorithms in genomics associated to Computer Science

# Part 6 - Pick a "technology" (from above, from [1] or otherwise) to briefly describe

## Exercise 2 (in groups of 1-3): 
### Goal: 
#### write ~2 sentences about what the method does
#### again, make the link (technology -> application -> statistics)
#### list the github usernames of everyone in your group
#### submit a pull request to brainstorm_modified.md

[1] [https://liorpachter.wordpress.com/seq/](https://liorpachter.wordpress.com/seq/)


### ChiRP-Seq
#### Group members: 
parizkh: Hana Parizkova

mkuijs: Merel Kuijs

lbourguignon : Lucie Bourguignon

#### Technology

Researchers treat cells containing the RNA molecule of interest so as to obtain chromatin segments that will react with the synthetic oligonucleotides designed to bind said RNA molecule. The resulting complexes are captured with streptavidin-labeled magnetic beads and treated with RNAse to isolate the bound DNA molecules. The DNA is sequenced using Next Generation Sequencing and the genomic locations corresponding to the obtained reads are determined.  

#### **Application**

The ChIRP-seq technology is a method of mapping _in vivo_ long noncoding RNA (lncRNA) binding sites genome-wide. Thus, one can study the interaction between RNAs and the chromatin. Just as ChIP-seq permits genome-wide explorations of DNA-proteins sequences, ChIRP-seq studies the "RNA interactome".

#### Statistics
- same as for ChIP-seq

- bimodal distribution (of ChIP/ChIRP-seq tags around the binding site)

- Poisson distribution of tags across genome (under null model), with dynamic parameter lambda

- FDR (False Discovery Rate) estimation

