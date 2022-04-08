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

#<h2 id="convolution"> Convolution </h2>
In the process of Convolution, a Kernel (a matrix) which is used to extract the features from the images, moves over the input image and performs dot product with the sub-region of that image. The output of Convolution is a matrix of this dot product.
The kernel is moved across the image from left to right, top to bottom according to the number of steps given by the Stride value.
The dimensions of the image after undergoing Convolution is given by<br/>
O=([I-K]/S)+1<br/>
`O` stands for Output image dimension<br/>
`I` stands for Input image dimension<br/>
`K` stands for Kernel size<br/>
`S` stands for Stride<br/>

#<h2 id="padding"> Padding  </h2>
Padding is the approach where an extra layer of pixels are added around the image copying the pixels from the edge of the image in order to make the process of convolution efficient at the edge pixels.
It is used to resolve the Border Effect that is caused when the edge pixels are not processed completely during convolution.
The dimensions of the image after undergoing Padding is given by<br/>
O=([I-K+2P]/S)+1<br/>
`O` stands for Output image dimension<br/>
`I` stands for Input image dimension<br/>
`K` stands for Kernel size<br/>
`P` stands for Padding size<br/>
`S` stands for Stride<br/>

#<h2 id="pooling"> Pooling  </h2>
Pooling is used to scale down the dimensions of the image by retaining the important features in the feature map. The features are scaled down by summarizing the presence of features in patches of the feature maps. These patches are generally known as `Pool Window`. 
The common Pooling methods are<br/>
* **Max Pooling**<br/>Used to summarize the most activated presence of a feature in the pooling window 
* **Min Pooling**<br/>Used to summarize the least activated presence of a feature in the pooling window 
* **Average Pooling**<br/>Used to summarize the average presence of a feature in the pooling window 

#<h2 id="flatten"> Flatten  </h2>
Once the pooled feature map is obtained the next step is to flatten this feature map into a single column before feeding it to the neural network. This step makes the computation of the neural network much efficient and less expensive.<br/><br/>
### The diagram below shows the processes that an image undergoes before it is fed to a neural network

![1inc9c00m35q12lidqde](https://user-images.githubusercontent.com/84195790/161396010-e9877daa-1ac1-4cb6-ab9d-c54d8c021aa9.png)
