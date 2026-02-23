# Text Classification using NLP and Machine Learning

This project builds an end-to-end Natural Language Processing (NLP) pipeline to classify text data into predefined categories using traditional machine learning models.

## Features
- Text data preprocessing and cleaning
- Tokenization and normalization
- Stopword removal
- TF-IDF feature extraction
- Model training and evaluation
- Accuracy and F1-score analysis
- Confusion matrix visualization
- Sample prediction on custom input text

## Technologies Used
- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- Matplotlib
- Seaborn

## Methodology
- Load raw text dataset
- Clean text (lowercasing, removing punctuation and special characters)
- Remove stopwords
- Convert text into numerical features using TF-IDF vectorization
- Split dataset into 80% training and 20% testing
- Train classification models (Logistic Regression / Naive Bayes / SVM)
- Evaluate model using Accuracy and F1-score
- Generate confusion matrix for performance analysis

## Model Pipeline
- Data Loading
- Text Preprocessing
- Feature Extraction (TF-IDF)
- Model Training
- Evaluation
- Prediction

## Results
- Successfully classified text into target categories
- Achieved competitive accuracy on test dataset
- Model generalizes well to unseen text inputs

## Project Structure
text-classification-nlp/
│
├── dataset.csv
├── nlp_preprocessing.py
├── model_training.py
├── evaluation.py
├── requirements.txt
└── README.md

## How to Run

Install dependencies:

```bash
pip install pandas numpy nltk scikit-learn matplotlib seaborn
```

Run the training script:

```bash
python model_training.py
```

Run prediction:

```bash
python predict.py
```

## Example Input
- "This product is amazing and works perfectly"
- "The service was terrible and disappointing"

The model outputs the predicted category for the input text.
