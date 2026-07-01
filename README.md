#  Aspect-Based Sentiment Analysis (ABSA) using NLP

An **Aspect-Based Sentiment Analysis (ABSA)** system that analyzes customer reviews to determine sentiment toward specific product or service aspects instead of assigning a single sentiment to the entire review.

This project implements a **two-phase hybrid NLP pipeline**:
- **Phase 1:** Lexicon-based sentiment analysis using **VADER** on the **SemEval-2014 ABSA Dataset**
- **Phase 2:** Transformer-based sentiment analysis using **BERT** on the **Amazon Electronics Reviews Dataset**

The project demonstrates the evolution from traditional sentiment analysis to modern transformer-based NLP while providing visual insights and evaluation metrics.

---

#  Features

- Aspect-Based Sentiment Analysis (ABSA)
- Automatic aspect extraction
- Sentiment classification
- Data preprocessing and cleaning
- Lexicon-based sentiment analysis (VADER)
- Transformer-based sentiment analysis (BERT)
- Aspect-wise sentiment visualization
- Performance evaluation
- Dataset preprocessing
- Model saving and loading
- Comparative analysis between traditional NLP and Transformer models

---

#  Technologies Used

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- NLTK
- Hugging Face Transformers
- Scikit-Learn
- Matplotlib
- Seaborn
- XML ElementTree

### NLP Models

- VADER Sentiment Analyzer
- BERT Sentiment Analysis Pipeline

---

#  Datasets

## 1. SemEval-2014 Task 4 Dataset

Used in Phase 1.

Contains:

- Laptop Reviews
- Restaurant Reviews

Dataset provides:

- Review Sentence
- Aspect Term
- Ground Truth Sentiment

---

## 2. Amazon Consumer Reviews Dataset

Used in Phase 2.

Contains:

- Product Name
- Customer Review
- Product Rating

The project filters reviews for the most reviewed product before performing aspect-based sentiment analysis.

---

#  Workflow

## Phase 1 — VADER-Based ABSA

### Step 1

Download and preprocess SemEval Dataset.

↓

### Step 2

Extract

- Sentence
- Aspect
- Sentiment
- Domain

↓

### Step 3

Clean text

↓

### Step 4

Map aspects into predefined categories

Examples:

- Battery
- Screen
- Price
- Performance
- Design
- Food
- Service
- Ambience

↓

### Step 5

Perform sentiment analysis using VADER

↓

### Step 6

Aggregate sentiments aspect-wise

↓

### Step 7

Visualize results

↓

### Step 8

Evaluate using

- Accuracy
- Weighted F1 Score
- Classification Report

---

#  Phase 2 — BERT-Based ABSA

### Step 1

Load Amazon Reviews Dataset

↓

### Step 2

Clean dataset

↓

### Step 3

Select the most reviewed product

↓

### Step 4

Extract aspects using keyword matching

Example aspects:

- Battery
- Camera
- Screen
- Performance
- Price
- Design

↓

### Step 5

Perform sentiment prediction using BERT

↓

### Step 6

Generate

- Aspect-wise Bar Graph
- Pie Charts

↓

### Step 7

Evaluate using product ratings as ground truth

↓

### Step 8

Save trained model

↓

### Step 9

Reload saved model

---

#  Evaluation Metrics

The project evaluates model performance using:

- Accuracy
- Weighted F1 Score
- Classification Report

---

#  Visualizations

The project generates:

- Aspect-wise Sentiment Distribution
- Sentiment Count Bar Charts
- Aspect-wise Pie Charts
- Positive vs Negative Sentiment Comparison

---

#  Aspect Categories

### Phase 1

- Battery
- Screen
- Price
- Performance
- Design
- Food
- Service
- Ambience

### Phase 2

- Battery
- Camera
- Screen
- Performance
- Price
- Design

---

#  Model Saving

The BERT model is saved locally using

```
save_pretrained()
```

Both

- Model
- Tokenizer

are stored for future inference.

---

#  Installation

Clone the repository

```bash
git clone https://github.com/yourusername/ABSA-NLP.git

cd ABSA-NLP
```

Install dependencies

```bash
pip install pandas
pip install numpy
pip install nltk
pip install transformers
pip install torch
pip install matplotlib
pip install seaborn
pip install scikit-learn
```

or

```bash
pip install -r requirements.txt
```

---

#  Running the Project

Open

```
NLP_ABSA.ipynb
```

Run all notebook cells sequentially.

The notebook automatically

- Downloads datasets
- Cleans data
- Performs ABSA
- Generates graphs
- Evaluates models
- Saves outputs

---

#  Outputs

Generated outputs include:

- Cleaned datasets
- Aspect-wise sentiment predictions
- Evaluation metrics
- CSV result files
- Visualizations
- Saved BERT model

---

#  Future Improvements

- Fine-tune BERT specifically for ABSA
- Dynamic aspect extraction using spaCy
- Replace keyword matching with Named Entity Recognition
- Multi-class sentiment prediction
- Domain adaptation
- Deploy using Streamlit or Flask
- Add explainable AI (XAI)
- Support multilingual sentiment analysis

---

#  Applications

- Product Review Analysis
- E-commerce Analytics
- Customer Feedback Mining
- Brand Monitoring
- Market Research
- Business Intelligence
- Restaurant Review Analysis
- Consumer Electronics Analysis

---

#  Author

**Leela Meghana**

**Role:** NLP Researcher

### Responsibilities

- Conducted research on Aspect-Based Sentiment Analysis techniques.
- Analyzed model outputs to evaluate sentiment classification performance.
- Compared traditional lexicon-based methods with Transformer-based approaches.
- Interpreted evaluation metrics and visualization results.

---

#  License

This project is intended for educational and research purposes.

---

#  Acknowledgements

- SemEval-2014 Task 4 Dataset
- Amazon Consumer Reviews Dataset
- Hugging Face Transformers
- NLTK
- Scikit-Learn
- Matplotlib
- Seaborn

---

 If you found this project useful, consider giving it a star!
