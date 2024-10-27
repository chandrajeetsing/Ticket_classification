# Ticket_classification
This project designed to automate the classification of customer support tickets utilizing Natural Language Processing (NLP) techniques, Non-Negative Matrix Factorization (NMF), and various Machine Learning (ML) algorithms.
# Problem Statement
For a financial company, customer complaints carry a lot of importance, as they are often an indicator of the shortcomings in their products and services. If these complaints are resolved efficiently in time, they can bring down customer dissatisfaction to a minimum and retain them with stronger loyalty. This also gives them an idea of how to continuously improve their services to attract more customers.

These customer complaints are unstructured text data. So, traditionally, companies need to allocate the task of evaluating and assigning each ticket to the relevant department, which then further gets assigned to a particular support employee. This becomes tedious as the company grows and has a large customer base.

In this case study, I will be working as an NLP engineer for a financial company that wants to automate its customer support ticket system. As a financial company, the firm has many products and services, such as credit cards, banking and mortgages/loans. So, need to build a model that is able to classify customer complaints based on the products/services. By doing so, company can segregate these tickets into their relevant categories and, therefore, help in the quick resolution of the issue.

# Text Preprocessing
Before analysis, we should process the text data so that we will get valuable insights and information from dataset for further extraction and prediction. Text preprocessing involves 3 main steps:

Data Cleaning (Removing Brackets, Punctuations, Numbers and special characters)
Lemmatization
Parts of Speech (POS) Tagging
Exploratory Data Analysis
This process helps to analyse the data and extract valuable insights and information from dataset. This process includes plotting of wordcloud to check the most frequent word occurring in the complaints and then visualize top 30 unigrams, bigrams and trigrams.

# Feature Extraction
As we cannot feed text data directly to NMF, we have to convert it into numerical values. So, to convert text data into numerical features we use TF-IDF (Term Frequency-Inverse Document Frequency) vectorization method.

# Dimensionality Reduction and Topic Modelling using NMF
Since text data can have high dimensionality, Non-Negative Matrix Factorization (NMF) is applied to reduce the number of features while maintaining meaningful latent structures in the data. This method also helps in choosing a significant number of topics after checking the 20 common words belonging to each topic and finally map relevant/significant topic to each complaint.

# Build a Supervised Leaning Model for making a prediction for new complaint
After mapping the significant topic to ecah complaint we have implemented various machine learning algorithms (Naive Bayes, Logistic Regression, Decision Tree, and Random Forest) on the training data and then evaluated using accuracy, precision, recall, F1-score and Confusion Matrix. Since, Logistic Regression Model have highest accuracy (93%) and F1-score (92.6%), We conclude that the Logistic Regression model is best for making a prediction on custom complaints data. Finally, Logistic Regression model is then selected for deployment.
