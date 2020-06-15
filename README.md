# Cancer-Diagnosis
Testing various Machine Learning algorithms to identify genetic variations of Cancer cells.

A lot has been said during the past several years about how precision medicine and, more concretely, how genetic 
testing is going to disrupt the way diseases like cancer are treated.But this is only partially happening due to the huge amount of manual work still required.
Once sequenced, a cancer tumor can have thousands of genetic mutations. But the challenge is distinguishing the mutations that contribute to tumor growth (drivers) from the neutral mutations (passengers). 
Currently this interpretation of genetic mutations is being done manually. This is a very time-consuming task where a clinical pathologist has to manually review and classify every single genetic mutation based on evidence from text-based clinical literature.
Credits > Kaggle

## Problem Statement:
Developing a Machine Learning algorithm that, using various features and literature as base as a baseline, automatically classifies genetic variations.

## Objectives and Constraints:
- No low-latency requirement.
- Model should be interpretable.
- Errors can be very costly.
- Probability of each class is needed.

## Data Overview:
- The data is taken from [Kaggle.](https://www.kaggle.com/c/msk-redefining-cancer-treatment/)
- We are given two data files: one conatins the information about the genetic mutations and the other contains the clinical evidence (text) that human experts/pathologists use to classify the genetic mutations.
- Both these datasets have a common column __"ID"__
- Data files info:
  - training_variants (ID, Gene, Variation, Class)
  - training_text (ID, Text)

## Mapping the real-world problem to a Machine Learning Problem:
- There are Nine different classes (0-8) that a genetic mutation can be classified into. We treat this problem as a __Multiclass Classification__ problem.
- Performance Metrics:
  1. Multiclass Log Loss.
  2. Confusion Matrix, Precision, Recall.
  

