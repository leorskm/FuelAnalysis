## Car Fuel Efficiency Analysis using Python

### Project Description
The objective of this project was to develop a supervised machine learning model capable of predicting the combined fuel efficiency (measured in miles per gallon, MPG) of vehicles. Predicting MPG is essential for assessing vehicle performance and environmental impact, a statistic relevant to stakeholders such as car manufacturers, regulators and consumers interested in fuel efficiency.

### Data Description
The dataset used in this project, derived from the `Dataset_Fuel types.csv` file, consists of 38,113 entries and includes various attributes related to vehicle specifications. Each entry corresponds to a specific vehicle model and includes data such as:
- **Vehicle Identification Details**: Model year, make, and model.
- **Engine Specifications**: Type of engine, number of cylinders, engine displacement, and whether the engine is turbocharged.
- **Fuel Efficiency Metrics**: City MPG, highway MPG, and combined MPG under different testing scenarios.
- **Emissions Data**: CO2 emissions metrics for different fuels.
- **Other Attributes**: Drive type, transmission type, and class of vehicle.

Columns with a significant amount of missing data (over 50% missing values) were removed, and the remaining missing values were imputed with the most frequent value for categorical variables and the median for numerical variables.

### Tasks Performed
Here are the detailed tasks performed throughout the project:

1. **Data Cleaning**:
   - **Handling Missing Values**: Columns with more than 50% missing data were dropped. Other missing values were imputed based on their data type—median for numerical attributes and mode for categorical attributes.
   - **Removing Duplicates**: Duplicate entries were removed to ensure the uniqueness of each data point.

2. **Feature Engineering**:
   - **Feature Selection**: Identified features with a strong correlation to the target variable (combined MPG). Selected features that significantly affect fuel efficiency based on domain knowledge and statistical measures.
   - **Standardization**: Numerical features were standardized to have zero mean and unit variance to ensure equal weighting in the machine learning model.

3. **Model Development**:
   - **Data Splitting**: The dataset was split into training (80%) and testing (20%) sets to evaluate the model's performance on unseen data.
   - **Model Training**: Trained a Gradient Boosting Machine (GBM) model due to its effectiveness in handling different types of features and capturing complex nonlinear relationships.
   - **Model Evaluation**: Evaluated using R-squared and Root Mean Squared Error (RMSE) metrics to assess the accuracy and performance of the model.

4. **Visualization**:
   - **Actual vs. Predicted Values**: Visualized to assess how closely the predicted values of MPG matched the actual values.
   - **Feature Importances**: Identified and visualized the importance of each feature used in the model to understand their impact on predicting vehicle fuel efficiency.

This project showcases a comprehensive approach to developing a predictive model with practical applications in understanding and improving vehicle fuel efficiency, using advanced machine learning techniques and thorough data handling practices.
