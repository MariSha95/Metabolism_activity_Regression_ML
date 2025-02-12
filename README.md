# Metabolism_activity_Regression_ML

Dataset METAB_training_disguised.csv is taken from https://www.kaggle.com/datasets/vivek153/data-root?select=METAB_training_disguised.csv (QSAR-data for Drug Discovery).

Quantitative structure−activity relationships (QSAR) is a very commonly used technique in the pharmaceutical industry for predicting on-target and off-target activities. Such predictions help prioritize the experiments during the drug discovery process and, it is hoped, will substantially reduce the experimental work that needs to be done.

The data is based on  10,000 compounds for each target. Each row of the data corresponds to a compound and contains descriptors ( D36-D1073) derived from that compound’s chemical structure. Activity between the target molecule and each compound is provided in the training data.	

Jupyter notebook presents presentation of the dataset and 5 ML algorithms for the regression analysis with hyperparameters selection. Best hyperparameters and quality metrics for each models are the following:


XGBoost Regressor :

Best parameters: {'colsample_bytree': 1.0, 'learning_rate': 0.05, 'max_depth': 5, 'n_estimators': 200, 'subsample': 0.8}

MAE: 0.14570767305734436

MSE: 0.0912853515488276

R²: 0.9999352216709442




Random Forest 

Best parameters: { n_estimators=200, max_depth=30,  min_samples_split=2,min_samples_leaf=4)

MAE: 0.096429653104992

MSE: 0.06499025510018563

R²: 0.9999538813176608




LGBM (without hyperparameters fitting):

MAE: 0.17809273457184246

MSE: 0.3221985108185801

R²: 0.9997713600177798




KNN 

Best parameters: {'metric': 'euclidean', 'n_neighbors': 9, 'weights': 'distance'}

MAE: 16.3731210025737

MSE: 456.5259181746757

R^2 Score: 0.6760379880424678 





Elastic Net 

Best parameters: {'alpha': 0.5, 'l1_ratio': 0.1}

MAE: 17.4338646220917

MSE: 479.0379982297341

R^2 Score: 0.6600628627371061
