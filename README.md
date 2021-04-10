# Fashion Mnist solution

# Fashion Mnist solution


## About FashionMNIST

- Fashion-MNIST is a dataset of Zalando's article images—consisting of a training and a test set 
- Each example is a 28x28 grayscale image
- The above mentioned dataset and has only 4 classes.
- Each image is 28 pixels in height and 28 pixels in width, for a total of 784 pixels in total.
- Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel,
with higher numbers meaning darker. This pixel-value is an integer between 0 and 255.


Each training and test example is assigned to one of the following labels:

> T-shirt/top
> Trouser
> Pullover
> Dress

## Library used

List of libraries mainly used 

- Keras
- Numpy
- Matplotlib
- Seaborn 
- Pandas

## Dataset Exploration 

- Reading datasets using Pandas
- Exploration of data using different methods
- Cleaning dataset
- Visualizing the datasets and their distributions 

## Implementing in ML

Using some ML algorithms to validate with dataset

| ML | Accuracy |
| ------ | ------ |
| Support Vector Machine | 0.9395 |
| XGBoost | 0.9395 |
| k-Nearest Neighbor classifier  | 0.9395 |

## Implementing using Deep Learning

### Creating a 2 hidden layer neural network 
- Using activation function relu and sigmoid where relu in the hidden layer and and sigmoid in output layer
- accuracy is coming 0.9554 but we can improve it using Batchnormalization
- Cross validating multiple times to see the accuracies but relu in the hidden layer and and sigmoid in output layer gives best results 

#### Implementing by increasing no of layers
- By increasing no of layers and using relu in the hidden layer and and sigmoid in output layer gives the better accuracy
- Cross validating with different activation functions used in different layer but gives poor accuracy

#### Dropout 
- Used Dropout before every hidden layer
- It is improving the accuracy 


#### Batch Normalisation 
- Used Batchnormalisation before every Dense layer it is improving the accuacy
- Cross validate it multiple times but giving good accuracies

#### Model Checkpoint 
- Here Checkpoint is used by using the model of BatchNormalization  
- Saved the model in a directory and let it run until it finds the best model
- In case of Batchnormalisation accuracy is around 0.9664 but using checkpoing it it coming around 0.9922 
