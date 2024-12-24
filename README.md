# Customer Churn Prediction

This project is a web application that predicts customer churn using a pre-trained machine learning model. The application is built using Streamlit for the web interface.

## Project Structure

- `streamlit_churn_app.py`: Streamlit application for customer churn prediction.
- `model.ipynb`: Jupyter Notebook for training and evaluating the machine learning model.
- `lgbm_model.pkl`: Pre-trained LightGBM model for churn prediction.
- `scaler.pkl`: Scaler used for preprocessing input data.

## Requirements

- Python 3.6+
- Jupyter Notebook
- streamlit
- scikit-learn
- pandas
- numpy
- matplotlib
- plotly
- xgboost
- lightgbm
- catboost


## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/customer-churn-prediction.git
    cd customer-churn-prediction
    ```

2. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

3. Place the `lgbm_model.pkl` and `scaler.pkl` files in the project directory.

## Model Training and Evaluation

1. Open the Jupyter Notebook:
    ```sh
    jupyter notebook model.ipynb
    ```

2. Follow the steps in the notebook to:
    - Load and preprocess the dataset.
    - Train the LightGBM model.
    - Evaluate the model's performance.
    - Save the trained model and scaler to `lgbm_model.pkl` and `scaler.pkl` respectively.

## Usage

### Streamlit Application

1. Run the Streamlit application:
    ```sh
    streamlit run streamlit_churn_app.py
    ```

2. Open your web browser and go to the URL provided by Streamlit.

### How to Use the Application

1. Enter the customer data in the form provided.
2. Click the "Predict" button.
3. The application will display the prediction result and the probability of churn.

## Example

1. Start the Streamlit application:
    ```sh
    streamlit run streamlit_churn_app.py
    ```

2. Open your web browser and go to the URL provided by Streamlit.

3. Enter sample customer data:
    - Age: 35
    - Gender: Male
    - Support Calls: 5 times
    - Payment Delay: 10 days
    - Total Spend: 1000$
    - Last Interaction: 6 days
    - Tenure: 90 days
    - Usage Frequency: 4 times/week
    - Subscription Type: Premium
    - Contract Length: Annual

4. Click the "Predict" button.

5. The application will display:
    - Prediction: The customer is likely to churn.
    - Probability: 0.85 (85% chance of churn).

## License

This project is licensed under the MIT License. See the LICENSE file for details.
