Credit Card Fraud Detection

Data (as pickle file) can be found at [google drive folder](https://drive.google.com/drive/u/1/folders/1yw2Y3cxsSXTgbTJg5nSaLs2cwNSPhWXl). All data are publicly available and are referred in the code as `pd.read_pickle(URL)`. 
 
The project has three parts: 
- EDA and Data Engineering: `data-mining-EDA-data cleaning-imputation.ipynb` under the `DataEngineering` folder is the main roadmap notebook with detailed comment of our thought process; `EDA_Fraud_Detection_transaction-2.ipynb` is other EDA procedures we took 
- Dimensionality Reduction and Upsampling: `step2_comb.ipynb` under the `DimensionReduction` folder incorporates the steps we took as remedy to high dimensionality (PCA and autoencoder) and class imbalance (SMOTE), the other files in the folder are other things we tried
- Model Development and Evaluation: under the `Modeling` folder, you can find both supervised approaches (`Random_Forest.ipynb`, `XGBoost.ipynb` and `old_MLP.ipynb` for random forest, XGBoost, neural network, respectively) and unsupervised approach (`k_means.ipynb`, `LOF.ipynb`, `IsolationForest.ipynb` for k-means, local outlier factor and isolation forest, respectively). Each file uses 3-fold cross-validation grid search with 3 repetitions to find the best hyperparameters, the best model fitted using these parameters, and the final test AUC, FPR, FNR.

You can also find the final report (including all literature reviewed) and slide deck. 
