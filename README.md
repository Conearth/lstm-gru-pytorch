## 注意
## 此文档没有实现stack_lstm/gru， 可以直接用torch.nn.GRU或torch.nn.LSTM替代底层cell。
## 此文档的主要价值是实现循环的状态转移，在model类中进行了实现



This repository is an implementation of the LSTM  and GRU cells without using the PyTorch LSTMCell and GRUCell.  

It is tested on the MNIST dataset for classification. 

The 28x28 MNIST images are treated as sequences of 28x1 vector.

The RNN consist of 

- A linear layer that maps 28-dimensional input to and 128-dimensional hidden layer
- One intermediate recurrent neural network (LSTM or GRU)
- A fully connected layer which maps the 128 dimensional input to 10-dimensional vector of class labels.



## Requirements 

Python>=3.5

PyTorch== 0.4.0



