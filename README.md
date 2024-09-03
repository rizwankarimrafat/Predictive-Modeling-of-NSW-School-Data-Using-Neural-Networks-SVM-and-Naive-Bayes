# Predictive Modeling of NSW School Data Using Neural Networks, SVM and Naive Bayes

This project focuses on the predictive modeling of New South Wales (NSW) government school data using three distinct machine learning techniques: Neural Networks, Support Vector Machines (SVM), and Naive Bayes. The dataset utilized in this project encompasses comprehensive information on NSW government schools, including school locations, student enrolment numbers, and various other attributes. The primary objective of the project is to predict specific target variables, such as the "Opportunity Class" and "Late Opening School" status, using advanced classification algorithms.

## Key Analyses Performed

1. **Neural Networks:** The project initially employs a neural network model using the Keras library to predict the "Opportunity Class" of schools. The neural network consists of multiple dense layers with ReLU activation functions, culminating in a sigmoid output layer for binary classification. While the model achieved a high test accuracy of 94.22%, it struggled with classifying positive cases accurately, leading to zero precision and recall. To improve the model's performance, the target variable was switched to "Late Opening School," resulting in a significantly better model with 97.47% accuracy, 85.71% precision, and 82.76% F1-score.

2. **Support Vector Machines (SVM):** SVM was applied to the same dataset with label encoding for categorical variables. Various kernels were explored, including linear, polynomial, and radial basis function (RBF) kernels. The linear kernel produced the highest accuracy of 98.92%, demonstrating the effectiveness of SVM for this classification task. Hyperparameter tuning, particularly adjusting the cost function (C), played a crucial role in optimizing the model's performance.

3. **Naive Bayes:** The Naive Bayes classifier, specifically GaussianNB, was also tested on the dataset. Despite its simplicity and efficiency, the model achieved a lower accuracy of 70.04% compared to the neural network and SVM models. The model's F1-score of 61.84% reflected its moderate performance, with the ROC AUC score indicating its ability to differentiate between classes reasonably well. However, the independent assumption inherent in Naive Bayes limited its effectiveness for this dataset, which contains interdependent variables.

## Conclusion

This project provides a comparative analysis of different machine learning models applied to a complex educational dataset. The results indicate that while Neural Networks and SVM offer higher accuracy and better performance metrics, Naive Bayes serves as a simpler, though less powerful, alternative. The choice of target variable significantly impacts model performance, highlighting the importance of feature selection and preprocessing in predictive modeling. The findings from this project can be used to inform future research and practical applications in educational data science.

