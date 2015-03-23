# NNet 0.1
This is a simple implementation of neural networks in Python. Use at your own risk, as  this is very messy and created in an ad-hoc manner to suit my needs.

<h1>Example</h1>
The model expects NxP numpy arrays as input (X) where N is the number of observations and P is the number of features. The target values (Y) can either be a numpy array where each column is a class for classification or a number for regression.
```
from NNet import NeuralNet

nnet = NeuralNet(100, learn_rate=1e-2, penalty=1e-8)
nnet.fit(X_train, Y_train, SGD=True, batch=100)
nnet.score(X_test, Y_test)
```

More information on the methods can be found in the Wiki.
