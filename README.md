**Ryerson University Data Analytics Final Project by Jessica Du**
__________________________________________________________________
By: Jessica Du x5du@ryerson.ca
Supervisor : Dr. Tamer Abdou tamer.abdou@ryerson.ca

The dataset used for this project:
https://www.kaggle.com/mlg-ulb/creditcardfraud

**Problem Statement**

The problem statement chosen for this project is to determine which machine learning algorithms can help determine abnormal transactions?
And how effictive is each system given that the dataset is highly imbalance. As well as, comparing each approach applied to the dataset.

In this capstone project, we will analyze customer level data collected analyzed during a research collaboration of Worldline and the
Machine learning Group of ULB.

The dataset was taken from Kaggle.com an online community for data analyst, where it contain a total of 284,807 transaction where only 492
are fraudulents resulting in a highly imbalance dataset.

**Data Dictionary**
The dataset contains transaction made by European credit cards holder in September 2013. This dataset present transaction that occurred in two
days, out of the 284,807 transactions, only 492 transaction were considered as fraud. This result in a highly unbalanced dataset, causing the 
positive class(frauds) only accounting for 0.172$ of all transactions. The dataset has already been Principle Component Analysis (PCA)
transformed to main confidenitality. The only features that have not been transformed are "Amount" and "Time" while all other features
such as (V1, V2, V3 ,... V28) are already transformed. "Time" contains the seconds elapsed between each transaction and the first transaction in
the dataset. The "Amount" feature is the total transaction amount. The feature "Class" is the response variabel, where it takes the value of 1 
as fraud and 0 as others.

**Project Pipline**
The project outline can be summarized in the following four steps:
- **Data Understanding**: In this following step, the dataset is loaded into Google Colab to understand features presented in it. This would help
determine which features to keep for the final model.

- **Exploratory Data Analytics(EDA)**: Since, the feature data set already contains Gaussian variables, Z-scaling was not necessary. However, the skewness
in the data was analyze and mitigated to improve accuracy and minimize problems during model building.

- **Train/Test Split**: The dataset was split into 70% training set and 30% testing set. For validation, K fold corss validation method was performed.
A k value of 5 was chosen for this project

- **Model-Building/Hyperparameter Tuning**: The final step of the project, where the given dataset was inputed into given selected mdoels. Each
model was tune to the desire hyperpapmeters until we get the desire level of performance. In addition, the dataset was also transformed by using
various of sampling techniques to obtain better results from each model.
