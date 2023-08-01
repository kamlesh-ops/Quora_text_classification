# Quora Insincere Questions Classification   
An approach to preprocess texts obtained from quora and classify them as sincere and insincere.  
  
Data Source: Kaggle  
Link: [Dataset](https://www.kaggle.com/competitions/quora-insincere-questions-classification)  
My Submission on kaggle: [quora_notebook](https://www.kaggle.com/code/kamleshsahoo730/quora-nlp#Quora-Insincere-Questions-Classification)  

## About Dataset  
The dataset comprises texts from different types of questions asked on Quora. There are about 1 million examples of sincere texts and about 80K for insincere ones.     

## Python Libraries/Frameworks used  
Pytorch  
Pandas, Seaborn  
NLTK  
sci-kit learn  

## Notes  
1. The dataset is found to have class imbalances. For instance, there are about 1 million questions tagged as sincere, and only about 80K are tagged insincere. To handle this, the F1 score has been used as an evaluation metric, rather than normal accuracy.
2. To speed up the process of training, a subset of the entire dataset has been used as a sample.

## Models
1. A basic neural network pipeline to check the functionality.  

## Training  
1. To speed up training, GPU was used.
2. Used train_test_split to split the dataset into 75% training and 25% validation data.

## Loss  
Binary Cross-Entropy: They are suitable for the f1 metric as they align well(when binary loss decrease, the f1 score does not change much).  

## Optimizer  
Adam: Converges faster than others like SGD.

## Accuracy/score  
1. Using basic NN from scratch:
   No. of epochs = 20 | 
   Loss: 1.30 | 
   F1-score: 0.33 







