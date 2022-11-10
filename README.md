# **Predicting the death by cancer rate for US counties** – Simon Kennedy

## Abstract
Four regression based models were built to predict the death rate from cancer for US counties. The original data was cleaned and pre-processed to prepare and improve the data for the modelling process. The model candidates are 1. Linear model with SGD Regressor, 2. Support Vector Machine for regression(SVR), 3. Random Forest Regressor, 4. Neuronal Network model. The data was split into training and testing sets. Following initial fitting, hyperparameter tuning was performed using K fold cross validation. The models were evaluated with all models outperforming the baseline. Hyperparameter tuning improved model accuracy in all but the Random Forest Regressor. Principal Component Analysis(PCA) improved the SVR model. The Neuronal Network model was the best performing model on this data and was saved for future use.

See the report for further details.

## Conclusion
All of the four models evaluated were more accurate at predicting the mean death rate by cancer in US counties than the mean baseline. The Support Vector Machine Regressor responded very well to hyperparameter tuning and also mildly to Principal Component Analysis. The Random Forest model has some issues with under or over fitting and may be better trained with a cross validated dataset. The Multi Layer Perceptron Neuronal Network model (model 4) was the best suited model to the high dimensional data of approx. 3000 instances demonstrating an RMSE of 18.37 mean deaths per 100, 000 population for a US county. This model has been saved for future use.
Some limitations of the project were the data having high dimensionality, collinearity and low target correlation. Approximately 3000 rows may have impacted the Random Forest variance in results for train compared to test. Further improvement in performance could be achieved by tuning or trialling different normalisation methods.
