# <strong>Neural Network from scratch </strong>


#### Table of contents
- How to Use
- Perceptron
- Multi - layer Perceptron
- Loss
- Backpropagation

## <strong> How to use </strong>


## <strong> Perceptron </strong>
How are we going to draw a line between circle and triangles?

![classification_problem](image/classification_problem.png)

<strong> Use Linear classifer or Perceptron! </strong>

Perceptron is a linear classifier(binary). It helps classify the given input data.

It gets input,transforms it and outputs result.

![perceptron](image/perceptron.png)

It gets input X, matrix multiply with W(weight), add bias, put in activation function and outputs result.

![perceptron_formula](image/perceptron_formula.png)

Perceptron can deal with linearly separable problems.
![linearly_separable](image/linearly_separable.png)

How about XOR problem? We need multi-layer Perceptron.

# Multi-layer Perceptron
It is a stack of perceptron, with hidden layer in between input layer and output layer.

![multilayer_perceptron](image/multilayer_perceptron.png)

2-layer Perceptron can deal with some nonlinear problems.
3-layer Perceptron can deal with more complex problems

## Loss : how to train multi-layer perceptron?
Loss(=cost) is a real number that represents how much wrong it is. We need to find how different true values are from calculated values. One way is to subtract calculated value from true value.

![loss_function](image/loss_function.png)

We can also use cross entropy, which is usually used in classification problem. q(x) is the output value and p(x) is true label where expressed in 0 and 1. Thus it adds all the output value of true labels.

![cross_entropy](image/cross_entropy.png)

# Backpropagation
We should minimize loss function. When used in multi-layer perceptron, how should we find out loss? Use Backpropagation.

Minimize the loss using differentiation. Keep moving towards the direction of global cost minimum by minus loss function.

![Backpropagation](image/back_propagation.png)

Then how will we find the gradient of multi-layered perceptron?

<Strong> Backpropagation </Strong>
Using chain rule, calculate gradient descent step by step.


![Backpropagation](image/back_propagation_2.png)

# My Example

I have implemented 2-layer perceptron, loss calculation and gradient calculation.

![example](image/my_example.png)

for loss funciton, i have used negative log- likelihood

![negative](image/negative_log_likelihood.png)

