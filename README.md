#  Resume Screening AI using NLP
An AI-powered system that ranks resumes using NLP techniques (TF-IDF and BERT) for automated candidate shortlisting.

##  Overview

This project builds an AI-based Resume Screening system that ranks resumes based on their relevance to a given job description.

It uses Natural Language Processing (NLP) techniques to compare resumes with job requirements and automatically shortlist candidates.


##  Objective

* Automate resume screening process
* Match resumes with job descriptions
* Rank candidates based on similarity


##  Methods Used

###  TF-IDF (Baseline Model)

* Keyword-based matching
* Fast and simple
* Does not understand meaning

###  BERT (Advanced Model)

* Transformer-based embeddings
* Captures semantic meaning
* Provides more accurate matching


##  Approach

1. Load resume dataset
2. Clean and preprocess text
3. Convert text into vectors
4. Compute similarity using cosine similarity
5. Rank resumes based on scores


##  Results

###  TF-IDF Results

* Low similarity scores (~10–17%)
* Based only on keyword matching

Example:

```text
17.4% → ARTS
14.12% → BANKING
13.16% → DESIGNER
12.42% → AGRICULTURE
10.5% → TEACHER
```

###  BERT Results

* Higher similarity scores (~38–48%)
* More relevant category matching

Example:

```text
Score: 48.99% → AGRICULTURE
Score: 45.86% → BPO
Score: 44.02% → ENGINEERING
Score: 42.59% → ENGINEERING
Score: 40.86% → ENGINEERING
```


##  Comparison

* TF-IDF → Keyword matching
* BERT → Semantic understanding

BERT provides better results for real-world applications


##  User Input Testing

The system allows dynamic job description input:

Example:

```text
Looking for a Data Scientist skilled in Python, machine learning, statistics, data visualization, and SQL.
```

Output:

```text
63.90% → ENGINEERING
44.33% → AUTOMOBILE
43.95% → CONSULTANT
43.74% → BANKING
```


##  Features

* Resume ranking system
* TF-IDF vs BERT comparison
* User input-based matching
* Real-world recruitment use case


##  Tech Stack

* Python
* Pandas
* Scikit-learn
* Sentence Transformers (BERT)
* Google Colab

  
##  Dataset

The dataset used in this project is publicly available on Kaggle:

🔗 https://www.kaggle.com/datasets/snehaanbhawal/resume-dataset

Due to file size limitations, the dataset is not included in this repository.

##  How to Run

1. Download the dataset from Kaggle  
2. Upload the ZIP file in Google Colab  
3. Open the notebook  
4. Run all cells  
5. Enter job description when prompted  
6. View ranked results  

##  Key Insight

* TF-IDF works for keyword matching
* BERT performs better due to semantic understanding


##  Limitations

* Requires clean text data
* BERT is computationally expensive
* Does not process PDF resumes directly


##  Future Improvements

* Add PDF resume parsing
* Build Streamlit web app
* Improve ranking with hybrid models


##  Use Case

This system can help:

* Recruiters
* HR teams
* Hiring platforms

to automate candidate shortlisting.


## 👨‍💻 Author

Ahalya Reddy Kora  
AI/ML Student
