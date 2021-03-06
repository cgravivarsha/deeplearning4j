---
title: Activations
short_title: Activations
description: Special algorithms for gradient descent.
category: Models
weight: 10
---

## What are activations?

At a simple level, activation functions help decide whether a neuron should be activated. This helps determine whether the information that the neuron is receiving is relevant for the input. The activation function is a non-linear transformation that happens over an input signal, and the transformed output is sent to the next neuron.

## Usage

The recommended method to use activations is to add an activation layer in your neural network, and configure your desired activation:

```java
GraphBuilder graphBuilder = new NeuralNetConfiguration.Builder()
	// add hyperparameters and other layers
	.addLayer("softmax", new ActivationLayer(Activation.SOFTMAX), "previous_input")
	// add more layers and output
	.build();
```

## Available activations

{{autogenerated}}