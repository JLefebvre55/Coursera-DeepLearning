# Learning

Learning is the process by which a neural network _adapts_ to minimize the cost of its fit.

## Loss Functions

$$\mathcal{L}(y,\hat y)\text{ where }y\text{ is the output and }\hat y \text{ is the "ground truth label".}$$

Define how poorly a given model fits. A good model has a loss function value *approaching zero*.

For **best** gradient descent, you want there to be `one minima` *at* the label value. See [Desmos](https://www.desmos.com/calculator/desmzbmxbh).

### Square Error

$\mathcal{L}(y,\hat y) = c(y - \hat y)^2$ where $c$ is a scalar.

### Logistic Regression

$\mathcal{L}(y,\hat y) = -(y\log(\hat y) + (1 - y)\log(1 - \hat y))$

Reasoning:

$y = 1\to \mathcal{L}(1,\hat y) = -\log(\hat y)$

$y = 0\to \mathcal{L}(0,\hat y) = -\log(1 - \hat y)$

## Loss Function Design

TODO: Consider convexity and optima

### Loss vs Cost

Loss is for one training datum and prediction. Cost is for the model itself, and is applied to the `parameters` (weights and biases) directly.

$$ C(w,b)=\frac 1m \sum_{i=0}^n \mathcal{L}(y ^i, \hat y^i)$$

## Propagation

Forward - compute the output

Backward - compute partial derivatives of cost relative to cost and perform gradient descent. This is done via the `chain rule` - how does the output vector change with respect to the final hidden layer's parameters, that layer to the previous, etc.

## Algorithms/Strategies

Gradient Descent: alteration of parameters `w` and `b` to minimize the cost function `C(w,b)` by changing each component of `w|b` according to the partial derivative of `C` with respect to the component.
## Supervised Learning

TODO.

## Deep Learning

Many, many hidden layers. Greater abstraction.