# Newton's Method for Classification
This project involved implementing Newton's Method to perform logistic regression on a breast cancer dataset. The goal was binary classification of malignant vs benign tumors.

The dataset was split 80/20 into training and test sets. Sklearn libraries were used for data preprocessing and normalization.

Newton's Method is an optimization algorithm that helps find roots of equations. For logistic regression, it maximizes the logistic function to find optimal coefficient values.

Mathematically, Newton's Method uses this iterative update rule:
X2 = X1 - f(X1)/f'(X1)
Where X is the coefficient vector, f(X) is the logistic loss function, and f'(X) is its gradient.

In code, sklearn's LogisticRegresssion class was customized to implement Newton's update rule. This replaced the default solver with a custom Newton optimizer.

# Key steps included:
Calculate gradient of loss function
Plug gradient into update rule to recalculate coefficients
Repeat until convergence or max iterations
The customized Newton Regression model was trained on the training set. It achieved an accuracy of 96% on the test set, demonstrating effective learning.

# Overall, this project demonstrated:
Proficiency in sklearn and implementing optimization algorithms
Mathematical understanding of Newton's Method and derivatives
Customizing sklearn models for specialized techniques
Achieving high accuracy on breast cancer classification
