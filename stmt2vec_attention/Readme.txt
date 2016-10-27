Stmt2vec

Training code from the paper "Stmt2vec: Learning Representations of Source Code".

Dependencies
Python 2.7 Latest version of NumPy and SciPy Theano 0.9

Instructions

To train the stmt2vec model at the task of extreme summarization:
         > python stmt2vec_learner.py <project_path>


Configuration

The parameters of this model have been already embedded in our source code. Key parameters include the dimension of the token embeddings, the dimensions of the hidden layers of GRU, and the window size of the convolutional layer. Other parameters are also important, like the learning rate, the dropout rate, the init_scale, etc.

We experimented different configurations of these parameters, e.g., the dimension of the token embeddings ranging from 64 to 256; the dimension of the first GRU hidden layer ranging from 16 to 64; the layer3_window_size ranging from 7 to 17; the dropout_rate ranging from 0.3 - 0.7, etc.

Moreover, we have done systematic experiments on different structures of the stmt2vec network and the usage of data/control dependencies.
