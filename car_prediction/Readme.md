## TASK 1
### CAR PRICE PREDICTION

This project aims to understand the key factors that influence car prices and develop an accurate predictive model to estimate prices based on vehicle features. With the help of machine learning techniques such as Logistic Regression, Random Forest and XGBoost, the project explores the relationship between car technical specifications and price, providing deep insights that can help the automotive industry determine better pricing strategies.

#### DATASET DESCRIPTION
The dataset used in this project includes various important information about the technical specifications and prices of cars of different vehicle types. These features fall into two main categories: numerical features and categorical features. The following is a description of each feature analyzed:
Numerical Features:
- Horsepower: Measures the power of the engine, which is usually directly proportional to the price of the car, as higher engine performance tends to increase the value of the vehicle.
- Engine Size: The capacity of a car's engine, which is often associated with a higher price.
- Curb Weight: The weight of the car without cargo or passengers. Heavier cars usually include additional construction or features that increase their value.
- City MPG and Highway MPG: Fuel efficiency in the city and on the highway. High fuel efficiency can be an attractive factor for consumers.
- Dimensions (Car Length, Width, Height): The physical size of the vehicle, which can also be a determinant of a car's price as it is often related to functionality and comfort.

Categorical Features:
- Car Body Type: The body type of the car such as sedan, hatchback, wagon, and convertible, which indicates the intended use of the car and can affect its price.
- Drive Wheel Type: The wheel drive system such as FWD (Front-Wheel Drive), RWD (Rear-Wheel Drive), or AWD (All-Wheel Drive), which affects the performance and price of the car.\Fuel Type: The type of fuel used (gasoline or diesel), which can affect efficiency and running costs.
- Engine Type: The type of engine such as DOHC or SOHC, which may be related to technology or performance that affects price.

### Steps of Analysis
- Data Exploration: Conduct exploratory data analysis (EDA) to understand the distribution of features and the initial relationship between key features and car prices.
- Data Cleaning: Resolving missing or anomalous values, and encoding categorical features for use in machine learning models.
- Model Selection and Training: Applying several prediction models, including Linear Regression, Random Forest, and XGBoost, to find the model with the best accuracy.
- Model Evaluation: Using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R²) to evaluate model performance.
- Interpretation and Insights: Analyze the model results to gain insights into the features that affect prices the most, and summarize the results in a way that is useful to stakeholders.

## KEY INSIGHTS
### Data Exploration and Key Feature Identification
From the data exploration, it can be seen that some features have a strong relationship with car prices. The key features that show a high correlation to price are horsepower, engine size, curb weight, and car body type.
- Engine Power and Engine Size: Cars with greater horsepower and engine size tend to have higher prices. This is natural, as higher engine performance gives the vehicle more value in terms of speed, acceleration, and durability.
- Curb Weight: Cars with greater weight usually have stronger construction and materials as well as additional features, which overall increases production costs and ultimately the selling price.
- Car Body Type and Wheel Drive Type: The body type and wheel drive system (such as rear-wheel drive/RWD or all-wheel drive/AWD) also affect the price. For example, cars with AWD or RWD are usually priced higher than those with FWD, due to their better performance and handling capabilities in various road conditions.

The findings indicate that engine performance, size, weight, as well as body type and wheel drive are important factors in determining car prices. These insights are valuable for setting prices that are more competitive and appropriate to the market segment.

### Prediction Model Selection and Evaluation
- Linear Regression provided an initial baseline, but was less than optimal as it did not fully capture the non-linear relationship between features and car price.
- Random Forest showed the best results with an R-squared value of 0.808, which means the model was able to explain about 80.8% of the price variation in the data. This makes it the best model for price prediction in this dataset.
- XGBoost also performed well with an R-squared of 0.767, slightly below Random Forest but still quite reliable in capturing complex patterns.
These results show that non-linear algorithm-based models, such as Random Forest and XGBoost, are more suitable for predicting car prices than simple linear models. These models show that the relationship between car features and price is non-linear, and more complex than what a simple linear model can capture.

### Model Performance Evaluation
Based on the Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE ) evaluation metrics, Random Forest has the lowest error rate compared to other models, with an MAE of 1265.86. This means that the average price prediction error is about 1265 units.

The low error rate indicates that Random Forest is a very accurate choice for car price prediction in this dataset. The model can provide price estimates that are close to the actual price, which is valuable for practical applications, especially in pricing strategies in the automotive industry.

## CONCLUSION

This analysis showed that car prices are highly influenced by factors such as engine performance, vehicle size, and wheel drive type. Random Forest emerged as the best predictive model with a high ability to capture complex relationships in the data. This accurate predictive model can support more informed and data-driven pricing decisions in the automotive industry, allowing manufacturers and dealers to set competitive and market-appropriate prices. In addition to improving predictive accuracy, this data-driven approach also provides insights into the key elements that determine car value, supporting more strategic decision-making.
