# APR_Assignment

1. Objective
This project applies Principal Component Analysis (PCA) for dimensionality reduction and Logistic Regression for classification on the Wine dataset. We first analyze classification performance using 5 principal components and then compare accuracy across different numbers of PCA components (1–13).


2. Dataset Description
• Samples: 178 wines
• Features: 13 chemical properties (e.g., alcohol, flavanoids, color intensity)
• Classes: 3 wine cultivars (59, 71, 48 samples)

3. Methodology

Step 1 – Data Standardization
• Standardize the dataset to zero mean and unit variance since PCA is sensitive to scale.

Step 2 – PCA with 5 Components
• Reduce 13 features into 5 uncorrelated principal components.

Step 3 – Logistic Regression Classifier
• Train a Logistic Regression classifier using the PCA-transformed data.

Step 4 – Accuracy vs Number of PCA Components
• Test classification accuracy across all possible PCA components to evaluate model performance.


4. Implementation & Results
• With 5 components, Logistic Regression achieved ~97% accuracy.
• Accuracy starts lower (~80–85%) with 1–2 PCs.
• Accuracy peaks at 5 PCs and stabilizes afterward.
• PCA reduced dimensionality effectively without losing accuracy.


5. Conclusion
• PCA reduced 13 features into fewer independent components.
• 5 components gave optimal accuracy (~97%), balancing efficiency and performance.
• Increasing components beyond 7 offered minimal gains.
• Logistic Regression worked effectively on PCA-transformed data.
