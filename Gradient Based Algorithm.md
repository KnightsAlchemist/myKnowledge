Gradient-based [[Algorithms]] are optimization techniques that iteratively adjust model parameters to minimize a loss function by following the gradient (or slope) of the loss with respect to the parameters.

Core types of gradient-based algorithms:

1. **[[Gradient Descent]] (GD)**: Updates parameters by moving in the direction of the negative gradient of the loss function. Variants include:
    
    - **[[Batch Gradient Descent]]**: Uses the entire dataset to compute the gradient.
    - **[[Stochastic Gradient Descent]] (SGD)**: Updates parameters using a single data point at a time, providing faster but noisier updates.
    - **[[Mini-batch Gradient Descent]]**: Balances between batch and stochastic by using small batches of data for each update.
2. **Variants of Gradient Descent**:
    
    - **Momentum**: Adds a fraction of the previous update to smooth out and speed up convergence.
    - **[[AdaGrad]]**: Adapts learning rates for each parameter based on their historical gradients, useful for sparse data.
    - **[[RMSProp]]**: Combines gradient history with exponential decay to maintain a more stable learning rate.
    - **Adam ([[Adaptive Moment Estimation]])**: Combines momentum and RMSProp to adaptively adjust learning rates, widely used for deep learning tasks.

These algorithms are central to training machine learning models, particularly neural networks, by optimizing their parameters efficiently.