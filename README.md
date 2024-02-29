# Rating the Language Appropriateness of Children’s Videos on YouTube
We propose a machine-learning method that uses labeled data from a movie rating website (for parents to decide the appropriateness of a movie) to train a deep-learning model to rank movies. When trained using a multi-task method, the model additionally produces a summary explaining the basis for the language rating, highlighting words and phrases that may be possibly inappropriate for children. Using the suggested approach, we examine over 85,000 videos from the top 100 YouTube Kid's channels and contrast them with Disney/Pixar films that are certified for children viewing.  
## Regression Eval. Metrics for Language Rating 
| Model | MSE | RMSE | MAE | R<sup>2</sup> | E. Variance|
|----------|----------|----------|----------|----------|----------|
| GPT-3.5 for Regression | 6.56 | 2.56 | 1.92 | 0.11 | 0.12 |
| BART Multitask Model    | 6.99    | 2.64    | 1.31    | 0.57    | 0.57    |
| Decision Tree    | 5.56    | 2.35    | 1.56    | 0.25    | 0.25    |
| Support Vector Machine    | 4.70    | 2.16    | 1.62    | 0.36   | 0.36    |
| Random Forest    | 3.59    | 1.89    | 1.27    | 0.51    | 0.51   |
| XGBoost   | 3.74    | 1.93   | 1.28   | 0.49    | 0.49    |
| BART for Regression    | 1.80   | 1.34    | 0.58    | 0.86    | 0.87   |


## Summarization Eval. Metrics for Language Description
| Model             | RougeL | Precision | Recall | F1    |
|-------------------|--------|-----------|--------|-------|
| MPT-7B            | 0.0209 | 0.772     | 0.794  | 0.78  |
|Stable LM Zephyr 3B| 0.0884 | 0.796     | 0.851  | 0.822 |
| Mistral-7B        | 0.1007 | 0.783     | 0.822  | 0.802 |
| GPT-3.5           | 0.1071 | 0.824     | 0.851  | 0.837 |
| GPT-4             | 0.1388 | 0.822     | 0.865  | 0.842 |
| Dolly 8B          | 0.1437 | 0.811     | 0.864  | 0.836 |
| BART Summarization*| 0.1823 | 0.822 | 0.894 | 0.856 |
