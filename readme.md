# Stock Price Prediction using a GRU Model

This project uses a Gated Recurrent Unit (GRU) neural network to predict the closing price of Apple Inc. (AAPL) stock. The model is built and documented in a Jupyter Notebook running within Visual Studio Code.

## Project Overview

The goal of this project is to build a time-series forecasting model that learns from historical stock data to predict future prices. The process includes:
1.  **Data Loading and Cleaning**: Loading historical AAPL stock data and handling missing values caused by market holidays.
2.  **Data Preparation**: Scaling the data and creating time-series sequences suitable for a recurrent neural network.
3.  **Model Building**: Constructing a multi-layer GRU model with Dropout for regularization.
4.  **Training and Evaluation**: Training the model on 80% of the data and evaluating its performance on a validation set (10%) and a final, unseen test set (10%).
5.  **Visualization**: Plotting the model's predictions against the actual prices to visually assess its performance.

## Dataset

The dataset used is `AAPL.csv`, which contains the daily stock prices for Apple Inc. from 2006 to early 2020.

## Technologies Used
* Python 3 in a Jupyter Notebook environment
* Pandas
* NumPy
* TensorFlow / Keras
* Scikit-learn
* Matplotlib

## How to Run

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-Maheswar9/stock-closing-price-prediction-gru.git]
    cd stock-price-prediction-gru
    ```

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows, use `env\Scripts\activate`
    ```

3.  **Install the required packages:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Run the Notebook:**
    Open the project folder in Visual Studio Code. Open the `stocks_prediction.ipynb` file and run the cells sequentially. Ensure that your VS Code is using the Python interpreter from the virtual environment you created.

## Results

The model successfully captures the trend of the actual stock price, demonstrating its ability to learn from historical time-series data.

### Key Metrics
The model's performance was evaluated using Root Mean Squared Error (RMSE) on the scaled data:
* **Train RMSE**: 0.01
* **Validation RMSE**: 0.03
* **Test RMSE**: 0.10

The low RMSE on the test set indicates that the model generalizes well to new, unseen data.

### Visualization
The final plot visually confirms the model's accuracy, showing a close match between the predicted and actual prices on the test set.

