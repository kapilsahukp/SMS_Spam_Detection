#### Objective:

     To buil an "SMS Spam Detector" to classify SMS as legit or spam.

#### Data:
     This corpus has been collected from free or free for research sources at the Web:
     - A collection of between 425 SMS spam messages extracted manually from the Grumbletext Web site. 
     This is a UK forum in which cell phone users make public claims about SMS spam messages, 
     most of them without reporting the very spam message received. The identification of the text 
     of spam messages in the claims is a very hard and time-consuming task, and it involved carefully scanning hundreds of web pages. 
     The Grumbletext Web site is: http://www.grumbletext.co.uk/
     - A list of 450 SMS ham messages collected from Caroline Tag's PhD Theses available at http://etheses.bham.ac.uk/253/1/Tagg09PhD.pdf
     - A subset of 3,375 SMS ham messages of the NUS SMS Corpus (NSC), which is a corpus of about 10,000 legitimate messages 
     collected for research at the Department of Computer Science at the National University of Singapore.
     The messages largely originate from Singaporeans and mostly from students attending the University. 
     These messages were collected from volunteers who were made aware that their contributions were going to be made publicly available. 
     The NUS SMS Corpus is avalaible at: http://www.comp.nus.edu.sg/~rpnlpir/downloads/corpora/smsCorpus/
     - The amount of 1,002 SMS ham messages and 322 spam messages extracted from the SMS Spam Corpus v.0.1 Big 
     created by José María Gómez Hidalgo and public available at: http://www.esp.uem.es/jmgomez/smsspamcorpus/

##### Link to detailed data description:

Click [here] (https://github.com/kapilsahukp/SMS_Spam_Detection/blob/main/data/data_readme)

#### Data Cleaning:
     -Removed special characters.
     -Removed STOP Words.
     -Used Stemming and Lemmatization to find root words in the text.
     
#### Data Modeling:
     -Used Bag of Words(BOW) and Term Frequency Inverse Document Frequency (TF-IDF) data models to represent text in the form of vectors.

#### Predictive Modeling:
     -To classify the SMS text as legit or spam, the Naive Bayes Classifier is used.
     -The model is trained and tested using 80/20 train-test split of dataset.

#### Performance Evaluation:
     -Confusion matrix is plotted to find out the performance of classifier.
     -Accuracy is calculated on the basis of Confusion Matrix data.

#### Results:
     -Using BOW + Stemming , Accuracy = 98.47% (approx.)
     -Using BOW + Lemmatization , Accuracy = 98.20% (approx.)
     -Using TF-IDF + Stemming , Accuracy = 96.95% (approx.)
     -Using TF-IDF + Lemmatization , Accuracy = 97.21% (approx.)

#### Conclusion:
     Best accuracy is achieved when we used the combination of BOW and Stemming but it has its drawbacks as 
     some words are not meaningful since we used stemming and the BOW gives weightage in binary form 0/1.
     A better approach is to use TF-IDF along with Lemmatization as it assigns relative weightage(fractional values) 
     and the we have meaningful words after lemmatization. 
     
#### Future Work:
     We can perform the same operations on a balanced dataset.
