# Dataset Card – Barn Owl Gene Expression

## Dataset Summary

This dataset contains raw gene expression counts derived from RNA-seq reads aligned to the barn owl reference genome (GCF_000687205.1). Read counts were extracted using STAR aligner (`ReadsPerGene.out.tab`), and six barn owl samples were merged into a single matrix.

Some individuals were infected with *Leucocytozoon* parasites. All the birds included in this merged matrix were positive for MaRNAV, Matryoshka RNA virus within the Leucocytozoon parasite, based on follow-up RT-PCR screening. This makes the dataset ideal for parasite and virus co-infection immune response analysis.

---

## Dataset Structure

- Format: `.csv`
- Rows: Genes (n = 18,892)
- Columns: 6 owl samples + `GeneID`

### ➕ Data Fields

| Column    | Description                                      |
|-----------|--------------------------------------------------|
| GeneID    | Barn owl gene symbol or LOC ID                   |
| LWC142    | Raw unstranded read counts (infected, juvenile)  |
| LWC143    | Infected, adult                                  |
| LWC153    | Infected, juvenile                               |
| LWC148    | Uninfected, juvenile                             |
| LWC157    | Uninfected, juvenile                             |
| LWC162    | Uninfected, juvenile                             |

---

## Supported Tasks

- RNA-seq differential expression analysis
- Immune gene screening
- ddPCR primer design validation
- Comparative immune transcriptomics

---

##  Source

- Folder: `/CFaircloth/BANO/reads_per_gene/`
- Merged manually on trypsin.sfsu.edu using custom R script
- Based on `.ReadsPerGene.out.tab` files from STAR alignment

---

## Curation Rationale

This dataset builds directly on a prior RNA-seq study by Caroline Faircloth, which identified differentially expressed immune genes in barn owls infected with *Leucocytozoon*. The purpose of this dataset is to increase the number of replicates and focus on a small subset of key immune-related genes such as HEBP1, MAP4K4 for further validation.

By expanding the dataset and focusing on genes of interest, this project helps strengthen the original study and prepares it for downstream ddPCR validation and publication.


---

##  Licensing & Usage

- For academic and educational purposes only
- Do not distribute without PI permission

---

##  Citation

Unpublished RNA-seq dataset expanded and curated by Pinkal Tandel, based on original analysis by Caroline Faircloth and Ravinder Sehgal. Prepared for BIOL 710 (Spring 2025), San Francisco State University.

