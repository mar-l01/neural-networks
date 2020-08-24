# A brief introduction to neural networks
This guide will give interested people a quick introduction into the basics of neural networks. Neural networks evolve over time. Given enough samples of input data, they are able to learn an internal representation of that data, that allows them to predict the desired output.

## Yet another neural network introduction
With so many descriptions about neural networks around, this one is not different at all. As I wrote my Master's thesis about deep learning, I read a lot about neural networks. The analysis of different types of neural networks, their field of application and their pros and cons gave me a deep insight into the nature of neural networks. Not to say, I am an expert on this field, but I dare say I can give a good introduction to newcomers.

## Applications of neural networks
Neural networks can be applied to different areas. For once there is image process or computer vision. So-called convolutional neural networks can be trained on millions of images to get as close as possible to predict the right output. For instance, training them on input images of [fashion-articles](https://www.kaggle.com/zalando-research/fashionmnist) (shoes, shirts, ties, ...) they are able to recognize previously unseen images correctly. Another way to apply neural networks is data-analysis. One can for instance train a neural network to detect a computer virus. Recurrent neural networks can be used, on the other hand, to predict time-series. These are mostly applied in language processing. Given several letters, they are able to predict the next one and the next and so on.

## Different types of learning
Depending on the application, neural networks are trained in different ways:
- __Supervised learning__: Training is done with a pairs of input/label data, meaning each input to a neural networks has a label, which the neural network should learn to predict. For example, if the input data is an image of a car, the label would be 'Car'.
- __Unsupervised learning__: In contrast to supervised learning, this learning type simply relies on the input data. It tries to figure out dependencies in the input data-set to predict an output.
- __Semi-supervised learning__: As the name implies, this learning type is a mix of both learning types described above.
- __Reinforcement learning__: An agent learns to  move in an unknown environment by receiving rewards for each action. The higher the reward, the better his action is/was. This way, the agent learns the best way to move by maximizing its reward.

## Neural networks
Though the name might imply it, neural networks are not exact copies of their biological counterparts. A neural networks is built-up by multiple neurons. They are connected layer-wise, i.e. neurons of one layer are connected to each neuron in the adjacent layer. There are variatons of neural networks where not all neurons of one layer are connected to each one in the adjacent layer to improve learning or predictions. An example of a so-called fully-connected feedforward neural network is given below:

![Feedforward Neural Network](/figures/neural_network.png)  
*Figure 1: A fully-connected feedforward neural network*

Other variations of such networks will be explained later. They range from those with loops to those that are not fully connected. But not matter which type of neural networks is chosen, there is one thing that is the same for all. They are all built-up by so-called neurons.

## Neurons - the basic unit of neural networks
Neurons are the computing unit of neural networks, they transfer information from one to another. Based on the biological system, one can also say that they fire in different strengths. The amount of information these neurons pass on to adjacent neurons is mostly computed the following way: All inputs <img src="https://render.githubusercontent.com/render/math?math=x_{i}"> are weighted by <img src="https://render.githubusercontent.com/render/math?math=w_{i}">. A bias value _b_ is added. The result is then passed into an activation function _a_, which then results the output _y(x)_ that is passed on to the adjacent neurons. A mathematical represenation looks as following: <img src="https://render.githubusercontent.com/render/math?math=y(x) = a(\sum_{i} x_{i}w_{i} %2Bb)">  
Figure 2 shows a single neuron, its inputs, weights, bias and the output using its activation function.

![Neuron](/figures/neuron.png)  
*Figure 2: A single neuron*

There are several activation functions available which will be explained next.

## To be continued..

