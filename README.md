# employee_salary_prediction_ml

**Pandas** is used for working with datasets. It provides a structure called a Data Frame, which looks like a table.
**NumPy** is used for numerical calculations.
Matplotlib is used to create graphs.
Seaborn is a visualization library built on top of Matplotlib.

---------------------------------------------------------------
from sklearn.model_selection import train_test_split

train_test_split() divides your dataset into:
*Training data
*Testing data

The model learns from training data and is evaluated using testing data.

------------------------------------------------------------------------------
from sklearn.preprocessing import LabelEncoder

LabelEncoder converts categorical text values into numbers.

For example:
Bachelor's → 0
Master's   → 1
PhD        → 2

Machine learning models generally require numerical inputs.

--------------------------------------------------------------------------------
from sklearn.linear_model import LinearRegression

This imports the Linear Regression algorithm.
Linear Regression is a basic supervised learning algorithm used for predicting continuous values.
It assumes there’s a linear relationship between the input variables (features) and the output variable (target).

Linear Regression tries to find the best mathematical relationship between the input features and the salary.

For one input, the basic equation is:

 y = b_0 + b_1x 

Where:

y = predicted value
x = input feature
b₀ = intercept
b₁ = coefficient/slope

------------------------------------------------------------------------------
from sklearn.ensemble import RandomForestRegressor

This imports the Random Forest Regression algorithm.
Random Forest is an ensemble learning method that combines multiple decision trees to make more accurate and stable predictions.
Each tree is trained on a random subset of the data and features.

Random Forest is a supervised machine learning algorithm that combines multiple decision trees to make a prediction.

-------------------------------------------------------------------------------

1. MAE — Mean Absolute Error

MAE tells us the average amount by which our predictions are wrong.

Formula:
MAE=n1​∑∣Actual−Predicted∣

Remember: Lower MAE = better

Your project:
Linear Regression → 11,508
Random Forest     →  9,871

-----------------------------------------------------------------------------------

2. RMSE — Root Mean Squared Error

RMSE also measures prediction error, but it penalizes large errors more heavily.

Formula:
RMSE=n1​∑(Actual−Predicted)2
​
Remember:

Lower RMSE = better

Your project:

Linear Regression → 15,975
Random Forest     → 13,897

---------------------------------------------------------------------------------

R² — R-Squared

R² tells us how much of the variation in the target variable is explained by the model.
Formula
R^2=1−(SStot/SSres)
	​
Where:

SSres = sum of squared prediction errors
SStot = total variation in the actual target values
	​
Generally:

R² closer to 1 → better explanatory fit
R² around 0 → model explains little of the variation
R² < 0 → model can perform worse than a simple baseline based on the mean

------------------------------------------------------------------------------------------

	​
