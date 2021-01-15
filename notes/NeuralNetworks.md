# Neural Networks

Chained mathematical functions, organized typically in layers.

## NN Structures

Densely connected: each element neuron of a layer is activated by combining all neurons of the previous layer, and activates all neurons of the subsequent layer.

Convolutional NN: Useful for image data.

Recurrent NN: Useful for one-dimensional/sequence data.

Support Vector Machine (SVM)

Logistic Regression

## Layers

- Input layer: `x`, no preceding layers;
- "Hidden" layers: All layers between input and output, arbitrary/no "real" meaning, purely mathematical;
- Output layer: `y`, no subsequenet layers;

## Activation Functions

- **ReLU** (**Re**ctified **L**inear **U**nits): `y = min(0, cx)` where `c` is a scalar;
- **Sigmoid**: `y = 1/(1 + e^-x)`, slow learning as `|x|>1`; gradient shrinks to zero (solved by ReLU)