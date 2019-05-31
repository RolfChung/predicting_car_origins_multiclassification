# predicting_car_origins_multiclassification
## Summary


This project works with the <a href = "https://archive.ics.uci.edu/ml/datasets/Car+Evaluation">Car Evaluation Data Set</a> taken from the UCI Center for Machine Learning and Intelligent Systems. It includes technical information as variables and observations on various car types. The variables are used in this project as features to predict the origin of production of the car. The target variable or label is the origin of manufacturing. Is the origin of the car either North America, Europe, or Asia? 

<ul>
<li>mpg -- Miles per gallon, Continuous.</li>
<li>cylinders -- Number of cylinders in the motor, Integer, Ordinal, and Categorical.</li>
<li>displacement -- Size of the motor, Continuous.</li>
<li>horsepower -- Horsepower produced, Continuous.</li>
<li>acceleration -- Acceleration, Continuous.</li>
<li>year -- Year the car was built, Integer and Categorical.</li>
<li>origin -- Integer and Categorical. 1: North America, 2: Europe, 3: Asia.</li>
</ul>

As the target variable has got three unique origins to choose from, making predictions creates a multiclass classification. The one-versus-all method of multiclass classification is applied here. The one-versus-all method 
offers a good access as it transforms multiclass classification into multiple binary classification problems.
Three in this case. The data is split into train-test-split of 70 to 30. Two models with different number of
features each with 3 binary classification models are created here and evaluated with sklearn metrics functionality.

