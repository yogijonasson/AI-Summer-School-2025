
# Notes on Neural Networks and Machine Learning
## Timeline of Key Developments


| Event | Year |
|-------|------|
| 1st Paper about AI (Neural Network Theory) | 1943 |
| Invention of the term "AI" (Dartmouth College) | 1956 |
| 1st Chatbot (Elisa) | 1966 |
| 1st GPT (Generative Pre-trained Transformer) | 2018 |

## Neural Networks (NN)

### Components of a Neural Network

- **Database**
  - Training base
  - Validation base
  - Test base
  - Note: Test data must not be used during training, and bases should not be correlated, in order to avoid bias.

- **Neural Network Structure**
  - **Neuron Parameters**
    - N weights (importance to inputs)
    - 1 bias
    - 1 (non-linear) activation function

There is then an internal output (z) which is a linear combination: Sum of (xi * wi) + bi. <br>
And then we evaluate z on the activation function. This can or no activates the neuron.


- **Cost/Loss Function**
  - Quantifies the error of the model.
  - Goal: Minimize this function.

- **Metric**
  - Quantifies the quality of a model.

- **Learning Algorithm**
  - Iterative algorithm that minimizes error over iterations.
  - Example: Gradient descent algorithm.

### Types of Neural Networks

#### Convolutional Neural Networks (CNN)

- No pre-processing (end-to-end model).
- Takes raw data and extracts/selects descriptors.
- Fully connected but descriptors are selected automatically.
- Convolution ~ filter.
- Pooling: Reduces size, e.g., from 2x2 to 1x1.
- Flattening between convolutional and fully connected layers.
- Other layers: Batch normalization, DropOut Layer.

#### Recursive Neural Networks (RNN)

- Efficient for sequential/temporal data.
- Recursive neurons: Output is an input with hidden state.
- More parameters, jointly optimized.
- Issues: Slow convergence, little memory, instability.

#### Long Short-Term Memory (LSTM)

- Augmented version of RNN.
- Gates: Forget, Input, Output.
- Processes time sequences more efficiently.
- Captures long-term dependencies.
- Issues: High computational cost, needs lots of training data.

## Key Concepts

### Overfitting and Underfitting

- **Underfitting**: Poor performance on both train and test data.
- **Overfitting**: Good performance on train data, poor on test data.
- **Bias/Variance Trade-Off**: Balance between bias and variance for optimal model performance.

### Regularization

- Method to deal with overfitting.
- Increases bias to decrease variance.

### Tokenization and Vectorization

- **Tokenization**: Dividing sentences into tokens.
- **Vectorization**: Associating tokens with IDs.
- **One-hot encoding**: Each ID is a vector with 1 at the IDth element.

### Embedding

- Words projected into a D-dimensional space.
- Preserves distances and semantic links.

## Machine Learning

### Database Split

- Training, Validation, Test.

### Types of Learning

- Supervised, Unsupervised, Semi-supervised, Self-supervised, Transfer Learning.

### ML Problems

- Classification, Regression, Clustering.

### Evaluation Metrics

- **Binary Classification**: Accuracy, Precision, Recall, F1-score.
- **Multi-class Classification**: Confusion matrix, One VS All strategy.
- **Regression**: Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Mean Absolute Error (MAE).

### Models

- **K-means Clustering**: Unsupervised learning for clustering.
- **KNN**: K Nearest Neighbors for classification.
- **Decision Tree**: Classification and regression with "if/else" nodes.
- **Logistic Regression**: Single neuron with sigmoid activation function.
