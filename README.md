# Twitter-Sentiment-Analysis

In this project the goal is to extract the sentiment of a tweet and give a score to it. I used the sentiment140 dataset with 1.6 million tweets, first I preprocessed the dataset using nltk library and the new cleaned dataset the a seperate file. For feature extraction I used TfidfVectorizer.

TfidfVectorizer extracts all the words from a set of documents and then based on the frequency of the word in different documents it generates a value for it. After this rather than having various words, I get an array of numbers such as [0,0,0,0.........0,0,0,0].
For understanding this algorithm i need to understand mathematical meaning of TF-IDF.Here 'TF' is 'Term frequency' and 'IDF' is 'Inverse document frequency'.

The formula for TF is given by => Number of times a term is repeated in a document
                                ----------------------------------------------------
                                        Number of terms in that document

And, formula for IDF is given by =>      Total number of documents
                                   ---------------------------------------
                                    Number of documents containg the term

After calculating both of these, the weight for word is given by = (TF)*(IDF)

Here, I only extracted best 50000 features or terms.
