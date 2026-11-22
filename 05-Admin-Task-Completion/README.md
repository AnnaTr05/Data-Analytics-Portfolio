# Admin Task Completion Prediction

## Project Overview
This project uses Logistic Regression to predict whether system administrators will complete their assigned tasks based on their experience, training, and team information.

The goal is to identify patterns associated with task completion and evaluate how effectively a classification model can predict administrative task outcomes.

## Tools & Technologies
- **R / RStudio** – Data analysis and model development
- **R Markdown** – Documentation and reporting
- **ggplot2** – Data visualization
- **caret** – Model training and evaluation
- **pROC** – ROC curve and AUC analysis
- **Logistic Regression (GLM)** – Predictive modeling
- **Confusion Matrix** – Classification performance evaluation

## Methodology
1. **Data Preparation:** Imported the administrator dataset, inspected its structure, and prepared variables for classification.
2. **Exploratory Data Analysis:** Used scatter plots to explore the relationships between experience, training, and task completion.
3. **Data Splitting:** Divided the dataset into training and testing subsets.
4. **Model Development:** Built a Logistic Regression model using Experience, Training, and Team as predictors.
5. **Model Evaluation:** Evaluated performance using confusion matrices, accuracy, sensitivity, specificity, and ROC-AUC.
6. **Prediction:** Generated predicted probabilities and classified administrators based on a 0.5 probability threshold.

## Results & Key Findings
The Logistic Regression model demonstrated strong classification performance:

- **Training Accuracy:** 89.08%
- **Testing Accuracy:** 85.47%
- **ROC-AUC:** 0.9562

The model achieved sensitivity above 92% on both training and testing datasets, indicating strong performance in identifying the negative class (administrators who did not complete their tasks, based on the reported class interpretation).

The ROC-AUC score of 0.9562 indicates excellent ability to distinguish between the two task-completion outcomes. In other words, the model has a strong ability to rank administrators with different outcomes based on their predicted probabilities.

The slightly lower testing accuracy compared with training accuracy is expected when evaluating a model on unseen data.

## Conclusion
This project demonstrates how Logistic Regression can be applied to administrative workforce data to predict task completion outcomes.

The results suggest that administrator experience, training, and team information can be useful predictors for understanding task completion patterns. The model provides a foundation for identifying potential task-completion risks and supporting more informed administrative planning.

*Note: Model performance reflects the reported results from this analysis and should be validated on an independent dataset before being used for real-world decisions.*
