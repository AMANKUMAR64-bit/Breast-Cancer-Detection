# Breast-Cancer-Detection
This project leverages machine learning techniques to enhance breast cancer detection. By analyzing medical data with various ML models, we aim to improve early diagnosis and classification accuracy. The repository includes data preprocessing, model training, and evaluation scripts for a robust detection system.
## Data Source
The data for this project is taken from Kaggle.
## Data Description
The data taken from Kaggle includes multiple columns.
### Attribute Information:

1) ID number
2) Diagnosis (M = malignant, B = benign)
3-32)

Ten real-valued features are computed for each cell nucleus:

a) radius (mean of distances from center to points on the perimeter)
b) texture (standard deviation of gray-scale values)
c) perimeter
d) area
e) smoothness (local variation in radius lengths)
f) compactness (perimeter^2 / area - 1.0)
g) concavity (severity of concave portions of the contour)
h) concave points (number of concave portions of the contour)
i) symmetry
j) fractal dimension ("coastline approximation" - 1)

The mean, standard error and "worst" or largest (mean of the three
largest values) of these features were computed for each image,
resulting in 30 features. For instance, field 3 is Mean Radius, field
13 is Radius SE, field 23 is Worst Radius.

All feature values are recoded with four significant digits.

Missing attribute values: none

Class distribution: 357 benign, 212 malignant

## Approach
This project involves classical machine learning tasks such as exploring and cleaning data, building models, and testing their performance. It also includes experimenting with various machine learning algorithms to identify the most effective ones for the problem at hand.

## Data Cleaning
#### Duplicate Removal 
We detect and eliminate duplicate records to keep the dataset unique, avoiding redundancy and preserving data integrity.

#### Outlier Handling 
Outliers that could distort results and affect model accuracy are identified and managed using Interquartile Range (IQR) methods. This ensures extreme values are appropriately addressed, enhancing dataset reliability.

#### Data Scaling 
To standardize data and ensure uniform feature impact, we apply scaling techniques like StandardScaler. This step normalizes data into a consistent range, boosting model performance and convergence.
## Model Selection
Numerous models were tested, but Logistic Regression with a C value of 1 was selected as the final model.
## Hyperparameter Optimization
We tested multiple models and adjusted their hyperparameters to find the optimal configuration for breast cancer detection, aiming to enhance model accuracy and performance.
## Model Dump
Used joblib to dump the selected model.
## Model Accuracy
97%
### THANKS!!!
