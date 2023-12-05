
## Project Title

# For ML Beginners: Predicting California House Pricing with Linear Regression Model
## Overview

Welcome to the machine learning project repository focused on forecasting housing prices using the California Housing dataset. This project employs a linear regression model, implemented in Python, to delve into the intricate dynamics of real estate economics.

**Key Features:**

**Accessible Starting Point:** This repository provides a user-friendly entry into the world of predictive analytics for beginner ML enthusiasts  who want to delve into machine learning in python.

**Python Implementation:** Dive into the codebase  in Python, a versatile and widely-used programming language in the field of machine learning.

**California Housing Dataset:** Leveraging the renowned dataset sourced from the 1990 U.S. census, this project explores the relationships between median house values and a set of eight crucial attributes, including median income, house age, and population.

**Practical Application:** Understand how machine learning can be practically applied to gain insights into real estate dynamics, offering a valuable resource for both learning and practical application.

To get started, download or clone the repository and follow our detailed documentation. Happy coding!"
## File Structure

- CA House Price Prediction Model.ipynb: Python Notebook containing the code for  model training and predictions.

- result/: Directory containing the scatter plots of training vs predict dataset 

- README.md: Project documentation providing an overview, usage instructions, and other relevant information.
## Steps

All the steps to process data and prepare for model are explained in python notebook. For quick learning, you can run this python codes on Google colab.
## Dataset Description

### Data Set Characteristics

- **Number of Instances:** 20,640
- **Number of Attributes:** 8 numeric, predictive attributes, and the target

### Attribute Information

1. **MedInc:** Median income in block group
2. **HouseAge:** Median house age in block group
3. **AveRooms:** Average number of rooms per household
4. **AveBedrms:** Average number of bedrooms per household
5. **Population:** Block group population
6. **AveOccup:** Average number of household members
7. **Latitude:** Block group latitude
8. **Longitude:** Block group longitude

### Missing Attribute Values

None

### Source

This dataset was obtained from the StatLib repository. [Link to the dataset](https://www.dcc.fc.up.pt/~ltorgo/Regression/cal_housing.html)

### Target Variable

The target variable is the median house value for California districts, expressed in hundreds of thousands of dollars ($100,000).
## **Model Optimization** 

We will run various machine learning techniques to optimize model performance.

### **Supervised learning**

**Filter Based Method**: Calculates dependencies on each features (univariate). This method shows that by selecting top 7 features out of 8 available features generate highest R2 score. However, top 3 features provide optimum R2 score of 0.58 and at the same, our model is now dependent on only top 3 features (MedInncome, Longitude, Latitude).

| K value | R2 Score   |
|---------|------------|
| 1       | 0.000513   |
| 2       | 0.459036   |
| 3       | 0.587496   |
| 4       | 0.567125   |
| 5       | 0.562701   |
| 6       | 0.588210   |
| 7       | 0.645204   |
| 8       | 0.606695   |


**Pearson Correlation** : Here, we will find certain overlapping parameters that impact the outcome (Housing price) in a same degree. We will remove this features and then re-calculate R2 score.

- Before removing any features: R2 = 0.5866
- Identified two pair of features: AveRooms and AveBedrms | Latitude and Longitude
- After dropping AveRooms and Longitude: R2 = 0.5249

This clearly shows feature removal has no impact on model performance improvement.

**Wrapper Based Methods**
- Recurive Feature Elimination: R2 = 0.5826
- Sequential Feature Selector: R2 = 0.5399

### **Unsuperervised**
- PCA: Dimenisonality Reduction technique that transforms the features into a new space where we can select features on the basis of variance captured (eigen values)
    - R2 Score: 0.6061


Overall, both supervised Filter based method and unsupervised PCA learning technique produces best R2 score for our learning model.

| Learning Method                   | R2 Score   |
|-----------------------------------|------------|
| Filter Based Method (k=7)         | 0.6452     |
| Filter Based Method (k=8)         | 0.6067     |
| PCA                               | 0.6061     |
| Filter Based Method (k=6)         | 0.5882     |
| Filter Based Method (k=3)         | 0.5875     |
| Pearson Correlation (Before)      | 0.5866     |
| Recursive Feature Elimination     | 0.5826     |
| Filter Based Method (k=4)         | 0.5671     |
| Filter Based Method (k=5)         | 0.5627     |
| Sequential Feature Selector       | 0.5399     |
| Pearson Correlation (After)       | 0.5249     |
| Filter Based Method (k=2)         | 0.459      |
| Filter Based Method (k=1)         | 0.0005     |


## Acknowledgements

 - [Scikit-learn](https://scikit-learn.org/stable/about.html)
 - [123ofAI](https://123ofai.com/)
 - [Readme Editor](https://readme.so/editor)
 - [StatLib Repository](https://www.dcc.fc.up.pt/~ltorgo/Regression/cal_housing.html)
 - [Google Colab](https://colab.google/)
## License

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

