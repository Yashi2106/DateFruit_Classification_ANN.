# Date Fruit Classification using Artificial Neural Network

## What is this?

A neural network model that classifies date fruits into **7 different varieties** based on 34 morphological features extracted from fruit images.

## Dataset

- **Samples:** 898
- **Features:** 34 (shape, color, texture features)
- **Classes:** 7 types of dates
- **Source:** Date Fruit Dataset

### Target Classes

| Class | Name |
|-------|------|
| 0 | BERHI |
| 1 | DEGLET |
| 2 | DOKOL |
| 3 | IRAQI |
| 4 | ROTANA |
| 5 | SAFAVI |
| 6 | SOGAY |

## Feature Types

- Shape features (AREA, PERIMETER, MAJOR_AXIS, MINOR_AXIS, ECCENTRICITY)
- Color features (Mean, StdDev, Skew, Kurtosis for R,G,B channels)
- Texture features (Entropy, Wavelet features)

## Model Architecture

- **Hidden Layers:** 2 layers with 64 neurons each
- **Activation:** ReLU
- **Output:** Softmax (7 classes)
- **Loss Function:** CrossEntropyLoss
- **Optimizer:** Adam

## Results

| Metric | Value |
|--------|-------|
| Test Accuracy | **95.56%** |
| Training Epochs | 100 |
| Batch Size | 32 |

## Preprocessing Steps

1. Label Encoding for target classes
2. Train-Test Split (80-20)
3. StandardScaler for feature normalization

## Requirements

## How to Run

1. Install required libraries
2. Place `DateFruit_Dataset.csv` in the same directory
3. Run the Jupyter notebook

## Key Insights

- Simple ANN with 2 hidden layers performs well on morphological features
- Standardization is crucial for this dataset due to varying feature scales
- 95.56% accuracy shows strong separability of date fruit classes

## File Structure

## License

MIT
