# TextClassification-CNNs

Two convolutional neural network (CNN) architectures were developed and trained for the task of text classification. The architectures differ in terms of the number of convolutional layers, kernel sizes, and the presence of dropout layers.

## First Architecture
1. Embedding layer
2. Two convolutional layers (kernel 3,3) with max pooling after each to down-sample the features
3. One dense layer with ReLU activation
4. A final dense layer with a sigmoid activation function for binary classification.

**Compilation**:
- Optimizer: Adam
- Loss function: Binary cross-entropy

**Performance**:
- Accuracy on training data: 71.25%
- Accuracy on validation data: 68.96%

## Second Architecture
1. Embedding layer
2. Two convolutional layers (kernel 3,5) with max pooling after each to down-sample the features
3. Two dense layers and Dropout layers are introduced after the dense layers to prevent overfitting
4. A final dense layer for classification

**Compilation**:
- Optimizer: Adam
- Loss function: Binary cross-entropy

**Performance**:
- Accuracy on training data: 78.99%
- Accuracy on validation data: 75.39%

## Conclusion
The second model which is more complex gave a higher accuracy.
