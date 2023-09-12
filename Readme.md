Text preprocessing is an essential step in natural language processing (NLP) that involves cleaning and transforming unstructured text data to prepare it for analysis. 

Natural Language Processing is a branch of Artificial Intelligence that analyzes, processes, and efficiently retrieves information text data. By utilizing the power of NLP one can solve a huge range of real-world problems which include summarizing documents, title generator, caption generator, fraud detection, speech recognition, recommendation system, machine translation, etc.

**NLTK** is an old library used for practicing NLP techniques by beginners. 
**Spacy** is the latest released library with the most advanced techniques and mostly used in the production environment 

###To prepare the text data for the model building we perform text preprocessing. It is the very first step of NLP projects. Some of the preprocessing steps are:
---
###1. Removing Punctuations like . , ! $( ) * % @
One of the other text processing techniques is removing punctuations. there are total 32 main punctuations that need to be taken care of. we can directly use the string module with a regular expression to replace any punctuation in text with an empty string. 32 punctuations which string module provide us is listed below.

'!"#$%&'()*+,-./:;<=>?@[\]^_`{|}~'

###2. Removing URLs
###3. Removing Stop words
Stopwords are the most commonly occurring words in a text which do not provide any valuable information. stopwords like they, there, this, where, etc are some of the stopwords. NLTK library is a common library that is used to remove stopwords and include approximately 180 stopwords which it removes. If we want to add any new word to a set of words then it is easy using the add method.
###4. Lower Casing
If the text is in the same case, it is easy for a machine to interpret the words because the lower case and upper case are treated differently by the machine. for example, words like Ball and ball are treated differently by machine. So, we need to make the text in the same case and the most preferred case is a lower case to avoid such problems.
###5. Tokenization 
###6. Stemming and Lemmatization
Stemming is a process to reduce the word to its root stem for example run, running, runs, runed derived from the same word as run. 

Basically stemming do is remove the prefix or suffix from word like ing, s, es,etc. NLTK library is used to stem the words. The stemming technique is not used for production purposes because it is not so efficient technique and most of the time it stems the unwanted words. So, to solve the problem another technique came into the market as Lemmatization. there are various types of stemming algorithms like porter stemmer, snowball stemmer. Porter stemmer is widely used present in the NLTK library.

Lemmatization is similar to stemming, used to stem the words into root word but differs in working. Actually, Lemmatization is a systematic way to reduce the words into their lemma by matching them with a language dictionary.

###7. Expand Contractions
Contraction is the shortened form of a word like don’t stands for do not, aren’t stands for are not. Like this, we need to expand this contraction in the text data for better analysis. you can easily get the dictionary of contractions on google or create your own and use the re module to map the contractions.

###8. Remove words and digits containing digits
Sometimes it happens that words and digits combine are written in the text which creates a problem for machines to understand. hence, We need to remove the words and digits which are combined like game57 or game5ts7. This type of word is difficult to process so better to remove them or replace them with an empty string. we use regular expressions for this. The first mail is not having digits but other mails in the dataset contain this problem like mail 4.

###9. Rephrase text
we may need to modify some text or change the pattern to a particular string which makes it easy to identify like we can match the pattern of email ids and change it to string like email address. In our example, we will modify the URL address and email address.

###10. Remove Extra Spaces
Most of the time text data contain extra spaces or while performing the above preprocessing techniques more than one space is left between the text so we need to control this problem. regular expression library performs well to solve this problem.

[Link](https://www.analyticsvidhya.com/blog/2021/06/text-preprocessing-in-nlp-with-python-codes/)

>**TODO** Next

[Next](https://www.kaggle.com/code/sudalairajkumar/getting-started-with-text-preprocessing)