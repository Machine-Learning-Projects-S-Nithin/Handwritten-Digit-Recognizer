# Handwritten-digit-recognizer
Different machine learning models were built and compared to recognize the handwritten digits.

## Input format fed to the models
### Training data
The `train.csv` file contains training data, which consists of 42000 images of dimensions 28 pixels x 28 pixels each. Each value in the training data represents the brightness of the particular pixel, and this value varies from 0 to 255, 255 being the brightest pixel value. The first column in the training data represents the target variable whereas the other columns represent the feature variables.
### Testing data
The `test.csv` file contains testing data, which consists of 28000 images of dimensions 28 pixels x 28 pixels each.  Each value in the training data represents the brightness of the particular pixel, and this value varies from 0 to 255, 255 being the brightest pixel value.

![Screenshot (445)](https://user-images.githubusercontent.com/84195790/161395248-1b8d9a76-e622-40e5-91e9-3569d1ffb768.png)

## Models built and their respective accuracy scores:
| Model| Accuracy Score |
|-------|---------------|
| Logistic Regression | 0.8 (80%) | 
| Random Forest Clasifier | 0.8 (80%) | 
| Decision Tree Classifier | 0.8 (80%) |
| Naive Bayes classifier | 0.8 (80%) |

From the table above we can see that a Convolutional Neural Networks model has the best performance in recognizing handwritten numbers.
Let us now understand the working of a convolutional neural network.

## Working of Convolutional Neural Networks
The important processes in a Convolutional Neural Network are as follows
1. [Convolution](#convolution)  
2. [Padding](#padding)
3. [Pooling](#pooling) 
4. [Flatten](#flatten)

<h2 id="convolution"> Convolution  </h2>


<h2 id="padding"> Padding  </h2>


<h2 id="pooling"> Pooling  </h2>

<h2 id="flatten"> Flatten  </h2>

