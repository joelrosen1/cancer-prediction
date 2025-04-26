# Cancer Prediction using MLP and CNN

This project implements two machine learning approaches for cancer prediction:
1. A Multi-Layer Perceptron (MLP) for lung cancer risk prediction
2. A Convolutional Neural Network (CNN) for skin cancer type classification

## Project Structure

```
.
├── MLP/                    # Lung Cancer Prediction
│   ├── Cancer_application.R    # Shiny application for visualization
│   ├── Lung_Cancer_Dataset.csv # Dataset with 5,000 records
│   ├── NN_Lung_Cancer.Rmd      # MLP implementation
│   └── NN_Lung_Cancer_NotPrebuilt.Rmd
└── CNN/                    # Skin Cancer Classification
    ├── CNN.ipynb           # CNN implementation
    └── accuracy_plot.png   # Model performance visualization
```

## MLP for Lung Cancer Prediction

The MLP model predicts lung cancer likelihood based on 18 risk factors from a dataset of 5,000 records. The model features:
- 5 hidden layers
- Input features related to lung cancer risk factors
- Interactive visualization through a Shiny application

### Running the MLP Application

1. Open `MLP/Cancer_application.R` in R Studio
2. Click the "Run App" button (green arrow) in the top right corner
3. The application will launch on localhost (typically takes ~5 minutes to load)

## CNN for Skin Cancer Classification

The CNN model classifies skin cancer types using the HAM10000 dataset. The implementation includes:
- Convolutional neural network architecture
- Performance visualization
- Jupyter notebook with detailed implementation

### Running the CNN Model

1. Open `CNN/CNN.ipynb` in Jupyter Notebook
2. Run the cells sequentially to train and evaluate the model

## Requirements

### MLP Requirements
- R Studio
- Required R packages:
  - shiny
  - neuralnet
  - ggplot2
  - dplyr

### CNN Requirements
- Python 3.x
- Jupyter Notebook
- Required Python packages:
  - tensorflow
  - keras
  - numpy
  - pandas
  - matplotlib

## Dataset Information

### Lung Cancer Dataset
- 5,000 records
- 18 features related to lung cancer risk factors
- Binary classification task (cancer likelihood)

### Skin Cancer Dataset (HAM10000)
- 10,000 dermatoscopic images
- 7 different types of skin cancer
- Multiclass classification task
