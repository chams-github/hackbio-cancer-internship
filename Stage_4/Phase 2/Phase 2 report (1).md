# Molecular docking of Histone deacetylases subtypes.
## Authors (@slack) :
 Alle Manideep(@Manideep)
 
 Chamss Daghsni (@ChamssDaghsni)

## Introduction

Histone deacetylases (HDACs) are enzymes involved in chromatin remodeling through the removal of acetyl groups from histones, leading to condensed chromatin and reduced gene transcription. Their role in silencing tumor suppressor genes has made them important drug targets for cancer therapy. Dysregulation or overexpression of HDACs is frequently observed in various cancers, promoting uncontrolled cell growth and tumor progression.

HDACs are divided into four classes, with class I, II, and IV enzymes being zinc-dependent. Among them, HDAC11, the sole member of class IV, is increasingly recognized for its involvement in cancer and other diseases. HDAC11’s unique biological functions make it a particularly attractive target for selective inhibition, which could lead to more precise cancer treatments with fewer off-target effects.

Several selective HDAC11 inhibitors, such as FT895 and SIS17, have been developed and shown efficacy in reducing cancer cell viability, particularly in non-small cell lung cancer. Although the absence of a crystal structure for HDAC11 complicates drug design, AI-driven approaches like AlphaFold have enabled the prediction of HDAC11’s structure. These models have been used successfully in virtual screening and structure-based design, making HDAC11 a promising target for future anticancer therapies.

## Methodology
## proteins preparation
The proteins HDAC1,HDAC2,HDAC3,HDAC4,HDAC5,HDAC6,HDAC7,HDAC8,HDAC9,HDAC10 structures downloded from PDB data base and the HDAC11 protein structure modeled using the Alphafold. Cleaning of the protein structure was done using PyMOL by removing water molecules together with bound ligands/hetero atoms. Hydrogens were thereafter added to the structure.
Changes were finally added to the protein with the help of tools available in PyMOL to ensure proper molecular interactions.

## ligands library preparation
The 50 phytochemical of turmeric and 11 inhibitors of 11 HDAC's one for each according to the literature, Total of 61 lignads are downloaded from Pubchem in SDF format. The energy minimization of all 61 ligands was done using PyRx and after that the structures of protein and ligand were converted to the pdbqt format for docking.

## Molecular Docking
The docking were conducted with the aid of a grid box laid over the active site, creating multiple binding modes for each ligand in the PyRx.To enhance reliability, docking simulations were performed in triplicate for each protein-ligand pair, with binding affinities (docking scores) calculated. The mean and standard deviation of the results were then computed to identify the ligands that demonstrated the strongest and most consistent binding affinities for each HDAC subtype.

## Results
| HDAC Subtype | PDB ID | Ligands with Highest Affinity (CID) | Mean of the Binding Affinity (kcal/mol) | Standard deviation |
|--------------|--------|-------------------------------------|-----------------------------------------|--------------------|
| HDAC1        | 4bkx   | 53344908                            | -8.5                                    | 0                  |
| HDAC2        | 4lxz   | 67324851                            | -5.9                                    | 0                  |
| HDAC3        | 4a69   | 53344908                            | -8.9                                    | 0                  |
| HDAC4        | 5zop   | 6654                                | -5                                      | 0                  |
| HDAC5        | 5uwi   | 67324851                            | -9.5                                    | 0                  |
| HDAC6        | 3phd   | 67324851                            | -9.1                                    | 0                  |
| HDAC7        | 3znr   | 53344908                            | -8.3                                    | 0                  |
| HDAC8        | 2v5x   | 53344908                            | -11.5                                   | 0                  |
| HDAC9        | 8Q9R   | 67324851                            | -7.8                                    | 0                  |
| HDAC10       | 7SGG   | 53344908                            | -10.1                                   | 0                  |
| HDAC11       |        | 53344908                            | -8.53                                   | 0                  |

Table1: Molecular Docking Analysis of HDAC Subtypes.

The docking analysis revealed 53344908 and 67324851 as top ligands, with high affinity for multiple subtypes.
53344908 exhibited the strongest binding to HDAC8 and showed consistent interactions across HDAC1, HDAC3, HDAC7, HDAC10, and HDAC11. 67324851 demonstrated high affinity for HDAC2, HDAC5, HDAC6, and HDAC9. No standard deviation, which indicated the stable binding of ligands in all triple docking.

## Comparating Binding Affinities of Compounds Across HDAC Subtypes
![download (1)](https://github.com/user-attachments/assets/372a7dc6-dba0-444c-8950-56460fa5857e)
Figure1: HDAC Binding Affinity Heatmap

## Conclusion
TMP269 exhibits a binding affinity for HDAC11 comparable to FT895, but its broader affinity profile makes it a versatile inhibitor for cancer therapy. With strong interactions across multiple HDACs, TMP269 can target a wider range of HDAC-driven oncogenic pathways. The low standard deviation in docking simulations indicates robust binding, positioning TMP269 as a promising candidate for future therapeutic development in cancer treatment.

## Reference
Baselious, F., Hilscher, S., Hagemann, S., Tripathee, S., Robaa, D., Barinka, C., ... & Sippl, W. (2024). Utilization of an optimized AlphaFold protein model for structure‐based design of a selective HDAC11 inhibitor with anti‐neuroblastoma activity. Archiv der Pharmazie, e2400486.











 
