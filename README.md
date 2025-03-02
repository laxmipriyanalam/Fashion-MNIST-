# Fashion-MNIST
The best perfroming model was determined based on its validation accuracy, with a final test accuracy of 86.05%.
The hyperparameters of this best performing model are:
1.The model was trained for 5 epochs, indicating that it learned effectively without overfitting.
2.The model consists of three fully connected layers, each with 32 neurons.This structure is relatively shallow.
3.Weight Decay (L2 Regularization): 0.0005
4.Learning Rate: 0.001 (A moderate learning rate that allows stable convergence )
5.Optimizer: Adam (Adaptive Moment Estimation).One of the best optimizers for deep learning.
6.A mini-batch size of 32 balances computation efficiency. Small batch sizes tend to generalize better.
7.Weight Initialization: Xavier (Ensures that weights start at optimal values.)
8.Activation Function: ReLU (Rectified Linear Unit).Efficient for deep neural networks.

Performance Metrics
Validation Accuracy: 87.22%
Test Accuracy: 86.05%

The dataset is divided into training and testing datasets. The 10% of large dataset is used for testing whereas the remaining data is used for training the model. A small portion of training dataset is also used for validation purpose.


Coding Style:
The code follows a modular and flexible design.
The create_model() function allows users to easily configure hidden layers, activation functions, optimizers, weight decay, and learning rate.
This design ensures the model can be reused and modified easily for different experiments.
The model supports multiple optimizers (SGD, Adam, RMSprop, etc.) and different weight initializations.
It allows custom batch sizes and different numbers of hidden layers, making it adaptable for various experiments.
The model is trained and tested using different possible combinations of hyperparameters.
