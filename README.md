# Crop Recommendation System 🌾

This project uses a machine learning model to recommend the most suitable crop to cultivate based on soil and weather conditions.

## 📊 Dataset

The dataset contains the following features:

- `N` - Nitrogen content in soil
- `P` - Phosphorus content in soil
- `K` - Potassium content in soil
- `temperature` - Temperature in °C
- `humidity` - Relative humidity in %
- `ph` - pH value of the soil
- `rainfall` - Rainfall in mm
- `label` - Crop label (e.g., rice, maize, coconut, etc.)

## 🧠 Model Architecture

A deep neural network built with TensorFlow/Keras:

```python
model = Sequential()
model.add(Input(shape=(7,)))
model.add(Dense(200, activation="relu"))
model.add(Dense(400, activation="relu"))
model.add(Dense(200, activation="relu"))
model.add(Dense(22, activation='softmax'))
```
##🚀 Getting Started
1. Clone the Repository
   ```
   git clone https://github.com/yourusername/crop-recommendation.git
   cd crop-recommendation
   ```
2. Train the Model
Ensure you have a dataset in .csv or .xlsx format.
```
model.fit(x_train, y_train, validation_split=0.2, epochs=10)
```
