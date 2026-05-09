Weather Prediction: ML vs. Deep Learning
An end-to-end comparative study on forecasting daily mean temperatures in Basel using a comprehensive European weather dataset. This project evaluates the performance of traditional Gradient Boosting Machines (ML) against Long Short-Term Memory (LSTM) networks (DL) for time-series regression.

🚀 Overview
The goal of this project is to predict the next day’s mean temperature for Basel, Switzerland. The model leverages historical weather data including humidity, global radiation, pressure, and cloud cover from multiple European cities to identify complex meteorological patterns.

🛠️ Key Features
Temporal Feature Engineering: Implemented lag features (1-3 days), rolling averages, and cyclical month encodings (Sine/Cosine) to capture seasonal trends.

Gradient Boosting (ML): Utilized GradientBoostingRegressor to capture non-linear relationships and determine feature importance.

LSTM Networks (DL): Built a gated recurrent neural network specifically designed for sequential data and long-term dependencies.

Model Interpretability: Included correlation heatmaps and feature importance plots to explain model decision-making.

📊 Performance Comparison
Both models achieve high precision (R 
2
 >0.90), with the Gradient Boosting model slightly outperforming the LSTM in absolute error metrics for this specific dataset.

Metric	Gradient Boosting (ML)	LSTM (DL)
MAE	1.53°C	1.69°C
R² Score	0.930	0.914

Export to Sheets

Visual Analysis
📂 Project Structure
Plaintext

├── data/
│   └── weather_prediction_dataset.csv  # Input meteorological data
├── notebooks/
│   └── weather_analysis.ipynb          # Step-by-step implementation
├── plots/
│   ├── correlation_heatmap.png         # Feature relationship analysis
│   ├── ml_feature_importance.png       # Top drivers for ML model
│   └── time_series_forecast.png        # Comparison of predictions
├── README.md                           # Project documentation
└── requirements.txt                    # Dependencies
💻 Installation & Usage
Clone the repository:

Bash

git clone https://github.com/yourusername/weather-prediction.git
Install dependencies:

Bash

pip install -r requirements.txt
Run the analysis:
Execute the cells in the provided Jupyter Notebook or run the Python script to generate predictions and plots.

🧪 Technologies Used
Python (Pandas, NumPy)

Scikit-Learn (Gradient Boosting, Scaling, Metrics)

TensorFlow/Keras (LSTM Architecture)

Matplotlib & Seaborn (Data Visualization)
