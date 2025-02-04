# Mobile Health Activity Detection

This repository contains a machine learning pipeline to detect user activity based on accelerometer and gyroscope data using multiple models and techniques.

## Project Overview

The goal of this project is to classify user activities from mobile health sensor data. Activities are predicted using various machine learning models, and the performance of each model is evaluated for accuracy, precision, recall, and other metrics.

## Dataset

The dataset used in this project is sourced from Kaggle: [Mobile Health Dataset](https://www.kaggle.com/datasets/gaurav2022/mobile-health).

## Setup

1. Clone the repository and install dependencies:

   ```bash
   git clone https://github.com/marksamfd/mhealth-classification.git
   cd mhealth-classification
   ```

2. Set up your Kaggle credentials to download the dataset:

   ```bash
   export KAGGLE_USERNAME=your_kaggle_username
   export KAGGLE_KEY=your_kaggle_key
   ```

3. Extract the dataset and ensure it is in the same directory as the script.

## Features and Data Preparation

- Data balancing ensures equal representation of all activities.
- Visualizations for sensor distributions are generated using Seaborn.
- One-hot encoding is applied for categorical features.

## Models Implemented

1. **Linear Regression**

   - Model evaluates with Mean Squared Error (MSE).

2. **Logistic Regression**

   - Simple classification model with accuracy and confusion matrix.

3. **K-Nearest Neighbors (KNN)**

   - Hyperparameters tuned with GridSearchCV.

4. **Support Vector Machine (SVM)**

   - Radial basis kernel with hyperparameter tuning.

5. **Neural Networks**
   - Built with TensorFlow and trained using sparse categorical cross-entropy.
   - TensorBoard used for logging and visualization.

## Evaluation

- Confusion matrices are generated for both train and test datasets.
- Metrics like accuracy, precision, and recall are calculated for comparison.

### Results Summary

- **Linear Regression**: Poor performance (MSE = 10).
- **Logistic Regression**: Moderate accuracy (54%).
- **KNN**: High accuracy (86%).
- **SVM**: High accuracy (85%).
- **Neural Networks**: Best performing model with training accuracy of 90%.

## How to Run

Run the code cells in sequence from the provided notebook or script. Ensure all dependencies are installed and the dataset is correctly placed.

## Visualizations

The project includes visualization of sensor data distribution and confusion matrices for detailed analysis.

## Future Work

- Enhance model performance with feature engineering.
- Implement additional deep learning architectures.
- Test models on real-time data streams.

## Contributing

Contributions are welcome! Please open issues or submit pull requests with improvements.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
