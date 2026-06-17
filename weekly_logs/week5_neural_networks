# [Week 5 - Neural Networks](https://cs50.harvard.edu/ai/weeks/5/)

## Progress
- Completed lecture [2026-06-15]
- Completed project Traffic [2026-06-16]

## Key Concepts
- **Artificial Neural Network (ANN)**: A machine learning model inspired by biological neural networks. In practice, an ANN is made of layers of nodes connected by weighted edges. During training, the model adjusts weights and biases to learn the relationship between inputs and outputs.
    - **Nodes and Edges**: In the input layer, nodes represent input features. In hidden layers, nodes represent learned intermediate features. Edges represent weights that determine how strongly one node contributes to another.
    - **Activation Function**: A function applied to a node’s weighted input to introduce non-linearity. Without activation functions, even a multi-layer neural network would behave like a linear model.
    - **Deep Neural Network (DNN)**: A neural network with multiple hidden layers, allowing the model to learn increasingly abstract representations.
        - **Feed-Forward Neural Network**: A neural network where information flows in one direction from input to output. The input and output sizes are fixed.
        - **Recurrent Neural Network (RNN)**: A type of neural network designed for sequential data. RNNs maintain hidden state information across time steps, making them useful for tasks such as speech recognition, text generation, translation, and video captioning.
- **Convolution**: An operation that applies learnable filters/kernels across an image to detect local patterns. Earlier convolutional layers may learn low-level features such as edges and corners, while deeper layers can learn higher-level visual patterns.
- **Pooling**: A downsampling operation that reduces the spatial size of feature maps by summarizing local regions. Common strategies include max pooling and average pooling.
- **Flattening**: The process of converting multi-dimensional feature maps into a one-dimensional vector before passing them into dense layers.
- **Dense Layer**: A fully connected layer where each input is connected to each output neuron. In classification tasks, the final dense layer often has one output unit per class.
- **Dropout**: A regularization technique that randomly disables a percentage of nodes during each training iteration. This helps prevent overfitting by forcing the network to learn more robust features.

## What I've Learned
I'm really glad that I finally got to learn the practical application of TensorFlow and Keras. It was interesting to implement a deep neural network using TensorFlow instead of only learning the theory. For the Traffic project, I decided to look for literature that used the same GTSRB dataset and tried to implement a similar neural network structure. Through experimenting with convolutional layers, dropout, dense layers, and preprocessing, I managed to **achieve about 97% accuracy on the testing set.** It was a great beginner project because it helped me connect the theory of convolutional neural networks with an actual image classification task. One important lesson I learned was that model architecture is only one part of neural network performance. Preprocessing, input size, dropout rate, and the size of dense layers can significantly affect the result. At first, my model performed poorly, but after adjusting the architecture and preprocessing the images, the accuracy improved dramatically. This project made me want to find other datasets and papers, then try to implement and experiment with the models myself.

## Challenges
The main challenge for me in neural networks is the scale. When there are thousands of parameters to train, or many convolutional layers stacked together, it becomes difficult to mentally track what is happening inside the model. I understood the concepts of convolution and pooling before this lecture because I had taken a computer vision course during my master's degree, and this lecture aligned with some of the material from that course. However, I did not previously have much hands-on experience using TensorFlow, Keras, or neural network training workflows. This was my first time implementing and tuning a neural network in practice. Another challenge was understanding how layer shapes change throughout the network. For example, I had to trace how convolution and pooling changed the image dimensions, how feature maps were flattened, and how dense layers produced class scores. Reading the model summary helped me connect the architecture to the actual tensor shapes and parameter counts.

## Next Step
- Start Lecture 6 Language.
- Read the UC Berkeley CS188 textbook section on machine learning: [Machine Learning](https://inst.eecs.berkeley.edu/~cs188/textbook/ml/motivation.html).


## Experiment Notes
- Initial model used heavier dropout and a larger dense layer, but the accuracy was low.
- Reducing the dense layer from 512 to 128 units and adjusting dropout improved performance.
- Image preprocessing was important for stabilizing training.
- Final model achieved approximately 97% accuracy on the testing set.