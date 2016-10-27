Stmt2vec

Training code from the paper "Stmt2vec: Learning Representations of Source Code".

Dependencies

This code is written in python. To use it you will need:
Python 2.7
Recent version of NumPy and SciPy
Theano 0.9

Usage Instructions

To train the Stmt2vec model at the task of extreme summarization:

> python stmt2vec_learner.py <project_path>

Parameter Settings

The parameters of this model has been defined in our source code already.
The most important parameters include the dimension of the token embedding, the dimensions of the hidden layers of GRU, and the window size of the convolutional layer. Other parameters are also important, like the learning rate, the dropout rate, the init_scale, etc. 

we experimented on these parameters, for example, the dimension of the token embedding ranging from 64 to 256,the first GRU hidden layer ranging from 16 to 64, the layer3_window_size ranging from 7 to 17 and the dropout_rate ranging from 0.3 - 0.7.

Our final

Moreover, we have done a lot experiments on the structure of the Stmt2vec and the usage of data and control dependencies.


When using the code in your research work, you should cite the following paper:

Stmt2vec: Learning Representations of Source Code. Shi Han, Haoyu Dong, Xin Li and Dongmei Zhang. 2016.
