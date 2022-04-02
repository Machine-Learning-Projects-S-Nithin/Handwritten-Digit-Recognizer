# Handwritten-digit-recognizer
Different machine learning models were built and compared to recognize the handwritten digits.

## Input format fed to the models
### Training data
The `train.csv` file contains training data, which consists of 42000 images of dimensions 28 pixels x 28 pixels each. Each value in the training data represents the brightness of the particular pixel, and this value varies from 0 to 255, 255 being the brightest pixel value. The first column in the training data represents the target variable whereas the other columns represent the feature variables.
### Testing data
The `test.csv` file contains testing data, which consists of 28000 images of dimensions 28 pixels x 28 pixels each.  Each value in the training data represents the brightness of the particular pixel, and this value varies from 0 to 255, 255 being the brightest pixel value.



## Models built and their respective accuracy scores:
| Model| Accuracy Score |
|-------|---------------|
| Logistic Regression | 0.8 (80%) | 
| Random Forest Clasifier | 0.8 (80%) | 
| Decision Tree Classifier | 0.8 (80%) |
| Naive Bayes classifier | 0.8 (80%) |

From the information above we can see that a Convolutional Neural Networks model has the best performance in recognizing handwritten characters.

## Convolutional Neural Networks
