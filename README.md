# Real-Time SMS Spam Detection using PySpark and LSTM

## Overview

This project simulates real-time SMS spam detection using PySpark Streaming for data processing and an LSTM deep learning model for classification. The dataset is processed in chunks to simulate streaming, and the model is trained to classify messages as spam or not spam.

## Technologies Used

- Python
- PySpark
- TensorFlow/Keras
- Scikit-learn
- NumPy
- Pandas

## Dataset

The dataset used is a CSV file containing SMS messages labeled as spam or ham. It is preprocessed and split into smaller chunks to mimic a streaming data environment.

## Steps Involved

### 1. Install Dependencies

```bash
pip install pyspark tensorflow scikit-learn numpy pandas
```

### 2. Read and Preprocess Dataset

- Load the dataset.
- Keep only relevant columns (label, message).
- Encode labels using `LabelEncoder`.

### 3. Simulate Streaming Data

- Split the dataset into chunks.
- Save each chunk into a directory with a time delay.

### 4. Setup PySpark Streaming

- Create a Spark session.
- Read streaming data from the directory.
- Perform real-time aggregations on incoming data.

### 5. Train LSTM Model

- Tokenize and pad text data.
- Split into training and test sets.
- Build an LSTM model.
- Train the model on the dataset.

### 6. Evaluate Model

- Calculate accuracy on the test dataset.
- Print model performance metrics.

### 7. Output Real-Time Aggregations

- Display the count of spam and non-spam messages in real time using Spark Streaming.

## Running the Project

1. Ensure all dependencies are installed.
2. Run the Python script.
3. Observe the streaming data processing and real-time spam classification.

## Model Performance

The trained LSTM model is evaluated on the test set and outputs the accuracy of classification.

## License

This project is open-source and available for use and modification.

