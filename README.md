# Neural-Network-ML-on-Uncle-fundamental-stock-datafeed
Neural Network ML to predict portfolio performance based on Uncle fundamental stock datafeed.

The objective is to let the neural network predict the future stock return.

Read a dataset with fundamentals on stocks: one row is one stock at a given moment in time.

The data looks like this:

![image](https://user-images.githubusercontent.com/78446548/109012385-3f1c2f00-76b2-11eb-8b00-a494ca2825c7.png)

The neural network is 12 * 30 * 1 fully connected deep NN consisting of an input layer (12 nodes), a hidden layer (30 nodes) and an output layer (one node with the future stock return).

The network structure (Tensorflow Dashboard / Tensorboard):

![image](https://user-images.githubusercontent.com/78446548/109649651-809e5580-7b5c-11eb-9169-e7123a4005e1.png)

Fully unfolded network architecture:

![image](https://user-images.githubusercontent.com/78446548/111709943-e5d69400-8848-11eb-9c9e-695f925c9d06.png)

GPU = Intel UHD Graphics 620, CPU = Intel Core i7 - 8565 U @ 1.8 Ghz

Tensorflow services are (automatically) spawned to execute the kernel implementations appropriate to the available hardware (either GPU or CPU)

The convergence of the losses on training and validation dataset (blue = loss, red = val_loss):

![image](https://user-images.githubusercontent.com/78446548/109648782-513b1900-7b5b-11eb-8b24-322bb3fd5226.png)

After 50 epochs, STOP criterium = fixed 50, hyperparameters not optimised

Activation functione relu

Tech stack Tensorflow with keras

Further details see notebook



Finally the resulting relations between stock price predictions and real historical stock returns for the test set. The black line is the 'perfect prediction' (predicted stock return = real stock return):

![image](https://user-images.githubusercontent.com/78446548/109011090-d97b7300-76b0-11eb-8946-71c6629ff51b.png)

The average real return of the TEST data series = 18.7 %

On the predicted best 30 stocks of the portfolio (out of 70 in TEST set) the average return = 35,9 %


