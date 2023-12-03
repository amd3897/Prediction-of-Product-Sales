# Prediction of Product Sales
The task is to predict the sales of food items at various stores to increase profit.

**Author: Aziz M. Duaibes**

### Business problem:
The task is to make good prediction of the sales of food items at various stores.

## Potential Stakeholders:
Grocery stores' owners.

## Data:
Data used for this project is attatched here.

**https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view?usp=sharing**


## Methods
- Data cleaning and imputation.
- Exploratory data analysis and visualization.
- Feature inspection.
- Preprocessing data and preparing it for machine learning.
- Modeling.

## Results
Results show that the model was a success in making considerably very good prediction of sales with R^2 score = 0.595

*The R^2 score is used to evaluate the goodness of fit of a regression model and its value is between 0 and 1*

#### The relation between Fat Content of products (feature) and the Sales (target).
![image](https://github.com/amd3897/Prediction-of-Product-Sales/assets/145266280/40fe3378-ffbe-4f54-818c-50e345338bf9)

The graph above show the relation between a specific feature and the sales (target value), in this case the fat content of products. Note that both types have nearly the same average of sales (around 2000).

#### The relation between the type of area in which the store is located (feature) and the Sales (target).
![image](https://github.com/amd3897/Prediction-of-Product-Sales/assets/145266280/298381cc-f47c-4255-95ef-dc2f997a5c0b)

The graph above shows the relation between the type of area in which the store is located and the sales. Both Tier 2 & Tier 3 are around 2000 (of sales), although Tier 3 has some very large values.


## Model
- The model is generated by RandomForest. The model performs well in predicting the sales.
- Mean Absolute Error = 734.918
- Mean Squared Error = 1,116,137.201
- Root Mean Square Error = 1,056.474
- R^2 score = 0.595
- The R^2 score is used to evaluate the goodness of fit of a regression model. The greater the R^2 score the better the results.

## Model Insights
### Feature Importances
![image](https://github.com/amd3897/Prediction-of-Product-Sales/assets/145266280/8c623071-6e42-4544-974c-0ec7809d6271)

The top 5 features that most affect the model's prediction are shown above. They are (in order):
- Item MRP (Maximum Retail Price): That is a manufacturer-calculated price that is the highest price that can be charged for a product.
- Outlet Type (Grocery Store): Which means grocery stores play a major role in predicting the sales.
- Item Visibility: How much visible the item is for the customer is highly important.
- Item Weight: The weight of the product could play a very important role since customers prefer to buy light things more than heavy things.
- Outlet Identifier (OUT027): The store ID somehow plays an important role.

### Visualizing Coefficient
![image](https://github.com/amd3897/Prediction-of-Product-Sales/assets/145266280/9de08f5f-6fc8-40be-9a77-948fc6dcacef)

Our Linear Regression Coefficients are shown above.
- Our model assumed a baseline score of 2.728
- Coefficients that Positively Influence the Sales:
  - Outlet ID (OUT013):
    The store with this ID increases the sales by  1.728.
  - Outlet Establishment Year:
    The year the outlet was built in increases the sales by 1.584.
  - Outlet ID (OUT045):
    The store with this ID increases the sales by  1.220.
  - Outlet Size:
    The outlet size increases the sales by 1.056

- Coefficients that Negatively Influence Final Grade:
  - Outlet Type (Supermarket Type1):
    This type negatively affects the sales by 2.856.
  - Outlet Type (Supermarket Type2):
    This type negatively affects the sales by 2.240.
  - Outlet ID (OUT018):
    The store with this ID negatively affects the sales by  1.893.
  - Outlet Location Type (Tier 3):
    The location negatively affects the sales by 1.396.
  - Outlet ID (OUT049):
    The store with this ID negatively affects the sales by  0.819.

    
## Recommendations:
As you can see from visualizing coefficients, you can further enhance the coefficients that positevely influence the sales, by by building bigger stores, new ones or rennovate old ones. You can also reduce the effect of the negative factors, such as, upgrading supermarkets of type 1 and type 2, or upgrade the location of some stores.


## Limitations & Next Steps
The model is ready to be deployed.


### For further information
For any additional questions, please contact **duaziz97@gmail.com**
