# Energy Consumption Prediction for Smart Buildings

## Project Overview

This project focuses on predicting energy consumption in smart buildings using machine learning techniques. It provides a Streamlit web application that allows users to input various environmental parameters and receive predictions for energy consumption. Additionally, the application offers data visualization and key performance indicator (KPI) insights based on historical energy consumption data.

## Features

*   **Energy Consumption Prediction**: Predicts energy consumption based on input parameters such as heat, relative humidity, air temperature, wind speed, weekend status, and pressure.
*   **Interactive Data Visualization**: Provides interactive plots to visualize daily energy consumption trends, distribution of energy consumption, and relationships between environmental factors (temperature, humidity, heat) and energy consumption.
*   **Key Performance Indicators (KPIs)**: Displays important metrics like average energy consumption, average temperature, and average humidity.
*   **User Authentication**: Includes a simple login system for accessing the application features.
*   **Data Exploration**: Allows users to view the raw dataset used for analysis.

## Technologies Used

The project is built using the following technologies:

*   **Python**: The core programming language.
*   **Streamlit**: For creating the interactive web application.
*   **Pandas**: For data manipulation and analysis.
*   **NumPy**: For numerical operations.
*   **Scikit-learn**: For machine learning model (scaler and predictor).
*   **XGBoost**: Likely used for the energy prediction model.
*   **Plotly Express**: For interactive data visualizations.
*   **Matplotlib & Seaborn**: For additional plotting capabilities.
*   **Pickle**: For serializing and deserializing Python objects (model and scaler).

## Installation

To set up and run this project locally, follow these steps:

1.  **Clone the repository**:

    ```bash
    git clone https://github.com/your-username/Energy-Consumption-Prediction-for-Smart-Buildings.git
    cd Energy-Consumption-Prediction-for-Smart-Buildings
    ```

    *(Note: Replace `https://github.com/your-username/Energy-Consumption-Prediction-for-Smart-Buildings.git` with the actual repository URL if available.)*

2.  **Create a virtual environment** (recommended):

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the required dependencies**:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  **Run the Streamlit application**:

    ```bash
    streamlit run app.py
    ```

2.  **Access the application**: Open your web browser and navigate to the URL provided by Streamlit (usually `http://localhost:8501`).

3.  **Login**: Use the sample credentials provided in `app.py` (e.g., `username: admin`, `password: password123`) to log in.

4.  **Navigate through sections**: Use the sidebar to switch between "Energy Consumption Prediction", "Visualize Data", "Data", and "Key Performance Indicators" sections.

## Project Structure

```
Energy-Consumption-Prediction-for-Smart-Buildings/
├── Dataset/
│   ├── Final_dataset.csv
│   └── Malmi_office_building_hourly.csv
├── Model/
│   ├── energy_predict.pkl
│   └── scaler.pkl
├── Notebook/
│   └── Malmi_office_energy_prediction.ipynb
├── Video/
│   └── Final.mp4
├── .devcontainer/
│   └── devcontainer.json
├── Energy Consumption Prediction PPT.pptx
├── README.md
├── app.py
├── requirements.txt
└── users.json
```

*   `Dataset/`: Contains the raw and processed datasets used for training and analysis.
*   `Model/`: Stores the trained machine learning model (`energy_predict.pkl`) and the data scaler (`scaler.pkl`).
*   `Notebook/`: Jupyter notebooks for data exploration, model training, and analysis.
*   `Video/`: Contains a video presentation of the project.
*   `.devcontainer/`: Configuration files for development containers.
*   `Energy Consumption Prediction PPT.pptx`: A PowerPoint presentation related to the project.
*   `README.md`: This file.
*   `app.py`: The main Streamlit application script.
*   `requirements.txt`: Lists all Python dependencies required for the project.
*   `users.json`: (Potentially) stores user credentials, though `app.py` currently uses hardcoded values.

## Data Source

The primary dataset used in this project is sourced from the AI4EU platform. It contains hourly electricity and heating consumption data from an office building in Malmi, Helsinki, Finland, along with weather-related variables from the Helsinki Malmi lentokenttä meteorological station.

*   **Dataset Link**: [AI4EU Platform - Electricity Consumption Dataset](https://www.ai4europe.eu/research/ai-catalog/electricity-consumption-and-weather-indicators-datasets)

## Model

The project utilizes a pre-trained machine learning model (likely an XGBoost regressor, given `xgboost` in `requirements.txt`) to predict energy consumption. A `StandardScaler` is also used to preprocess input features before feeding them to the model.

## Authentication

The `app.py` includes a basic authentication system. The current hardcoded credentials are:

*   **Username**: `admin`
*   **Password**: `password123`
*   **Username**: `user1`
*   **Password**: `userpass`

For a production environment, it is highly recommended to implement a more secure authentication mechanism and store user credentials securely (e.g., in a database with hashed passwords).

## Contributing

Contributions are welcome! Please feel free to fork the repository, create a new branch, and submit a pull request for any improvements or bug fixes.

## License

This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT). (Assuming MIT License, please update if different.)

## Contact

For any questions or inquiries, please contact [Saipraneeth S/saipraneethsattu@gmail.com].
