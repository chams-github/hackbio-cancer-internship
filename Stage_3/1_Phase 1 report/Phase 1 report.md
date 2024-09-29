<!--StartFragment-->

# Virtual screening by Molecular docking of anti-cancer activity of turmeric phytochemicals compounds that target S100A16 on patients with lung cancer

## Authors (@slack) :

- Chamss Daghsni (@ChamssDaghsni)

- Alle Manideep (@Manideep) 

## Introduction:

In spite of limited treatment options and poor survival rates, lung cancer remains one of the most lethal cancers worldwide. Recently, S100A16 has appeared as a potential target for therapy because it is highly expressed in lung adenocarcinoma (LUAD) and  it is associated with poor prognosis. Because S100A16 participates in promoting tumor progression, targeting S100A16 has become one of the most promising ways of therapeutic interference against lung cancer.

Meanwhile, phytoconstituents from natural sources, like turmeric Curcuma longa, have been identified to possess anti-cancer properties. The  work aimed at virtual screening and molecular docking studies in the quest for potential turmeric phytochemicals that might inhibit S100A16 and thus possibly lead to the discovery of new phyto-pharmacological interventions against lung cancer.

## Phytochemical libraries:

A library of 50 phytochemicals from turmeric was curated. Complete details of these phytochemicals were documented. This library would be useful in the next step of molecular docking by providing a set of phytochemicals with their structures for the interaction analysis.

## Protein preparation:

A protein structure with PDB ID 3NXA, which corresponds to S100 calcium binding protein A16(S100A16), was selected as the target for docking analysis.

Cleaning of the protein structure was done using PyMOL by removing water molecules together with bound ligands/hetero atoms. Hydrogens were thereafter added to the structure.

Changes were finally added to the protein with the help of tools available in PyMOL to ensure proper molecular interactions.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcrY8POJuNd7UNaSmuTPFTMxacc2Luv62Z5KPqKCN4OZskRGCV3FyVfc4kOMKnEuY_HY7BTiPVbN-AD-_ixYaiRuYgJgD9V0pyisRtY2m9ik-lCJ8hORaB1RHsgCZVLSqCgJtAMS96cZMiGkW8UU_hLuj42?key=sPTx3fOf_JHU4MjjphSNgA)

**_Figure 1:_** _3NXA Protein Structure Prepared for Molecular Docking in PyMOL_

 CASTp is used to obtain active sites for 3NXA.

**_Table 1:_** _Active Site Characteristics of 3NXA for Molecular Docking_

|    **Parameter**    |            **Value**            |
| :-----------------: | :-----------------------------: |
|   **Active site**   |             Pocket 1            |
|  **Binding sites**  |   572 205 410 133 149 144 204   |
|     **Receptor**    |            3NXA.pdbqt           |
|  **Exhaustiveness** |                8                |
| **Grid Box Center** | X: 3,4100 Y: 58,7302 Z: 30,5230 |
|  **Grid Box Size**  |    X: 87,7549 Y: 76,7914 Z: 25  |

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeIxCUHfZNMoth9EyfiasFD0FC9XKPE-KnSe0KYW7bqOd6sLfZAOTVdV1QL5aHVU2UE8fjUjTxBfGA1bXj0Xv5Gocpts22rLd-urvfumhlXsyFmD3AfuTVrKzaevt8PQ68xcDDOPyzzffzuyIs1YfZLLc4?key=sPTx3fOf_JHU4MjjphSNgA)

**_Figure 2:_** _Crystal Structure of 3NXA Highlighting the Most Active Binding Pocket_

## Molecular Docking of Turmeric Compounds against S100A16

The energy minimization of the 50 curated turmeric compounds was done using PyRx and after that the structures of protein and ligand were converted to the pdbqt format for docking.

Simulations of docking were conducted with the aid of a grid box laid over the active site, creating multiple binding modes for each ligand.

The binding affinity analysis revealed 3 turmeric compounds with the top binding affinities to 3NXA.

**_Table2:_** _Binding Affinity Results of Top Three Turmeric Phytochemicals Docked to 3NXA_

| **Ligand**                        | **Binding Affinity** | **rmsd/ub** | **rmsd/lb** |
| --------------------------------- | -------------------- | ----------- | ----------- |
| Terpecurcumin A (3nxa\_71457832)  | -7.9                 | 0           | 0           |
| Terpecurcumin B (3nxa\_71459743)  | -7.6                 | 0           | 0           |
| Dehydrodeguelin (3nxa\_3083803)   | -7.5                 | 8.08        | 5.626       |

## Visualizations of the protein with the best ligand 

The binding interactions of the top compound, Terpecurcumin A are visualized in PyMOL at the active site of 3NXA.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc2_Jqzd52EbF58A-beZbYkI-FfpZBkJd3n0UybLXkiLNEkFpsodgZPVVQ9vUWXJixJOwYMPNsAn8V4F4MHICYq5kDt9OUMLh3fLJHs8rFDXwXZlgdVvYMZmtZ4lmU1Zm5VihJZm-W-4QHAZ_eRvPey2Z2i?key=sPTx3fOf_JHU4MjjphSNgA)

**_Figure 3:_** _Binding Model of Terpecurcumin A in the Active Site of 3NXA_

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcTR-SFKoiDKHj0ALpAVhCOXHHjT8K7R6b9UXa1QOnLCN28kiEFukQOUWZSACAPdRcUwKDOmW4Y8-tH_1YmT1YEzRq52yf9S7yu9DsFvuS-n_hEE7uhpfDpw-Cbyy7reL7blblqpCmElft_zdcinGt0CemA?key=sPTx3fOf_JHU4MjjphSNgA)

**_Figure 4:_** _Close-Up of Terpecurcumin A Binding Interactions within 3NXA Active Site_

 
## Conclusion 

In conclusion, this study identifies Terpecurcumin A, Terpecurcumin B, and Dehydrodeguelin as the turmeric-derived compounds showing high binding affinity with S100A16 and, therefore, stand as potential therapeutic candidates for lung cancer treatment. This work also provides a reusable pipeline of protein-ligand docking analysis for further research in molecular docking studies of cancer therapy.

<!--EndFragment-->

<!--EndFragment-->
