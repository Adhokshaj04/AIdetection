**AI Text Detection Project**

Authors:
- Adhokshaj Baliga
- Swathy Ragupathy
- Westin Perry
  
**Introduction**

This project aims to differentiate AI-generated text from human-written language. With the rapid growth of generative Large Language Models (LLMs) such as GPT and BERT, identifying AI-generated text is crucial for preserving information authenticity, upholding academic integrity, and protecting against false information.

**Importance**

As AI technologies advance, the boundaries between machine-generated and human-created content become increasingly blurred. Efficient detection systems are essential to maintain media and academic standards and to prevent the spread of misinformation.

**Innovation**

This project enhances the precision and reliability of AI text identification by integrating several machine learning models. By utilizing advanced preparation techniques and a varied ensemble of algorithms, this research sets a new benchmark for AI text identification, particularly in generalizing across different text types and languages.

**Paper Organization**

1. Problem Statement: Introduction to the research challenge and its significance.
2. Literature Review: Analysis of existing methodologies and their limitations.
3. Methodology: Detailed approach to developing and validating a model ensemble for detecting AI-generated texts.
4. Results: Findings of the study, focusing on model performance.
5. Discussion: Implications of the results for AI and digital content verification.
6. Conclusion: Summary of the study and suggestions for future research.
 
**Methodology**
Data Preparation
Two distinct datasets are used:

LLM-Generated Text Corpus: Contains 788,922 text records from 63 sources (one human-generated, 62 from different LLMs).
AI and Human-Generated Essays: Comprises 487,235 essays (181,438 human-generated).
Preprocessing Steps
Downsampling: Ensures an equal distribution of both classes in the training set.
Standard Scaler: Standardizes data to improve model behavior.
Stemming: Reduces words to their root forms.
Text Conversion: Converts all text to lowercase.
Whitespace and Special Character Removal: Cleans the text by removing unnecessary spaces and characters.
Stop Words Removal: Eliminates common words that do not contribute to classification.
Model Training
Various models are used, including:

TF-IDF: Traditional word representation technique.
BERT: Modern neural language model.
Random Forest: Robust algorithm for capturing nonlinear relationships.
One-Class SVM: Self-supervised model for anomaly detection.
Logistic Regression: Simple yet effective linear model.
Neural Network: Deep learning model for capturing subtle patterns.
Model Ensemble
Combining predictions from multiple models using techniques like majority voting or weighted averaging to improve accuracy and robustness.

**Results**

Performance metrics (accuracy, precision, recall, F1 score) are presented for both datasets, showing the strengths and weaknesses of each model and preprocessing method.

**Discussion**

TF-IDF vs. BERT: Both have unique advantages, with BERT performing better in semantic understanding.
Ensemble Model Performance: Combining models improves classification accuracy and robustness.
Methodological Insights: Highlighting the complexity of text representation and suggesting future work on adaptive models.

**Conclusion**

The study successfully compares TF-IDF and BERT in identifying AI-generated texts, emphasizing the importance of both methods depending on the context. Future research should explore hybrid models and their scalability in various operational scenarios.

**Future Work**

Development of adaptive models that dynamically choose the best text representation technique.
Evaluation on a wider range of datasets to confirm generalizability.
Investigation into the scalability and real-time use of these models.

**How to Use This Project**

Prerequisites
Python 3.x
Required libraries: scikit-learn, pandas, numpy, transformers (Hugging Face)
