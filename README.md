### Detecting Spam Email
This project aims to develop a machine-learning model that can automatically classify emails as either spam or non-spam (ham). The model will be trained on a dataset of labeled emails, where each email is associated with a class label indicating whether it is spam (1) or non-spam (0).

# Project Components:

1. Dataset:
The project starts with a labeled dataset containing emails and corresponding class labels (spam or non-spam).
The dataset is split into training and testing sets to evaluate the model's performance.

2. Text Preprocessing: Text data preprocessing is essential to clean and prepare the email content for analysis.
Steps may include removing stop words, punctuation, special characters, and stemming or lemmatization.

3. Feature Engineering: The raw text data is converted into a numerical format suitable for machine learning models.
The CountVectorizer is used to create a token matrix, representing the count of each word in the emails.

5. Model Selection: Logistic Regression is chosen as the classification algorithm for its simplicity and effectiveness in binary classification tasks.
The model is trained on the training set, learning the optimal weights for the features.

6. Model Training: The logistic regression model is trained using the training data. During training, the model adjusts its weights to minimize the logistic loss or cross-entropy loss.

7. Model Evaluation: The trained model is evaluated on the testing set to assess its performance on unseen data.
Evaluation metrics such as accuracy, confusion matrix, and classification report are calculated to measure the model's effectiveness.

8. Fine-Tuning: If needed, hyperparameter tuning and cross-validation can be performed to optimize the model's performance.

9. Prediction: Once the model is trained and evaluated, it can be used to predict the spam or non-spam status of new, unseen emails.

# How Logistic Regression Works : 
# 1.Hypothesis Function:
In logistic regression, the logistic function (also called the sigmoid function) is used as the hypothesis function. The logistic function is defined as:

![image](https://github.com/NehaSJ99/Spam_email_detection/assets/72608245/c4e01f65-f34b-4cdd-bd2e-fea4c5f5d474)

# 2.Training Process:

The goal of logistic regression is to find the optimal values for the weights (\( \theta \)) that minimize the difference between the predicted probabilities and the actual class labels.

The training process involves defining a cost function (also called the logistic loss or cross-entropy loss) that measures the difference between the predicted probabilities and the actual labels. The cost function is defined as:
![image](https://github.com/NehaSJ99/Spam_email_detection/assets/72608245/c9c600cc-aa1f-4ea2-a370-d2d8601bea3a)


# 3. Optimization:

Gradient Descent or other optimization algorithms are used to minimize the cost function by updating the weights iteratively. The gradient of the cost function with respect to the weights is computed, and the weights are updated in the opposite direction of the gradient.

![image](https://github.com/NehaSJ99/Spam_email_detection/assets/72608245/a926da51-5e53-4249-93c7-5725dc56183b)


# 4. Prediction:

Once the model is trained, predictions can be made for new examples by using the learned weights in the logistic function. If \( h_\theta(x) \) is greater than or equal to 0.5, the predicted class is 1; otherwise, it is 0.

Logistic regression is a powerful and widely used algorithm for binary classification tasks. It is interpretable, relatively simple, and works well in many real-world scenarios.

# Results and Conclusion:
The project concludes with an analysis of the model's performance and effectiveness in accurately classifying spam and non-spam emails. Insights gained from the project can be used to enhance the model further or deploy it for real-world applications, such as an email filtering system. The logistic regression model serves as a reliable tool for automated email spam detection, contributing to improved email security and user experience.
