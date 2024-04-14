# **LEVEL-1**
<br />
<br />

## **Task 1: Linear and Logistic Regression - HelloWorld for AI-ML**

<br />


1. **Linear Regression** - Predict the price of a home, based on multiple different variables.
`Use sci-kit’s linear_model.LinearRegression()`
<br />

Certainly! Here's a brief explanation of both linear and logistic regression:

### Linear Regression:
Linear regression is a statistical method used to model the relationship between a dependent variable (target) and one or more independent variables (features) by fitting a linear equation to observed data. The basic form of a linear regression equation with one independent variable is:

\[ y = mx + b \]

- \( y \) represents the dependent variable (target).
- \( x \) represents the independent variable (feature).
- \( m \) represents the slope of the line (the change in \( y \) with respect to \( x \)).
- \( b \) represents the intercept (the value of \( y \) when \( x = 0 \)).

Linear regression aims to find the best-fitting line that minimizes the difference between the observed values and the values predicted by the model. It is commonly used for predicting continuous outcomes, such as predicting house prices based on square footage, number of bedrooms, etc.


link: https://colab.research.google.com/drive/1JQQ0DanRt-UakMghQyESqg-RoddcA1nu?usp=sharing


<br />

2. **Logistic Regression** - Train a model to distinguish between different species of the Iris
flower based on sepal length, sepal width, petal length, and petal width.
`Use sci-kit’s linear_model.LogisticRegression`

<br />

### Logistic Regression:
Logistic regression is a statistical method used for binary classification tasks, where the target variable has only two possible outcomes (e.g., yes/no, 1/0). However, it can also be extended to handle multi-class classification problems (e.g., distinguishing between different species of flowers, as in the Iris dataset).

Instead of fitting a straight line to the data, logistic regression fits an S-shaped logistic function (sigmoid function) to estimate the probability that a given input belongs to a certain class. The logistic function maps any real-valued number into a value between 0 and 1, making it suitable for classification tasks.

The logistic regression equation can be represented as follows:

\[ P(y=1|x) = \frac{1}{1 + e^{-(mx + b)}} \]

- \( P(y=1|x) \) represents the probability that the target variable \( y \) equals 1 given the input features \( x \).
- \( e \) represents the base of the natural logarithm.
- \( m \) represents the coefficients (weights) associated with the features.
- \( b \) represents the intercept.

Logistic regression models are trained to learn the optimal weights and bias that maximize the likelihood of the observed data belonging to their respective classes. It is commonly used in various fields such as healthcare (predicting disease occurrence), marketing (customer churn prediction), and finance (credit risk assessment).

<br />

link: https://colab.research.google.com/drive/1b5XWFzaAi7tAK0iSsLklZxOAwsLpnphl?usp=sharing

<br />

