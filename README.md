**Project 1: Home Credit Kaggle Competion:** 

***Summary of Business Problem and Project Objective***

Home Default Credit Risk needs to identify potential customers who lack sufficient credit history for traditional credit approval but are at low risk of becoming delinquent on a loan. This can be accomplished by using alternative data sources, such as telecommunications data and transactional history. Home Default Credit Risk primarily operates in countries where potential customers use mobile phones, rather than computers, to conduct most of their economic activities.

The goal of this project is to harness this transactional data and create a model that improves the ability to predict default for the unbanked community, who lack sufficient credit to be approved by traditional means.

**Solution to the Problem***

Our group used data from the bureau.csv and bureau_balance.csv files, which captured customers’ transaction behaviors, to supplement Home Credit’s application data. We first created a model using only the application data to serve as a baseline for comparison. Our new model incorporated the transactional data, which increased its AUC (Area Under the Curve) performance from 0.70 (baseline) to 0.75.

**My Contribution**

I cleaned and merged the bureau.csv and bureau_balance.csv files into a joined data frame that we used for the new model. I also created the gradient boosting model that we selected as our final solution, which outperformed all other candidate models. Additionally, I conducted research into Home Credit’s customer base and business practices in the Philippines, which we included in our presentation.

For the exploratory data analysis notebook, I focused on the application and bureau datasets. In the application data, education level appeared to be a strong predictor of default. The CREDIT_ACTIVE variable from the bureau data also showed potential for improving model performance.

**Business Value**

Home Credit’s application data includes three external credit scores, which are strong predictors of potential default. However, 13.6% of applicants had only two or fewer of these scores available. Our model enables Home Credit to extend credit to a larger portion of this population by supplementing missing credit information with alternative data sources.

**Difficulties Encountered**

This was our first time working with such a large dataset that had not already been cleaned. As a result, getting the data ready for modeling took a lot of time and effort. Due to the large volume of data, we had to balance potential model performance against the time it took for models to run.

The target variable was very imbalanced: 92% of customers did not default. To address this, we adjusted the training split to 80/20, ensuring that the model had more default cases to learn from.

Our gradient boosting model initially had a strong tendency to overfit the training data, so we made several adjustments to help it generalize better to the test data.

**What I Learned**

This was my first experience working with gradient boosting and the XGBoost library. I learned how to improve a model’s ability to generalize and prevent overfitting by experimenting with techniques such as adjusting tree depth, using early stopping, tuning the learning rate, applying regularization, and enabling parallel processing. 

Additionally, this was my first experience working as part of a team on a larger data project. I learned a lot about collaboration, problem-solving, and sharing responsibilities in a team setting in a data science environment.
