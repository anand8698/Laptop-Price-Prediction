# Laptop-Price-Prediction
In this project, the goal was to build a machine learning model that predicts laptop prices based on a dataset containing various specifications of laptops. The dataset included features like the brand, model, CPU specifications, RAM, storage, GPU, screen resolution, weight, and more. The target variable was the laptop price (in Euros).

### Key Steps Involved:
1. **Data Cleaning**: 
   - Converted the **'Memory'** column to a numerical format, expressing the storage capacity in gigabytes (GB).
   - Processed the **'ScreenResolution'** column by extracting the width and height and splitting it into separate numerical columns.
   - Handled missing values, if any, and dropped unnecessary or redundant columns.

2. **Feature Engineering**:
   - Categorical columns (such as **'Company'**, **'Product'**, **'CPU_Company'**, etc.) were encoded using **one-hot encoding** to convert them into numerical representations that machine learning algorithms can process.

3. **Model Training**:
   - **Linear Regression** was chosen as the initial algorithm to train the model. This algorithm is often used for regression tasks, where the goal is to predict a continuous target variable (in this case, the price).
   - The dataset was split into training (80%) and testing (20%) sets to ensure the model was evaluated on unseen data.

4. **Model Evaluation**:
   - After training, the model's performance was evaluated using metrics like:
     - **Mean Absolute Error (MAE)**: Measures the average magnitude of errors in predictions.
     - **Mean Squared Error (MSE)**: Penalizes larger errors more than smaller ones, helping to identify models that are underperforming.
     - **R² Score**: Indicates how well the model's predictions fit the actual values (with 1 being a perfect fit).

### Machine Learning Algorithm: **Linear Regression**

**Linear Regression** is a simple and interpretable algorithm that models the relationship between a dependent variable (the laptop price) and one or more independent variables (laptop specifications). In this project:
- The **independent variables** (features) included various laptop specifications like **RAM**, **CPU frequency**, **screen resolution**, etc.
- The **dependent variable** was the **price**.

The model fits a straight line (or hyperplane in higher dimensions) to minimize the distance between the actual and predicted prices by finding the optimal weights for each feature.

### Why Linear Regression?
Linear regression was chosen for its simplicity and because it works well with numerical data. It allows us to understand the impact of each laptop specification on the price. For example, it can show how increasing the RAM or CPU frequency affects the predicted price.

### Potential Future Work:
- **Advanced Algorithms**: After establishing a baseline with Linear Regression, more advanced machine learning algorithms like **Random Forest**, **Gradient Boosting**, or even **Neural Networks** could be used to improve prediction accuracy.
- **Feature Scaling**: Algorithms like Support Vector Regression (SVR) might benefit from scaling the features.
- **Hyperparameter Tuning**: Further tuning of model parameters could enhance the model's performance.

This approach provides a foundation for understanding how machine learning can be applied to predict prices based on product specifications and can be extended or enhanced as needed.
