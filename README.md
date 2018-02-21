# reddit classifier using Latent Dirichlet Allocation

In this project I use topics identified using Latent Dirichlet Allocation as features in a machine learning classifier.  The project includes loading JSON formatted data, exploratory analysis, cleaning and processing the data into a machine learning friendly format, implementing Gensim's Latent Dirichlet Allocation to identify topics in the corpus, transoforming the topic contributions into features that can be used by a machine learning model, and a bag-of-words model using tfidf for comparison.  

The results of using topic features alone as classifier show a slight decay compared with the perforamance acheived with a bag-of-words model.  Additional lift may be found in compbining the two approaches (tfidf and topic features) either through weighting scheme or perhaps through additional phrase-modelling. 

The analysis is based on one month of reddt comment data (May 2017) downloaded from www.pushshft.io

project includes:
  *Loading JSON formatted data into a pandas dataframe
  *processing text in comments
  *using GenSim LDA to cluster corpus into topics
  *parsing LDA attributes to attach topics to each document
  *parsing LDA attributes to extract words in each topic and contribution to topic probability
  *predicting good or bad comment based on score
