# BHMLAI-Application17_1

The link to the notebook is: 

Data understanding: The dataset collected is related to 17 campaigns that occurred between May 2008 and November 2010, corresponding to a total of 79354 contacts. During these phone campaigns, an attractive long-term deposit application, with good interest rates, was offered. According to the dataset description the data has already been cleaned at the source. 

Observations on dataset: 
- The dataframe does not have any missing values
- The two classes / labels are very unbalanced.
- We are required to us only the first 7 columns
- There are a lot of categorical features which will require encoding using OneHotEncoder or Label Encoding. The labels will be changed to numeric, '1' for 'yes and '0' for 'no'

Business objective:

Background: There are huge pressures for European banks to increase financial assets. To solve this issue, one adopted strategy is offer attractive long-term deposit applications with good interest rates, specifically by using direct marketing campaigns.
The overall business goal is to increase efficiency of directed campaigns for long-term deposit subscriptions by reducing the number of contacts to do. The goal of this Machine Learning analysis is to find a model that can explain the success of a contact, i.e. if the client subscribes the deposit thus making it a classification problem. Such model can increase campaign efficiency by identifying the main characteristics that affect success, helping in a better management of the available resources (e.g. human effort, phone calls, time) and selection of a high quality and affordable set of potential buying customers.

This application objective:
Find the best model that can tell the bank whether a customer call will produce a new deposit subscription. Do this by comparing the performance of the classifiers k-nearest neighbors, logistic regression, decision trees, and support vector machines.

Conclusions: 

1. The labels in this dataset are very unbalanced, which shows that data collecting was either biased in some ways, or the overall customer true sentiment is that subscribing to a new deposit is not something they want. The unbalanced nature gives limited chances for the models to work well.
2. The data collected through the marketing campaigns is not relevant. More than this, to the campaign-collected data they had to add extra attributes from internal bank databases.
3. The task limited the features to the first 7 columns which represent core bank customer data. This has influence on the models performance.
4. The best model for the task of classifying the customers, with a chance of classifying on both labels, is the Decision Tree Classifier.
5. AUC has been used as the principal performance criteria. All models performed better than the baseline, which in itself is a good thing
6. The machine time for fitting the models is significant and Grid Searching is a very time-costly process. However, the actual fit time of just a tuned model is reasonable.

Overall conclusion: Unable to produce a truly useful model which can be used for classifying the customers.

Next steps:
1. What can be done to improve the models:
	- include all the features from the original full dataset and redo the
	- manually remove rows to balance the labels
	- include all the available hyper-parameters fora each model, using large ranges for the parameter values.
	- refine the encoding of the categorical data
	- use only a few features, such as 'default', 'education', 'job'
2. What to advise the bank regarding future campaigns?
	- change the data collected, since the existing data is not very useful for predicting customer decision
	- change the offer to something different, a better and more attractive banking product




 
