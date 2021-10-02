# Text-Summarizer-and-Essay-Grader
### Project description:
- The entire purpose of text summarization is to condense the source data into a concise version of text while preserving information content and overall meaning
- Grading essays takes up a significant amount of an instructor's valuable time, and hence is an expensive process.Automated Essay grading system allows us to assign scores to essays using computer programs

### Problem Statement:
To build an automated Text summarizer & Essay grading model 

### Dataset:
The dataset is taken from kaggle . Link to the dataset : https://www.kaggle.com/c/asap-aes/data

### Tools used:
spaCy, Gensim, NLTK, Lexrank, Sumy, sklearn, Flask

### Work Flow:
1. Essay Grader
- Scaling grades from different sets
- Pre-processing
- Feature extraction using sklearn and nltk
- Prediction using Suppoer vector regressor

2. Text Summarizer using Sumy Lexrank and Gensim
- Convert Paragraphs to sentences
- Text Pre-processing
- Find vector representation for every sentence
- Construct similarity matrix between vectors
- Similarity matrix is then converted into a graph
- The top-ranked sentences form the final summary

3. Text Summarizer using Spacy and NLTK:
- Convert Paragraphs to Sentences
- Text Pre-processing
- Tokenizing the Sentences
- Find Weighted Frequency of Occurrence
- Replace Words by Weighted Frequency in Original Sentences
- Sort Sentences in Descending Order of Sum


### Result :
Link to a live demonstration of the dashboard :
 
### Inferences
- This model helps us by simplifying the sheer volume of information that humans interact with daily and hence optimises and reduces the time complexity.
- The working of Spacy and NLTK is the same. Also, gensim and Sumy is the same. Hence, they produce the same result.
- Easy grader helps grade essays without bias and saves time.
