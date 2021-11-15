# hate_speech_detection  
This application tries to classify the tweets given as data if it contains hate speech of any kind.  
Hate speech is defined as a type of speech that takes place online with the purpose of attacking a person or a group based on their race, religion, ethnic origin, sexual orientation, disability, or gender.
  
  
#This application utilizes hate_speech_detection.csv as dataset for training the model used for classification the dataset comprises of 2 features:  
1) Label - It comprises of the label given a tweet, if label is 0 then tweet is free of hate speech of any form if 1 then it consist of some kind oh hate speech.  
2) Tweet - It consist of tweets from large number of users online with their usernames redacted or censored.  

#Libraries used in the projects :  
1) Pandas  
2) nltk  
3) sklearn  
4) re
5) numpy
6) wordcloud  

Cassification model used here is Random forest classifier from ensemble class with 50 trees. Dataset passed is first cleaned by removing the words that offer no use to out classification model by using regular expression to remove these words. In the next step we lemmatize the words eg. 'running' is converted to 'run', thus making the dataset more simple. After that tokenisation is done on dataset and dataset is split in to test and training set. Model is trained on training set and tested on test set and the classification report is created, measuring the required aspect of model.  
Further improvements can be done by refining the qualitybof dataet and by trying out other classification model and tweaking their parameters. 

