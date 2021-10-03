# Text-Summarizer-and-Essay-Grader
### Project description:
- The entire purpose of text summarization is to condense the source data into a concise version of text while preserving information content and overall meaning
- Grading essays takes up a significant amount of an instructor's valuable time, and hence is an expensive process.Automated Essay grading system allows us to assign scores to essays using computer programs

### Problem Statement:
To build an automated Text summarizer & Essay grading model 

### Dataset:
The dataset for essay grading is taken from kaggle . Link to the dataset : https://www.kaggle.com/c/asap-aes/data.
It consists of 12976 rows, 28 columns of which 6 columns are considered.

### Data description:
- essay_id : Unique id for each essay
- essay_set : A particular set number to which the eassay belongs (there are 8 distinct essay sets)
- essay : Consists of essays
- rater1_domain1 : Score given manually by an examiner 1
- rater2_domain2 : Score given manually by an examiner 2
- domain1_score : Average score of rater1_domain1 and rater2_domain2

### Tools used:
spaCy, Gensim, NLTK, Lexrank, Sumy, sklearn, Flask

### Work Flow:
1. Essay Grader
- Scaling grades from different sets
- Pre-processing 
- Feature extraction using sklearn and nltk
- Prediction using Support vector regressor

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
Live demonstration of the dashboard :
https://user-images.githubusercontent.com/73699314/135741675-bd9fb3ca-3aef-448d-964f-5707b10c365b.mp4
 
### Inferences
- This model helps us by simplifying the sheer volume of information that humans interact with daily and hence optimises and reduces the time complexity.
- The working of Spacy and NLTK is the same. Also, gensim and Sumy is the same. Hence, they produce the same result.
- Easy grader helps grade essays without bias and saves time.