![image](https://github.com/HemaShenoy/images/assets/122464897/89d93d57-9141-4b60-a1c6-8d6374107f55)


<br />





## **Task 2 - Matplotlib and Data Visualisation**
<br />

### I.Explore the various basic characteristics to plots as given below with python libraries:
<br /><br />
 1.Import Libraries


 2.Set Axes Label and Limits


 3.Create a Figure with Multiple Plots using Subplot

 
 4.Add a Legend to the Plot
 

 5.Save Your Plot as PNG

### II. Explore the given plot types:

<br />

 1.Make a multivariate distribution for the given dataset using the given dataset for a classification task. Understand an elementary idea of clustering, that you will explore in more detail later.

[here](https://github.com/HemaShenoy/marvel)


LINK:  https://colab.research.google.com/drive/1FTyIpK4r-2wqp9-qnCN9sZuHm3Gup3bo?usp=drive_link

<br />
<br />

---


## **Task 3 - Numpy**
<br />
<br />
NumPy is a powerful numerical computing library for Python. It provides support for large, multi-dimensional arrays and matrices, along with mathematical functions to operate on these arrays. NumPy is a fundamental package for scientific computing with Python.
<br />
<br />



### Generating an Array by Repeating a Small Array Across Each Dimension:

```python
import numpy as np

# Small array
small_array = np.array([[1, 2], [3, 4]])

# Repeat the small array along each dimension
repeated_array = np.tile(small_array, (3, 2))

print("Small Array:")
print(small_array)

print("\nArray by Repeating Small Array:")
print(repeated_array)
```
<br />

![Scr](https://github.com/HemaShenoy/images/assets/122464897/8c312041-daca-4b1d-b381-dec54b785126)

<br />


### Generating an Array with Element Indexes in Ascending Order:

```python
import numpy as np

# Specify the shape of the desired array
array_shape = (4, 5, 3)

# Generate an array with element indexes in ascending order
index_array = np.arange(np.prod(array_shape)).reshape(array_shape)

print("Array with Element Indexes:")
print(index_array)
```
<br />

![Scre6](https://github.com/HemaShenoy/images/assets/122464897/35544b44-b348-484d-99a5-6372965baa93)

<br />

LINK:https://colab.research.google.com/drive/101UNvWYXa9dZ5lMrXQCD_Iybag6oBE2P?usp=sharing
<br />

---

<br />



## **Task 4 - Metrics and Performance Evaluation**
<br />
<br />

### Understanding Regression Metrics in Scikit-Learn

Regression models predict continuous numerical values, and scikit-learn provides various algorithms like Linear Regression, Decision Trees, Random Forests, and Support Vector Machines (SVM). Before diving into metrics, let's grasp some key concepts:

### 1. True Values and Predicted Values:

- **True Values:** Actual target values in your dataset.
- **Predicted Values:** Values your model predicts.

### 2. Evaluation Metrics:

Metrics help measure how well a regression model fits the data. Key metrics include:

### Types of Regression Metrics:

#### Mean Absolute Error (MAE):
- Measures average absolute differences between actual and predicted values.
- **Formula:** \(MAE = \frac{1}{n} \sum_{i=1}^{n} |x_i - y_i|\)

#### Mean Squared Error (MSE):
- Measures average squared differences between actual and predicted values.
- **Formula:** \(MSE = \frac{1}{n} \sum_{i=1}^{n} (x_i - y_i)^2\)

#### R-squared (R²) Score:
- Indicates the percentage of variance in the dependent variable explained by independent variables.
- **Formula:** \(R^2 = 1 - \frac{SSR}{SST}\)

#### Root Mean Squared Error (RMSE):
- Measures the square root of the MSE.
- **Formula:** \(RMSE = \sqrt{MSE}\)
<br />
![Scre)](https://github.com/HemaShenoy/images/assets/122464897/e8f53f32-6760-48e5-b902-0b31d44c0852)

### Example: Mean Absolute Error (MAE)

```python
from sklearn.metrics import mean_absolute_error

true_values = [2.5, 3.7, 1.8, 4.0, 5.2]
predicted_values = [2.1, 3.9, 1.7, 3.8, 5.0]

mae = mean_absolute_error(true_values, predicted_values)
print("Mean Absolute Error:", mae)
```
<br />

![Scre)](https://github.com/HemaShenoy/images/assets/122464897/0c81863c-8231-428f-8347-eb6a1dd82918)

<br />


### Conclusion:

Understanding these metrics is crucial for assessing regression model performance. In a practical example using scikit-learn, we applied metrics to evaluate a Linear Regression model on house prices. This process helps gauge the model's accuracy and effectiveness in predicting continuous values.

<br />

---

<br />

## **Task 5 - Linear and Logistic Regression - Coding the model from SCRATCH**

<br />
<br />


### Linear Regression from Scratch:

Linear regression is a linear approach to modeling the relationship between a dependent variable and one or more independent variables

```python
import numpy as np
import matplotlib.pyplot as plt

# Generate  linear-like data
np.random.seed(42)
X = 2 * np.random.rand(100, 1)
y = 4 + 3 * X + np.random.randn(100, 1)

# Your Linear Regression Implementation
# ...

# Scikit-learn Linear Regression
from sklearn.linear_model import LinearRegression
sklearn_lr = LinearRegression()
sklearn_lr.fit(X, y)

# Plot the data and the linear regression line
plt.scatter(X, y, label='Data')
plt.plot(X, sklearn_lr.predict(X), color='red', label='Scikit-learn Linear Regression')
plt.xlabel('X')
plt.ylabel('y')
plt.title('Linear Regression')
plt.legend()
plt.show()
```




![121](https://github.com/HemaShenoy/images/assets/122464897/298df9c1-55bc-4ea9-8721-9d8997408972)

### Logistic Regression from Scratch:

Logistic regression is a statistical method for analyzing a dataset in which there are one or more independent variables that determine an outcome.

```python
import numpy as np
import matplotlib.pyplot as plt

# Generate  logistic-like data
np.random.seed(42)
X = 2 * np.random.rand(100, 1)
y = (X &gt; 1).astype(int).ravel()

# Your Logistic Regression Implementation
# ...

# Scikit-learn Logistic Regression
from sklearn.linear_model import LogisticRegression
sklearn_logreg = LogisticRegression()
sklearn_logreg.fit(X, y)

# Plot the data and the logistic regression curve
plt.scatter(X, y, label='Data')
X_test = np.linspace(0, 2, 300).reshape(-1, 1)
plt.plot(X_test, sklearn_logreg.predict_proba(X_test)[:, 1], color='red', label='Scikit-learn Logistic Regression')
plt.xlabel('X')
plt.ylabel('y')
plt.title('Logistic Regression with Complicated Data')
plt.legend()
plt.show()
```


![1313](https://github.com/HemaShenoy/images/assets/122464897/339f82e2-a486-4b58-a971-53b99cdad142)




In this example, we generate a dataset with a logistic-like relationship. 






Link: https://colab.research.google.com/drive/1rR699_0qcK9ZsA_xHymq1XMS4zrYmzmS?usp=sharing
<br />
<br />

---

<br />

## **Task 6:K- Nearest Neighbor Algorithm**

<br />

Understand the K-Nearest Neighbour Algorithm and implement it, first with a built in interface
and next, from scratch. Compare the results for both with the indicated datasets.
References:
1. Implement KNN using sci-kit’s neighbors.KNeighborsClassifier for multiple
suitable datasets

2. Understanding the algorithm

3. Implement KNN from scratch. Compare results with sci-kit’s built in method for different
datasets.

<br />
link: https://colab.research.google.com/drive/1XZz7kP93GMlifAZIQyyKuY1_fcllAG1X?usp=sharing

[here](https://github.com/HemaShenoy/marvel)

<br />

---

<br />

## **Task 7: An elementary step towards understanding Neural Networks**

<br />

 A blog about your understanding of Neural Networks and types like CNN, ANN, etc


[Decoding Convolutional Neural Networks: Insights into CNNs and ANNs](https://medium.com/@hemashenoy2017/decoding-convolutional-neural-networks-insights-into-cnns-and-anns-afcf188b8eea)

<br />
about Large Language Models at a basic level and make a blog post explaining how you would build GPT-4.

[Building GPT-4: A Comprehensive Guide to Creating Advanced Large Language Models](https://medium.com/@hemashenoy2017/building-gpt-4-a-comprehensive-guide-to-creating-advanced-large-language-models-074d29e86f05)

<br />

---

<br />


## **Task 8: Mathematics behind machine learning**

<br />

**Curve-Fitting-** Model a curve fitting for a simple function of your choice, on Desmos.

**1.Enter the Quadratic Function:**
In the input bar, enter the quadratic function:

f(x)=2x^2 +3x−5

![(16)](https://github.com/HemaShenoy/images/assets/122464897/1dedcfe4-d2d9-40db-9fd2-5a1b9887aafb)

<br />

**2.Add Noisy Data Points:**
To simulate real-world data with noise, we'll add some random data points around our quadratic function.

![ (17)](https://github.com/HemaShenoy/images/assets/122464897/9af30db5-c184-47ea-aa92-d655d779cb53)

![ (18)](https://github.com/HemaShenoy/images/assets/122464897/30ca4a58-6314-4797-be9f-5023ee40d472)

<br />

**3.Fit a Quadratic Curve:**

After adding the data points, click on the wrench icon in the upper right corner of the table to adjust settings.
Under "Regression Type," choose "Quadratic" to fit a quadratic curve to the data points.
Desmos will automatically fit the best quadratic curve to your data points.

<br />

**4.Visualize the Fit:**
You will see the original quadratic function 

f(x)=2x^2 +3x−5 plotted in blue, and the curve fitted to the noisy data points in red.

![(19)](https://github.com/HemaShenoy/images/assets/122464897/19b8ac96-2e8c-4fb1-af62-5d2f923006d4)

<br />

DESMOS LINKS:


[Quadratic Curve Fitting](https://www.desmos.com/calculator/dz8se30psf)

<br />

[Desmos Graph](https://www.desmos.com/calculator/z9zdwlypsq)

<br />

**Fourier Transforms-** Fourier transforms are perhaps the most important function approximators used today. Model a fourier transform for a function of your choice on MATLAB.

<br />
Example 1:
Square Wave Function:
The square wave function is periodic and can be defined as follows:


f(t)=   1,   if 0≤t
         −1,  if T/2≤t
​
  where T is the period of the square wave.    

<br />



![Screenshot (24)](https://github.com/HemaShenoy/images/assets/122464897/fe0459c4-1aa1-4f9b-81e6-f87f1cefa3ee)



<br />

![Screenshot (20)](https://github.com/HemaShenoy/images/assets/122464897/40b76a70-d2e2-4242-8074-77196eef49b4)





<br />
Example 2:

create a signal that consists of multiple sinusoidal components at different frequencies and perform its Fourier transform to analyze its frequency components.
<br />

![Screenshot (23)](https://github.com/HemaShenoy/images/assets/122464897/cee8cdf9-ab51-4083-b3b9-a371bc511f8f)


<br />

![Screenshot (22)](https://github.com/HemaShenoy/images/assets/122464897/c54a3455-d586-4858-b3a0-3f3404ec0e19)

<br />

---

<br />

## **Task 9: Data Visualization for Exploratory Data Analysis**

<br />

Use Plotly for data visualization. This is an advanced visualization library, more dynamic than
the generally used MatPlotlib or Seaborn.

[example 1](https://colab.research.google.com/drive/1U1f2q9sCEGC789wq46MnK4KoGX6Vajm3?usp=sharing)

<br />


![newplot](https://github.com/HemaShenoy/images/assets/122464897/dfab92d6-6270-4132-bd61-1177040eecb4)

[example 2](https://colab.research.google.com/drive/1y9QlUlGFXtbg5GX-NcGv7WFk41GXlABH?usp=sharing)

<br />

---

<br />


## **Task 10: An introduction to Decision Trees**
<br>

Decision Tree is a supervised learning algorithm that can be used for Regressive or Classifying
Tasks. It is a way to use conditional statements as a hierarchy so that, for an event, you get the
chances of given outcomes.

<br>

[here](https://github.com/HemaShenoy/marvel)

