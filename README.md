# Barn Owl Immune Gene Expression in Leucocytozoon Infection – BIOL 710 GitHub Assignment

This project builds on a previously published RNA-seq dataset analyzing immune responses in wild barn owls (*Tyto alba*) infected with the blood parasite *Leucocytozoon*. The original study (by Caroline Faircloth) identified differentially expressed genes in owls co-infected with *Leucocytozoon* and Matryoshka RNA virus. This project expands her dataset by increasing replicates, focusing on gene expression patterns in owls infected with *Leucocytozoon* and MaRNAV.

## Project Objectives

- Load and inspect RNA-seq read count data from `.ReadsPerGene.out.tab` STAR output
- Prepare dataset for downstream immune gene analysis and ddPCR primer design
- Validate RNA-seq expression patterns for genes like **HEBP1**, **MAP4K4**, and others
- Build a clean GitHub repository with well-documented dataset and metadata

## Introduction

Malaria is one of the most widespread parasitic diseases, affecting over 263 million people and causing 597,000 deaths globally in 2023 [1,2]. Malaria is caused by Plasmodium parasites, which belong to the order Haemosporidia — a group that also includes avian parasites such as Leucocytozoon. These parasites can cause significant disease in birds, triggering immune responses, anemia, and in some cases, population decline [3].

While Plasmodium and Haemoproteus parasites are well-studied, Leucocytozoon remains underexplored, especially regarding how it interacts with other biological agents like viruses. In 2019, researchers discovered a new group of RNA viruses that infect protozoan parasites — Matryoshka RNA viruses (MaRNAVs), named for the "nested doll" concept of viruses within parasites within hosts [4]. These viruses include MaRNAV-1 (discovered in Plasmodium vivax), and later MaRNAV-2 through MaRNAV-6, identified in avian hosts infected with Leucocytozoon or Haemoproteus [5,6].

Co-infections like these may influence parasite behavior and host immune response, but the biological significance of MaRNAVs is still unknown. In avian malaria systems, understanding these interactions could provide valuable insights into immune evolution and disease outcomes.

In an earlier study by Caroline Faircloth, RNA-seq analysis of barn owls (Tyto alba) identified genes that were differentially expressed in owls infected with both Leucocytozoon and MaRNAV. However, the dataset was limited to six individuals.

To build on this foundational work, this project focuses on expanding the dataset by adding more Leucocytozoon-infected barn owls and analyzing expression of a small number of key immune genes for validation.

## Research Question

Which immune-related genes are upregulated in barn owls infected with Leucocytozoon, and can we strengthen RNA-seq results through replication and ddPCR validation?

### Aims

Aim 1: Expand the Dataset
Increase the number of barn owl samples infected with Leucocytozoon, building on the original RNA-seq study. This improves statistical power and robustness of observed gene expression differences.

Aim 2: Focus on Key Immune Genes
Analyze expression levels of a small number of immune-related genes such as HEBP1, MAP4K4, TLR7, IFNG identified in prior work. Prepare for downstream ddPCR validation of these genes in additional owl samples.

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

## References

1. Ferraboli JW, Veiga GTS da, Albrecht L. Plasmodium vivax transcriptomics: What is new? Exp Biol Med. 2023;248(19):1645. doi:10.1177/15353702231198070

2. Fact sheet about malaria. Accessed March 7, 2025. https://www.who.int/news-room/fact-sheets/detail/malaria

3. Valkiūnas G. Avian Malaria Parasites and Other Haemosporidia. CRC Press; 2005.

4. Rodrigues JR, Roy SW, Sehgal RNM. Novel RNA viruses associated with avian haemosporidian parasites. PloS One. 2022;17(6):e0269881. doi:10.1371/journal.pone.0269881

5. Petrone ME, Charon J, Grigg MJ, et al. A virus associated with the zoonotic pathogen Plasmodium knowlesi causing human malaria is a member of a diverse and unclassified viral taxon. Published online September 19, 2024. doi:10.1101/2024.09.18.613759

6. Duc M, Esperanza C, Chagas CRF, Iezhova T, Sehgal RNM, Valkiūnas G. First report of Matryoshka RNA virus in an African-European migrant bird. PLOS ONE. 2025;20(3):e0319395. doi:10.1371/journal.pone.0319395

7. Outlaw DC, Walstrom VW, Bodden HN, Hsu C Yu, Arick M, Peterson DG. Molecular evolution in immune genes across the avian tree of life. Parasitol Open. 2019;5:e3363. doi:10.1017/pao.2019.33


