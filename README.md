# LanguageRatingAndSummary
## Regression Eval. Metrics
| Model | MSE | RMSE | MAE | R<sup>2</sup> | E. Variance|
|----------|----------|----------|----------|----------|----------|
| Random Forest    | 3.59    | 1.89    | 1.27    | 0.51    | 0.51   |
| XGBoost   | 3.74    | 1.93   | 1.28   | 0.49    | 0.49    |
| Decision Tree    | 5.56    | 2.35    | 1.56    | 0.25    | 0.25    |
| Support Vector Machine    | 4.70    | 2.16    | 1.62    | 0.36   | 0.36    |
| BART for Regression    | 1.80   | 1.34    | 0.58    | 0.86    | 0.87   |
| GPT-3.5 for Regression    | 18.99    | 4.35    | 3.66     | -1.44    | -1.25    |
| BART Multitask Model    | 6.99    | 2.64    | 1.31    | 0.57    | 0.57    |


## Summarization Eval. Metrics
| Model             | RougeL | Precision | Recall | F1    |
|-------------------|--------|-----------|--------|-------|
| BART Summarization| 0.34   | 0.78      | 0.79   | 0.78  |
| GPT-3.5           | 0.0050 | 0.38      | 0.26   | 0.31  |
| Multitask Model   | 0.0110 | 0.35      | 0.28   | 0.30  |



