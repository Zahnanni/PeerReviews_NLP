# Peer Review Content Analysis

This is an exam project for the course of computational literacy, analysing the content of Peer Reviews within the subject Natural Language Processing. 

## How to reproduce the analysis

### Data acquisition
You have to download the dataset PeerRead from this Github repository: https://github.com/allenai/PeerRead
In the first draft, only the reviews from the conferences ACL 2017, CoNLL 2016 and ICLR 2017 were used which are already provided in the dataset.
Than, you'll have to import the JSON encoded text files into a Jupyter notebook and extract the reviews from the single files. Each file contains several reviews which can be extracted using the hierarchy of the documents and regular expressions. The libraries used were Panda and Regex.

### Data Processing
The list of reviews were tokenised and tagged with the part of speech using the library NLTK. A list of all adjectives was extracted. Over 80 percent of adjectives were classified manually into the classes: positive, negative, both, non-evaluative and false.

It is planned to repeat the before mentioned steps with the additional data from the NIPS conference and to add cleaning steps which were recognised while classifying the adjectives. After the classification of all adjectives (together with the ones extracted from the reviews of the NIPS conference), it is planned to extract the sentences containing the adjectives and to create two lists: one with the positive expressions and one wth the negative. The adjectives attributed with "both" will be manually classified and added to the existing lists.


### Analysis
The analysis was not conducted yet. It is planned to apply a keyword extraction with the software Annif on the two lists with extracted sentences and to analyse the keywords with descriptive statistics afterwards.

### Results
No analysis took place yet, therefore, no results are available yet.


The python code used, the list of extracted reviews and the list of adjectives are available at Github (https://github.com/Zahnanni/PeerReviews_NLP/).