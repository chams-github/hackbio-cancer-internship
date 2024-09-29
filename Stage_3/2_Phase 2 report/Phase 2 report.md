<!--StartFragment-->

# Building a ML model to predict the IC50

## Authors (@slack) :

- Chamss Daghsni (@ChamssDaghsni)

- Alle Manideep (@Manideep) 

## Link to [The project script](https://github.com/chams-github/hackbio-cancer-internship/blob/main/Stage_3/Phase%202%20Script/phase2%20script.ipynb) 

## Introduction

The goal of this phase was to develop a machine learning model able to predict the bioactivity of compounds against S100A16-a protein associated with poor prognosis in lung cancer. S100A16 is crucial in the proliferation, migration, and invasion processes of cancer cells and thus serves as an important target for therapeutic development. Bioactivity data in terms of IC50 values of compounds were used in conjunction with calculated molecular descriptors using cheminformatics libraries to train predictive models.

## Dataset and Preprocessing

Dataset was downloaded from the ChEMBL database, focusing on the compounds having IC50 values specific to S100A16. The steps involved in preprocessing are as follows:

- Data Cleaning: Only invalid or missing values for IC50 and duplicate entries were removed.

- Calculation of Molecular Descriptor: Calculation of more than 200 kinds of molecular descriptors of each compound with RDKit and other molecular weight, LogP, hydrogen bond donors, and acceptors.

- The log transformation to pIC50: done for normalization of distribution for the IC50 values.

This was further divided into 80% for training and 20% for testing.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdoPdDkyQnJyVR08IBhUjYeOUVcLQtXnhp8_-012fCyVTgPfkDqWYNLXlKwSFmVd3CkNcBDZCzq9mtbCweGYLVrpFdJqqTkPae4QOh5Otf-Bw-ZF262KTxEUNZdmVNCBqwIou_9x0H92X2sIVT_4rsMjNZZ?key=nH1WlKwfNEqCTNX4I8rkhg)

**_Figure 1:_** _Summary Statistics of pIC50 Values after Transformation_

__![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeyqJviSX29RzNuI5lJT7_3yF0MPD3hu2FHxWxRW39c8MdTIdbEASQaS0M0N6NDknKGFmmWwlfFcfqGXGLOvFAsSn2Y3s6wyovkVCUE9xDY13sgoFg0OjETGQiyZl2h60xrf68GVFhhIW98D_bO8YwPbm-8?key=nH1WlKwfNEqCTNX4I8rkhg)__

**_Figure 2:_** _Distribution of Compounds by Bioactivity Class_

__![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdZOtQrbnFZZAqW_yc-KXbLwM-OaQL4CpHK6rvYbIM-CH1CckxJmNx0tu75GN-529z1IJqxScLBdfHdtZfvjMW-JzhDcXAmK7TJxRm7gxkTUzHfIaRwE3Be4QUCMzdzHUVxdOnDC6udw22Wy5auxrflyGor?key=nH1WlKwfNEqCTNX4I8rkhg)__

**_Figure 3:_** _Scatter Plot of Molecular Weight (MW) vs. LogP Colored by Bioactivity Class and pIC50_ 

## Model Development and Training

Because of the nature of the pIC50 values, the complex nonlinear relationships between molecular descriptors and their activities are supposed to be utilized by a Random Forest Regressor. The model was trained on molecular descriptors and pIC50 values and performance improvements were done by tuning the model and doing a default grid search over different parameters. Cross-validation was used to assess generalizability.

Overall, the key metrics were:

- Mean Squared Error (MSE): 0.154

- Mean Absolute Error (MAE): 0.313

- R-squared (R²): 0.356

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf2oBoiomkqjX2qaYgWyPM8BfSUtWo-vvLwyonzeTsUeH5IZHb7nfpjHFJ9SfycybBo0A6XleGMGGs6phnjrq3xaWKIhKRkgOIPaFCs13WYWJUFl1MzrfOeBUBFASHrzjzjAJTkFaFusw8UB7PqmZHivxo?key=nH1WlKwfNEqCTNX4I8rkhg)

**_Figure 4:_** _Predicted Values for the two ligands Predicted pIC50 Values for Ligands Zingiberene and Zerumbone Using the Random Forest Model_

## Results and Feature Importance

The metrics for the predictions of the ligands Zingiberene and Zerumbone were as follows:

- MSE (Ligands): 0.28

- MAE (Ligands): 0.49

- R-squared (Ligands): 0.74

The model's performance on the docked ligands was higher compared to the ChEMBL data, where higher predictive accuracy is observed for ligands. The feature importance analysis post-modeling indicated that LogP and Molecular Weight were the most influencing descriptors on bioactivity:

- LogP: Permeability and binding affinity

- Molecular Weight: Better activity of moderately sized compounds due to target engagement.

## Conclusion

This model demonstrated moderate predictive power for bioactivity against S100A16. While performing better in the case of docked ligands, the fit was weaker in the case of the ChEMBL dataset. Further improvements will most likely consider refinement of feature selection, the probing of alternative algorithms, and the expansion of datasets for more significant accuracy and generalization.

<!--EndFragment-->


<!--EndFragment-->
