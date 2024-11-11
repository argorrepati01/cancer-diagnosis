# Personalized Cancer Diagnosis

This project is inspired by the MSKCC Kaggle Competition, which aims to advance cancer diagnosis by distinguishing impactful mutations from neutral ones in tumor genetic profiles.
Currently, interpreting genetic mutations involves a time-intensive manual process. Clinical pathologists must individually review and classify each mutation based on supporting evidence from clinical literature. The goal of this project is to build a machine-learning model that can classify genetic mutations based on clinical texts.

## Objective

- Build a multiclass classification model using Gene, Variant, and Text features that categorize into nine different classes.
- Interpretability is important, to understand how the model is classifying.
- Probability of a data point belonging to each class.
- Low-error model, since errors are costly.

## Data Overview

The training dataset has two files:
  - training_variants: ID, Gene, Variation, and Class (1-9) labels
  - training_text: ID, text

Similarly for the test dataset.

## Performance Metrics Used

- MultiClass Log Loss
- Confusion Matrix
  
## Approach

- Data Pre-processing: Encoding the Gene, Variant, and Text features using One-Hot, Response, and TF-IDF.
- Perform Uni-Variate analysis and understand the importance of each feature in the classification.
- Build a random model that randomly assigns class labels to each data point.
- Implement various machine learning models and use the random model as a baseline to compare the performance metrics.
