# Tesla Stock Price Prediction Using TensorFlow and Keras

This project analyzes and predicts Tesla's stock prices using deep learning techniques with TensorFlow and Keras in Python.

## Dataset

- **Source:** [Kaggle - Tesla Stock Data](https://www.kaggle.com/datasets)
- **Period:** 2010 to 2022
- **Features:** Date, Open, High, Low, Close, Volume, etc.

## Project Steps

### 1. Data Collection

- Downloaded Tesla stock data from Kaggle.
- Loaded the dataset using pandas.

### 2. Data Preprocessing

- Checked for missing values and handled them.
- Converted date columns to datetime format.
- Sorted data by date.
- Normalized features using MinMaxScaler for better neural network performance.
- Split data into training and testing sets.

### 3. Exploratory Data Analysis (EDA)

- Visualized stock price trends over time.
- Plotted moving averages to observe trends and volatility.
- Analyzed correlations between features.

### 4. Model Building

- Used TensorFlow and Keras to build a Sequential LSTM (Long Short-Term Memory) model.
- Defined input shape based on time steps and features.
- Added LSTM layers and Dense output layer.

### 5. Model Training

- Compiled the model with loss function (mean squared error) and optimizer (Adam).
- Trained the model on the training dataset.
- Used validation split to monitor overfitting.

### 6. Model Evaluation

- Predicted stock prices on the test set.
- Inversed the scaling to get actual price values.
- Calculated evaluation metrics: RMSE, MAE.
- Plotted actual vs. predicted prices for visual comparison.

### 7. Results and Visualization

- Displayed prediction results with matplotlib.
- Compared model performance with baseline methods.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- scikit-learn
- tensorflow
- keras

## Usage

1. Clone the repository.
2. Install dependencies:  
   `pip install -r requirements.txt`
3. Run the main script:  
   `python main.py`

## References

- [Kaggle Tesla Stock Dataset](https://www.kaggle.com/datasets)
- [TensorFlow Documentation](https://www.tensorflow.org/)
- [Keras Documentation](https://keras.io/)

---

*This project demonstrates time series forecasting using deep learning for financial data analysis.*