# Machine Learning for Predicting Cancer Drug Sensitivity

## Authors (@slack) :

* Chamss Daghsni (@ChamssDaghsni)  
* Alle Manideep (@Manideep) 

## Link to The Project script

## Background

Machine learning has evolved to be a potent tool in cancer drug discovery, offering novel ways of predicting cancer cell sensitivity to drugs. The paper "Machine Learning Prediction of Cancer Cell Sensitivity to Drugs Based on Genomic and Chemical Properties" describes ML models that integrate genomic data with drug properties for the prediction of the efficacy of a certain drug. It deals with cancer treatment's complexity by identifying which drugs are more effective on certain cell lines of cancers.

With ML, large datasets yield patterns that give insight into the behavior of cancer. Regression and classification algorithms predict drug sensitivity by mapping drug response relations to genomic alterations, hence enabling personalized therapies. Eventually, ML in cancer drug discovery accelerates identification and decreases costs and time. It has the potential to optimize treatment options by predicting patient response and opening ways to more targeted and effective therapies for cancer.

## Methodology

The dataset was prepared by encoding genomic information and chemical properties onto 827 features by the researchers. The authors used 8-fold cross-validation, partitioning the data into eight parts with no overlap to enable robust training and testing of the model. Hyperparameter tuning resulted in optimal performance for the neural networks. They have further estimated the performance of random forest models with the intention of comparing the performances using an alternative machine learning approach. This broad methodology allowed for correct predictions of cancer cell sensitivity to drugs, hence improving the treatment responses' understanding. 

## Results

The model's performance was checked using cross-validation. The average MAE for the models stood at 2.01, while RMSE was 2.54 and R²  0.0373, with about 9.81% variance of the predicted drug sensitivity. A scatter plot comparing the predicted vs. actual values yielded a correlation coefficient of 0.3257, hence some positive correlation, although the model is limited.

![image](https://github.com/user-attachments/assets/b808673c-e5bc-4400-a103-a0bd6de8b708)

***Figure 1:** Scatter Plot of Actual vs. Predicted LN\_IC50 Values*

## Comparison of Findings

This model performed worse compared to the model of Menden et al., which had an R² of 0.72 in cross-validation. The likely reason for this performance difference was that genomic features providing better accuracy for Menden's analysis were absent.

## Conclusion and Insights

The study highlights the capability of machine learning in predicting cancer drug sensitivity. The model returned a positive correlation between the predicted and actual values; however, the R² value remains low, thus leaving much space for improvement. Even with modest results, the study depicts the importance of predictive modeling for the advance of drug discovery.

