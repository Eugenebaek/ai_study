# Natural Language Processing Advancements By Deep Learning: A Survey - Summary
> "Generally AI is anything a computer can do that formerly was considered a job for a human"


## II. Background

### A. Artificial Intelligence and Deep Learning

#### Definitions
- Deep Learning: Applying massive amounts of data to deep neural networks for it to learn how to handle a task.
- Feed-Forward Neural Network: A neural network in which the connections between nodes do not create any cycle, i.e., information flows in one direction.
- Bag-of-words (BoW): A method of representing textual data by word and frequency. BoW ignores the order and interaction of words, and treats each word as a unique feature. 

#### Deep Learning Architectures
1. Multi Layer Perceptron (MLP)

	A MLP has at least 3 layers: input, hidden, output. A layer is a collection of neurons which are nodes that transform information. Each neuron in a layer connects to all neurons in the next layer. However, neurons within each layer **do not** communicate with each other. MLPs are a class of FNNs.
![Multilayer Perceptron](./assets/mlp.png)

2. Convolutional Neural Network (CNN)

	A CNN is a class of FNNs inspired by the human visual cortex. CNNs are used in situations where data is represented as 2D or 3D data maps. CNNs take in an image represented as an array of values and use convolution to preform feature extraction by determining the relationship of a pixel to neighboring pixels. Convolutional layers have 3 dimension (width, height, depth) and are most commonly used in computer vision.

3. Recurrent Neural Networks (RNN)

	A RNN is a sequence of FNNs with each output fed to the input of the next FNN. Hidden layers in the RNN carry information from the past (memory) making it suited to handle a sequence of inputs common in language modeling. Long Short Term Memory Networks (LSTM) are the most common class of RNNs used to try to capture long time dependencies of inputs from different time steps.

	Ex. Consider the sentence: "Michael Jackson was a singer; some people consider him King of Pop." It's easy for a human to identify *him* as referring to Michael Jackson. The pronoun *him* happens seven words after *Michael Jackson*

4. Autoencoders

	Autoencoders consist of an encoder and a decoder. An encoder is similar to a FNN in that it encods an input into a vector. A decoder constructs an output based on the vector produced by the encoder. The goal of the autoencoder is to generate an approximate reconstruction of the output which is why it is used in unsupervised learning. 

5. Generative Adversarial Networks (GAN)

	A GAN consists of a discriminator neural network and a generator neural network. First the generator generates a fake sample. Then the discriminator tries to determine if the sample was generated or from the training data. This iterative process continues until the generator can produce samples that the discriminator cannot distinguish from the training data. In NLP, GANs are often used in text generation. 

### B. Motivations for Deep Learning in NLP

Currently, most NLP tasks rely on annotated data. Because of the abundance of unlabeled data, unsupervised feature learning is considered a crucial tasks in the progression of NLP.

## III. Core Concepts in NLP

### A. Feature Representation
1. One-Hot Representation
	
	Each unique element has its own dimension which leads to a high dimensional and sparse representation space. This structure allows for no connection between words.

	Ex. Highly correlated words such as 'ocean' and 'water' will not be closer to each other compared to less correlated pairs such as 'ocean' and 'fire'

2. Continuous Bag of Words (CBOW)

	Tries to predict a word given a few surrounding words as context. Like BoW, CBOW does not consider the order of words.

3. Word-Level Embedding

	Semantically correlated words become more probabalistic in the representation space.

4. Character-Level Embedding 
	
	Instead of a representation space of words, character embedding utilizes a vocabulary of characters to represent text. This type of embedding is useful when encountering out-of-vocabulary words (OOV) which are words that have no equivalent word in the representation space. 

### B. Seq2Seq Framework

	
