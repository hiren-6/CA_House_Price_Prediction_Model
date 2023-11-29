# CA_House_Price_Prediction_Model
The repository provides python notebook for running codes, readme file and folder containing results picture.


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
## Model Performance Metric

| Metric | Score   |
|--------|---------|
| R2     | 0.5937  |
| MSE    | 0.5349  |

### Significance of Metrics

#### R-squared (R2)

R-squared is a statistical measure that represents the proportion of the variance in the dependent variable that is predictable from the independent variable(s). An R2 score of 0.5857 indicates that approximately 58.57% of the variability in the target variable is explained by the model. A higher R2 score suggests a better fit of the model to the data.

#### Mean Squared Error (MSE)

Mean Squared Error is a measure of the average squared difference between the predicted and actual values. The MSE score of 0.5602 indicates a relatively low average squared error, suggesting that, on average, the model's predictions are close to the actual values. Lower MSE values are desirable as they indicate better model performance.

### Overall Significance

- The R2 score provides an understanding of how well the independent variables explain the variability in the dependent variable.
- The MSE score quantifies the average squared difference between predicted and actual values, giving insights into the accuracy of predictions.
- A good model typically has a high R2 score and a low MSE, indicating a strong fit to the data and accurate predictions.

These metrics collectively offer valuable insights into the model's performance and its ability to generalize well to new, unseen data.

**Explore, Collaborate, Contribute!**

**Happy Coding!**

## Acknowledgements

 - [Scikit-learn](https://scikit-learn.org/stable/about.html)
 - [123ofAI](https://123ofai.com/)
 - [Readme Editor](https://readme.so/editor)
 - [StatLib Repository](https://www.dcc.fc.up.pt/~ltorgo/Regression/cal_housing.html)
 - [Google Colab](https://colab.google/)
## License

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
