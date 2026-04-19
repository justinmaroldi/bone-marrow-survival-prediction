# Bone Marrow Transplant Survival Prediction

**Tools:** R, Python (sklearn)
**Dataset:** UCI Bone Marrow Transplant Dataset — 187 pediatric 
patients, 37 clinical variables

## Overview
Built and compared classification models to predict 
post-transplant survival status in children, using only 
pre-surgery variables to avoid data leakage.

## My Contributions
- Logistic Regression (Model C): full end-to-end ownership
  - Handled missing values via k-NN imputation
  - Performed stepwise regression for initial variable selection
  - Applied VIF analysis to eliminate multicollinearity
  - Final model: RecipientRh, RecipientCMV, Riskgroup, 
    Recipient Age, DonorCMV (all VIF ≈ 1.0)
  - 70/30 train/test split, accuracy ~59%
- Model comparison and conclusions: evaluated Random Forest, 
  KNN, and Logistic Regression across accuracy, F1, and ROC

## Model Results
| Model | Accuracy |
| Random Forest | 54.3% |
| KNN | 59.6% |
| Logistic Regression | 59.0% |

## Key Findings
- KNN achieved the highest accuracy but was sensitive to 
  variable scaling
- Random Forest underperformed due to small dataset size
- Logistic Regression offered the best interpretability with 
  near-equivalent accuracy to KNN
- Dataset size (187 obs) was the primary constraint on all models

## Full Report
See attached PDF for complete analysis and slides.
