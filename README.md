# Neural-Network-ML-on-Uncle-fundamental-stock-datafeed
Neural Network ML to predict portfolio performance based on Uncle fundamental stock datafeed.

The objective is to let the neural network predict the future stock price.

Read a dataset with fundamentals on stocks: one row is one stock at a given moment in time
The data looks like this:
![image](https://user-images.githubusercontent.com/78446548/109012385-3f1c2f00-76b2-11eb-8b00-a494ca2825c7.png)

A neural network is defined consisting of an input layer, a hidden layer and an output layer.
The network structure (Tensorflow Dashboard / Tensorboard):

![image](https://user-images.githubusercontent.com/78446548/109649651-809e5580-7b5c-11eb-9169-e7123a4005e1.png)

The fully unfolded network architecture consists of an input layer, one hidden layer and one output node:

![image](https://user-images.githubusercontent.com/78446548/109649492-48971280-7b5c-11eb-9148-7b28bde05f55.png)



The convergence of the losses on training and validation dataset:

![image](https://user-images.githubusercontent.com/78446548/109648782-513b1900-7b5b-11eb-8b24-322bb3fd5226.png)

Finally the resulting realtions between stock price predictions and real historical stock prices for the test set:

![image](https://user-images.githubusercontent.com/78446548/109011090-d97b7300-76b0-11eb-8946-71c6629ff51b.png)
