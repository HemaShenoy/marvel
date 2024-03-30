


## Introduction
In this , we implement the K-Nearest Neighbor (KNN) algorithm using two approaches:
1. Using scikit-learn's `KNeighborsClassifier`.
2. Implementing KNN from scratch.

We will compare the performance of both implementations on a synthetic dataset and analyze their accuracy, efficiency, and scalability.

## 1: Using scikit-learn's KNeighborsClassifier

### Dataset Used
We used a synthetic dataset named "Classified Data" for this analysis. The dataset contains several features (WTT, PTI, EQW, SBI, LQE, QWG, FDJ, PJF, HQE, NXJ) and a target class column.

### Implementation Steps
1. Loaded the dataset using pandas and examined its structure.
2. Preprocessed the data by standardizing features using scikit-learn's `StandardScaler`.
3. Split the data into training and testing sets (70% training, 30% testing).
4. Trained the KNN model using scikit-learn's `KNeighborsClassifier` with various values of `n_neighbors` (k) ranging from 1 to 100.
5. Evaluated the model's performance using accuracy metrics on the testing data.

### Results and Analysis
- Accuracy vs. K Value:
  - K = 1: Accuracy = 92.67%
  - K = 3: Accuracy = 91.00%
  - K = 5: Accuracy = 92.67%
  - K = 10: Accuracy = 91.33%
  - K = 50: Accuracy = 91.67%
  - K = 100: Accuracy = 91.67%

The accuracy of the KNN model varies with the choice of K. The highest accuracy is achieved when K=1 and K=5, with a slight decrease as K increases beyond 5.

## 2: Implementing KNN from Scratch

### Implementation Steps
1. Defined a custom KNN algorithm from scratch including distance calculation (Euclidean distance) and neighbor selection.
2. Used the same training and testing data splits as in the scikit-learn implementation.
3. Trained and evaluated the scratch KNN model with various values of K similar to the scikit-learn approach.

### Results and Analysis
- Accuracy vs. K Value (Scratch Implementation):
  - K = 1: Accuracy = 90.67%
  - K = 3: Accuracy = 89.67%
  - K = 5: Accuracy = 91.00%
  - K = 10: Accuracy = 89.33%
  - K = 50: Accuracy = 87.67%
  - K = 100: Accuracy = 85.67%

The scratch implementation also shows varying accuracies with different K values, similar to the scikit-learn implementation. However, the accuracies are slightly lower compared to scikit-learn.

## 3: Analysis and Comparison

### Performance Comparison
- Both scikit-learn's KNN and the scratch implementation provide reasonable accuracies for this dataset.
- Scikit-learn's implementation offers higher accuracy and convenience due to optimized algorithms and feature scaling.

### Efficiency and Scalability
- Scikit-learn's KNeighborsClassifier is more efficient and scalable for large datasets due to its optimized algorithms and parallel processing capabilities.
- The scratch implementation may be suitable for small datasets but may not scale well for larger datasets.

### Conclusion
- Scikit-learn's KNeighborsClassifier provides a robust and efficient implementation of the KNN algorithm, suitable for most practical applications.
- Implementing KNN from scratch can be educational and useful for understanding the algorithm's internals, but it may not be optimal for large-scale or production use cases.

