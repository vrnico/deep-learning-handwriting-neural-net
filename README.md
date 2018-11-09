# using neural nets to recognize handwritten digits

### a neural net built in python using the MNIST handwriting database.

###### based off educational content in the tutorial linked below by Michael Nielsen
[Neural Networks and Deep Learning](http://neuralnetworksanddeeplearning.com/chap1.html)

## SETUP:
(this setup assumes installation of Python 3.7 and numpy)

- in Python command line navigate to the repository
	>`>>>import os`

	>`>>>os.chdir(“C:\\your-file-path-goes-here\\neural-networks-and-deep-learning\\src”)`

- Import the MNIST database via the mnist_loader file
	>`>>>import mnist_loader`

	>`>>>training_data, validation_data, test_data = \`

	>`... mnist_loader.load_data_wrapper()`

- Set up the network using your own parameters or the parameters listed below (this is a network with 30 hidden neurons for example)

	>`>>>import network`

	>`>>> net = network.Network([784, 30, 10])`

	>`>>> net.SGD(training_data, 30, 10, 3.0, test_data=test_data)`

- Sit back and watch your neural net learn the nuance and subtlety of handwritten recognition! Toy with network parameters to see how dumb or smart your new computer friend can be! The sky is the limit!

	![gif of neural net](https://imgur.com/z8drJLK.gif)




## Note from Original Author Micheal Dobranski

This repository contains code samples for my book on ["Neural Networks
and Deep Learning"](http://neuralnetworksanddeeplearning.com).

The code is originally written for Python 2.6 or 2.7, but updated for Python 3.7 by Nico Daunt

 Michal Daniel Dobrzanski
has a repository for Python 3
[here](https://github.com/MichalDanielDobrzanski/DeepLearningPython35). I
will not be updating the current repository for Python 3
compatibility.

The program `src/network3.py` uses version 0.6 or 0.7 of the Theano
library.  It needs modification for compatibility with later versions
of the library.  I will not be making such modifications.

As the code is written to accompany the book, I don't intend to add
new features. However, bug reports are welcome, and you should feel
free to fork and modify the code.

## License

MIT License

Copyright (c) 2012-2018 Michael Nielsen

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
