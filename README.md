# Quora Insincere Questions Classification  
Data Source: Kaggle  
Link: [Dataset](https://www.kaggle.com/competitions/quora-insincere-questions-classification)

## About Dataset  
The dataset comprises texts from different types of questions asked on Quora, and the objective is to find how many of them are sincere ones.  

## Python Libraries/Frameworks used  
Pytorch  
Pandas, Seaborn  
NLTK  

## Notes  
1. The dataset is found to have class imbalances. For instance, there are about 1 million questions tagged as sincere, and only about 80K are tagged insincere. To handle this, the F1 score has been used as an evaluation metric, rather than normal accuracy.
2. To speed up the process of training, a subset of the entire dataset has been used as a sample.  
3. With an intention to get the vocabulary built from the document itself, and also tokenize it, the tfidf vectorizer has been used.  



