# Housing Price Prediction Model

## Overview
This project builds a prediction model to forecast housing prices using the Ames Housing Data Set. The dataset contains 79 variables—ranging from numerical measurements like house size to categorical details such as ceiling type. By leveraging feature engineering, binarization, and Principal Component Analysis (PCA), the dimensionality of the data was reduced, thereby enhancing the model’s performance. Three regularized regression techniques were applied: Ridge Regression, Lasso Regression, and Elastic Net Regularization.

## Dataset Description
The Ames Housing Data Set offers a rich variety of features:
- **79 Variables:** A mix of numerical and categorical variables.
- **Examples of Features:** House size, type of ceiling, and other property-related characteristics.
  
This diversity allows the model to capture complex patterns affecting housing prices.

## Feature Engineering & Dimensionality Reduction
Before modeling, several preprocessing techniques were applied:
- **Binarization:** Categorical variables were converted into binary (dummy) variables to make them compatible with regression models.
- **Principal Component Analysis (PCA):** Employed to reduce dimensionality, PCA helped in isolating the most significant features, reducing noise and multicollinearity.

## Modeling Techniques
Three different regression models with regularization were implemented to predict housing prices:

### 1. Ridge Regression
- **Optimal Alpha Values:** 
  - Primary optimal value: **30.0**
  - An alternate value also considered: **24.0**
- **Performance:**
  - **RMSE on Training Set:** 0.1154057232845079
  - **RMSE on Test Set:** 0.11642721377799554

### 2. Lasso Regression
- **Optimal Alpha Value:** **0.0006**
- **Performance:**
  - **RMSE on Training Set:** 0.11411150837458059
  - **RMSE on Test Set:** 0.11583213221750702

### 3. Elastic Net Regularization
- **Optimal Parameters:**
  - **l1_ratio:** **1.0**
  - **Alpha:** **0.0006**
- **Performance:**
  - **RMSE on Training Set:** 0.11411150837458059
  - **RMSE on Test Set:** 0.11583213221750702

*Note:* The Lasso and Elastic Net models produced identical RMSE values, indicating that an l1_ratio of 1.0 essentially reduces Elastic Net to Lasso in this case.

## Conclusion
The results indicate that the combination of feature engineering and regularized regression techniques effectively predicts housing prices. Among the tested models, both Lasso and Elastic Net achieved lower RMSE values compared to Ridge Regression, highlighting the importance of selecting the appropriate regularization strategy for datasets with high dimensionality.

## Getting Started

### Prerequisites
- **Python 3.x**
- Required libraries:
  - numpy
  - pandas
  - scikit-learn
  - matplotlib
  - seaborn

### Installation
1. **Clone the Repository:**
   ```bash
   git clone <repository_url>
   cd <repository_directory>
   ```
2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

### Running the Model
You can run the prediction model either via a Python script or within a Jupyter Notebook:
- **Python Script:**
  ```bash
  python run_model.py
  ```
- **Jupyter Notebook:**
  Open the provided notebook file and run the cells sequentially.

## License
This project is licensed under the MIT License.

## Acknowledgements
- **Data Source:** Ames Housing Data Set.
- **Inspiration:** The data science community for insights into advanced feature engineering and regularization techniques.
