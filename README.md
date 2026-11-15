# CNN Image Classification and Streamlit Application

Minor project for Unlox Academy. It has two parts:

- **Part A:** A Convolutional Neural Network that classifies handwritten digits (MNIST).
- **Part B:** A Streamlit web app, a Health & Fitness Calculator (BMI and daily calories).

## Results (Part A)
| Metric | Value |
|---|---|
| Test accuracy | 99.17% |
| Validation accuracy | 99.05% |
| Training accuracy | 99.42% |
| Misclassified test images | 83 / 10,000 |

## Model
Two Conv2D + MaxPooling blocks, Dropout (0.3), Dense(128) and a Dense(10) softmax layer.
225,034 trainable parameters, trained for 10 epochs with the Adam optimizer.

## Streamlit app
Takes name, age, gender, height, weight and activity level. It returns BMI, BMI category,
daily calorie estimate (Mifflin-St Jeor) and a health tip. Unrealistic inputs show an error.


## Dataset
[MNIST in CSV (Kaggle)](https://www.kaggle.com/datasets/oddrationale/mnist-in-csv):
60,000 training and 10,000 test images, 28x28 grayscale, 10 classes (0-9).
The data is not included in this repository.

## How to run
```bash
pip install -r requirements.txt
python YourName_CNN_Streamlit_Project.py      # trains and evaluates the CNN
streamlit run YourName_CNN_Streamlit_Project.py   # launches the app
```
The notebook can also be run on Kaggle or Google Colab.

## Report
See `report/Minor project report(Minor project 7)`.

## Author
Udeep Karmakar
