# Sentment-Analysis-on-Covid-19-Tweets
DataSet is Attached with python Notebook file.
Dataset is already labelled (annoted) so you can directly use it for your project.

# My Approch On Sentiment Analysis Using Deep Nueral  Network
## First Model is based on 
  - Uses LSTM based Network with Input, Embedding, GlobalMaxPooling1D, Dense Layers
  - And its padding Sequence = 96 (max words in a tweet in this dataset)
  
 ## Second Model is based on 
  - Uses Bi-LSTM based Network with Input, Embedding, GlobalMaxPooling1D, Dense, Bidirectional,BatchNormalization, GlobalMaxPool1D, Dropout, Flatten Layers
  - And its padding Sequence = 20 (randomly taken avg length of tweets text in this dataset is 15)


# Procedure
  - 'Here, is an sample text for the input #TextFile' (raw input tweet text content)
  - 'Here sample text input' (after textCleaning and removing the stopwords)
  - ['Here sample text input'] (converted to python list)
  - ['Here','sample','text','input'] (Sentense is splitted int words)
  - [10,250,381,58] (each number that maps to position of the word in the VOCABULARY built using taking all tweet text in the dataset) 
  - [10,250,381,58, 0,0,0,0,0 ,0,0,0] (padded  sequence for length = 12 this is used make all sentense to same length = input layer size)
  - Now it can be feeded into Nueral Network.



 # Tips:
  - If you Reduce the padding sequence Model accuracy increases but it will ignore words that comes after seq length

 
 # !!! Training these model takes lot of time if have nvidia gpu install cuda drivers that reduces the training time significantly but, it is completely optional !!!
 



 

