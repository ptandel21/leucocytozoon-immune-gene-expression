# Barn Owl Immune Gene Expression – BIOL 710 GitHub Assignment

This project builds on a previously published RNA-seq dataset analyzing immune responses in wild barn owls (*Tyto alba*) infected with the blood parasite *Leucocytozoon*. The original study (by Caroline Faircloth) identified differentially expressed genes in owls co-infected with *Leucocytozoon* and Matryoshka RNA virus. This project expands her dataset by increasing replicates, focusing on gene expression patterns in owls infected with *Leucocytozoon* and MaRNAV.

## Project Objectives

- Load and inspect RNA-seq read count data from `.ReadsPerGene.out.tab` STAR output
- Prepare dataset for downstream immune gene analysis and ddPCR primer design
- Validate RNA-seq expression patterns for genes like **HEBP1**, **MAP4K4**, and others
- Build a clean GitHub repository with well-documented dataset and metadata

## Sample Metadata

| Sample ID | Condition  | Age      | Notes                            |
|-----------|------------|----------|----------------------------------|
| LWC142    | Positive   | Juvenile | Minor foot wounds; eye irritation |
| LWC143    | Positive   | Adult    | Minor body wounds; eye irritation |
| LWC153    | Positive   | Juvenile | Fell from nest                   |
| LWC148    | Negative   | Juvenile | Euthanized (fracture)            |
| LWC157    | Negative   | Juvenile | Found in dumpster                |
| LWC162    | Negative   | Juvenile | Found on ground                  |

- “Positive” = *Leucocytozoon*-infected
- “Negative” = uninfected with both parasite and virus (per Caroline’s RT-PCR and RNA-seq screening)

---

## Repository Structure

---

## Notes

This work supports a follow-up ddPCR experiment to quantify expression levels of key immune genes. Genes were selected based on differential expression in Caroline’s paper and relevance to *Leucocytozoon* or *Plasmodium* infection studies in birds.


