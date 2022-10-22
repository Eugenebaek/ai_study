# Natural Language Processing Advancements By Deep Learning: A Survey - Summary
> "Generally AI is anything a computer can do that formerly was considered a job for a human"


## Background

### Definitions
- Deep Learning: Applying massive amounts of data to deep neural networks for it to learn how to handle a task.
- Feed-Forward Neural Network: A neural network in which the connections between nodes do not create any cycle, i.e., information flows in one direction.

### Deep Learning Architectures
1. Multi Layer Perceptron (MLP)

	A MLP has at least 3 layers: input, hidden, output. A layer is a collection of neurons which are nodes that transform information. Each neuron in a layer connects to all neurons in the next layer. However, neurons within each layer **do not** communicate with each other. MLPs are a class of FNNs.
![Multilayer Perceptron](./assets/mlp.png)

2. Convolutional Neural Network (CNN)
	A CNN is a class of FNNs inspired by the human visual cortex. CNNs are used in situations where data is represented as 2D or 3D data maps. CNNs take in an image represented as an array of values and use convolution to preform feature extraction by determining the relationship of a pixel to neighboring pixels. Convolutional layers have 3 dimension (width, height, depth) and are most commonly used in computer vision.

3. Recurrent Neural Networks (RNN)
	
