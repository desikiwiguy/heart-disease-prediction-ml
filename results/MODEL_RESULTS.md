# Model Performance

After training multiple models, their performance was compared on the test dataset.

## Evaluation Metrics Used
- Accuracy
- Precision
- Recall
- F1 Score

F1-score was considered the most important metric because in medical prediction, failing to detect a diseased patient is more critical than a false positive.

## Observations

Logistic Regression:
- Produced stable predictions
- Lower recall for positive cases
- Good baseline performance

Random Forest:
- Better at identifying high-risk patients
- Higher recall and F1-score
- Handled complex feature relationships better

## Final Model
Random Forest was selected as the final model because it provided better balance between precision and recall.

The trained model was saved and integrated into the Flask web application for real-time prediction.

## Confusion Matrix Interpretation
The confusion matrix shows:
- True Positives → correctly identified sick patients
- True Negatives → correctly identified healthy patients
- False Positives → predicted sick but actually healthy
- False Negatives → predicted healthy but actually sick

Minimizing false negatives was important because missing a heart disease case can be dangerous.
