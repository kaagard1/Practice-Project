Project 1: Home Credit Kaggle Competion:

Individual Notebook

This project focused on identifying potential customers who lack sufficient credit history for traditional credit approval but are at low risk of defaulting on a loan. The objective was to build a predictive model that improves our ability to accurately distinguish between those who will and will not default. For this exploratory data analysis notebook, I focused on the application and bureau datasets. In the application data, a person’s education level appeared to be a strong predictor of default. The CREDIT_ACTIVE variable from the bureau data also showed potential for improving model performance.

Group Workbook

For group portion of the project, I cleaned and merged the bureau and bureau_balance files into a single dataframe. Additionally, I researched Home Credit’s customer base and business practices in the Philippines, which served as the basis for our revenue projections. Finally, I created the gradient boosting model that we selected as our final solution. It outperformed all other candidate models. This was my first experience working with gradient boosting and the XGBoost library. As a result I learned about how to prevent overfitting by adjusting parameters in the model such as the learning rate, depth and early stopping. Our final model combined the application, bureau, and bureau_balance datasets. This enhancement could enable Home Credit to expand its lending population by 13.6%. One major challenge was dealing with missing data across a large number of predictors, which made it difficult to maintain a sample size large enough to support generalizable predictions. We also had to balance model accuracy with how long it would take to run.

