# XGBoost Energy Prediction

This project uses XGBoost to predict energy consumption based on time series and building metadata. The notebook includes data preprocessing, model training, evaluation, and visualization of predictions compared to actual values.

## Features

- Data preprocessing for building-specific datasets.
- Training and evaluation of XGBoost models.
- Visualization of actual vs. predicted energy consumption.

---

## How to Clone

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/your-username/xgboost-energy-prediction.git
   cd xgboost-energy-prediction

## Setting Up Google Drive Path

This project relies on datasets hosted in a shared Google Drive folder. Follow these steps to set up proper paths:

1. Access the shared Google Drive folder using [this link](https://drive.google.com/drive/folders/1JxD35ISdCnzNeE-yBvaaCNmbocbWmSW0?usp=sharing).
2. Create a **Google Drive shortcut** to the folder in your personal Google Drive.
3. Update the path in the notebook:
   - Locate the `# Load the datasets` section in the notebook.
   - Update the ```PROCESSED``` to point to the shortcut folder in your Google Drive:
     ```python
     # PROCESSED = f'/content/drive/MyDrive/YOUR_GOOGLE_SHORTCUT'
     ```

## Usage Instructions

1. Open the Jupyter Notebook in your environment. (Preferably Google Colab)
2. Update the paths for datasets under the `# Load the datasets` section.
3. Run the notebook to:
   - Train the model.
   - Evaluate its performance.
   - Visualize the results using time series plots.

---

## Key Sections

### Data Preprocessing

- Cleans and aligns building datasets.
- Ensures the input data matches the model’s expected format.

### Model Training

- Trains an XGBoost model with hyperparameter tuning and early stopping.
- Outputs feature importance metrics for better interpretability.

### Model Evaluation

- Uses the trained model to predict energy consumption for unseen data.
- Calculates evaluation metrics like SMAPE (Symmetric Mean Absolute Percentage Error).

### Visualization

- Creates interactive time series plots to compare actual vs. predicted energy consumption.
- Highlights areas where the model's predictions deviate from reality.
