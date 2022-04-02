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
Convolutional Neural networks is a branch in Deep-learning that is found to be very effective in the field of media processing such as image recognition and audio/video recognition.
The dimentionality of the image is reduced before it is fed to a full-connected neural networks, in such a way that all the important features in an image is retained.
The important processes in a Convolutional Neural Network in image processing are as follows
1. [Convolution](#convolution)  
2. [Padding](#padding)
3. [Pooling](#pooling) 
4. [Flatten](#flatten)

## Convolution {#convolution#}
In the process of Convolution, a Kernel (a matrix) which is used to extract the features from the images, moves over the input image and performs dot product with the sub-region of that image. The output of Convolution is a matrix of this dot product.
The dimensions of the image after undergoing Convolution is given by<br/>
O=([I-K]/S)+1
`O` stands for Output image dimension
`I` stands for Input image dimension
`K` stands for Kernel size
`S` stands for Stride

<h2 id="padding"> Padding  </h2>


<h2 id="pooling"> Pooling  </h2>


<h2 id="flatten"> Flatten  </h2>


![1inc9c00m35q12lidqde](https://user-images.githubusercontent.com/84195790/161396010-e9877daa-1ac1-4cb6-ab9d-c54d8c021aa9.png)
