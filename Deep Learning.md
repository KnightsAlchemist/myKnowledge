Deep Learning (DL) is a subset of machine learning that focuses on algorithms inspired by the [[structure and function of the brain]], specifically neural networks. It excels in modeling complex patterns and representations, particularly in large datasets, and is a driving force behind many modern AI applications such as image recognition, [[natural language processing]], and autonomous systems.

### Core Concepts in Deep Learning:

1. **[[Neural Networks]]**:
    
    - **Artificial Neural Network (ANN)**: A network of layers composed of nodes (neurons), where each neuron applies a transformation to the input. Neural networks consist of:
        - **Input Layer**: Takes in the raw features or data.
        - **Hidden Layers**: Perform transformations on the data using weights and biases, applying activation functions to introduce non-linearity.
        - **Output Layer**: Produces the final prediction (classification or regression).
2. **[[Activation Functions]]**: Introduce non-linearity into neural networks, allowing them to model complex patterns.
    
    - **Sigmoid**: Compresses input values to a range between 0 and 1, often used in binary classification.
    - **ReLU (Rectified Linear Unit)**: Outputs the input if positive, otherwise zero. It is computationally efficient and commonly used in hidden layers.
    - **Tanh**: Similar to Sigmoid but compresses the output to the range of -1 to 1.
    - **Softmax**: Used in multi-class classification to output probabilities that sum to 1.
3. **[[Deep Networks]]**:
    
    - Networks with multiple hidden layers (often more than three) are referred to as deep neural networks. This depth allows them to model hierarchical data representations, such as detecting edges, shapes, and objects in images.

### Common Deep Learning Algorithms:

1. **[[Convolutional Neural Networks]] (CNNs)**:
    
    - Primarily used for image and video processing. CNNs use convolutional layers that apply filters to capture spatial hierarchies in images, extracting features like edges, textures, and objects.
    - Components include:
        - **Convolutional Layer**: Applies filters to the input data to capture spatial features.
        - **Pooling Layer**: Reduces the spatial dimensions ([[downsampling]]) to reduce computational complexity and focus on dominant features.
        - **Fully Connected Layer**: Maps learned features to the final output.
2. **[[Recurrent Neural Networks]] (RNNs)**:
    
    - Designed for sequential data, such as time series or natural language. RNNs retain memory of previous inputs, enabling them to model temporal dependencies.
    - Variants:
        - **Long Short-Term Memory (LSTM)**: An advanced RNN designed to handle long-term dependencies and mitigate the vanishing gradient problem. It uses gates to control the flow of information.
        - **Gated Recurrent Units (GRU)**: A simplified version of LSTMs with fewer gates, but still effective for handling long-term dependencies.
3. **[[Generative Adversarial Networks]] (GANs)**:
    
    - GANs consist of two networks: a [[generator]] and a [[discriminator]]. The generator creates synthetic data, while the discriminator evaluates its authenticity. The two networks compete in a zero-sum game, improving each other until the generator produces highly realistic data.
    - Applications include image generation, data augmentation, and deepfake creation.
4. **[[Autoencoders]]**:
    
    - [[Neural Networks]] designed for unsupervised learning tasks, specifically [[dimensionality reduction]] and data compression. An [[Autoencoders]] consists of an encoder (which compresses the input) and a decoder (which reconstructs the input from the compressed representation).
    - Variants:
        - **Denoising Autoencoders**: Learn to reconstruct clean data from noisy input.
        - **Variational Autoencoders (VAEs)**: Generate new data by learning a probabilistic representation of the input data.
5. **[[Transformers]]**:
    
    - Revolutionized [[natural language processing]] (NLP) by using self-attention mechanisms to process entire input sequences in parallel, improving on the sequential nature of RNNs. [[Transformers]] are foundational in models like BERT and GPT.
    - **Self-Attention**: Allows the model to focus on different parts of an input sequence when making predictions, enabling better handling of long-range dependencies.
    - **BERT (Bidirectional Encoder Representations from Transformers)**: A pre-trained transformer model that understands context by considering both the left and right sides of a word in a sentence.
    - **GPT (Generative Pre-trained Transformer)**: A transformer-based model optimized for generating text, fine-tuned for various NLP tasks.
6. **[[Reinforcement Learning]] in Deep Learning (Deep RL)**:
    
    - Combines deep learning with reinforcement learning techniques, where an [[agent]] learns by interacting with its environment and receiving rewards for actions. Deep Q-Networks (DQNs) use deep neural networks to approximate the action-value function in RL tasks.
    - Applied in robotics, gaming (e.g., AlphaGo), and autonomous systems.

### Key Terminology in Deep Learning:

1. **[[Epoch]]**: One complete pass of the entire dataset through the model during training.
    
2. **[[Batch Size]]**: The number of samples processed before updating the model's parameters.
    
3. **[[Learning Rate]]**: The step size used by optimization algorithms to adjust model parameters during training.
    
4. **[[Backpropagation]]**: The process of calculating gradients of the loss function with respect to each parameter in the network using the chain rule, allowing the model to update weights during training.
    
5. **[[Vanishing/Exploding Gradient Problem]]**: In very deep networks, gradients can become too small (vanish) or too large (explode), making it difficult to train. Techniques like LSTMs, ReLUs, and normalization mitigate these issues.
    
6. **[[Dropout]]**: A regularization technique that randomly drops neurons during training to prevent overfitting.
    
7. **[[Weight Initialization]]**: Proper initialization of network weights is critical to achieving fast convergence. Common strategies include Xavier or He initialization.
    
8. **[[Transfer Learning]]**: A technique where a pre-trained model (often on a large dataset) is fine-tuned on a new, smaller dataset, leveraging previously learned features.
    
9. **[[Loss Functions]]**:
    
    - **Cross-Entropy Loss**: Used in classification tasks, measuring the difference between predicted probabilities and actual labels.
    - **Mean Squared Error (MSE)**: Used in regression tasks to measure the average squared difference between predicted and actual values.
10. [[Optimization Algorithms]]:
    
    - **Stochastic Gradient Descent (SGD)**: An optimization algorithm that updates weights iteratively based on a small subset of data (mini-batch).
    - **Adam**: An adaptive optimization algorithm combining momentum and RMSProp, widely used for deep learning tasks due to its efficiency and performance.

### Deep Learning Applications:

1. **[[Computer Vision]]**: Image recognition, object detection, segmentation, and self-driving car technology.
2. **[[natural language processing]]**: Text classification, machine translation, chatbots, and sentiment analysis.
3. **[[Speech and Audio Processing]]**: Speech recognition, synthesis, and music generation.
4. **#Healthcare**: Predictive diagnosis, medical imaging analysis, and drug discovery.
5. **[[Autonomous Systems]]**: Robotics, drones, and autonomous vehicles.

Deep learning’s ability to model complex, non-linear relationships in data makes it a powerful tool for a wide range of applications, particularly when handling large-scale, high-dimensional data.