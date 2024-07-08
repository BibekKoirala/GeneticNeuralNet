# Neural Network Training Algorithms

This repository contains implementations of neural network training algorithms, including a `genetic algorithm-based` approach and a `gradient descent-based` approach. The repository features a `custom` NeuralNetwork class trained using a genetic algorithm and an MLP3 class trained using gradient descent.

## Table of Contents

- [Introduction](#introduction)
- [Classes](#classes)
  - [Weight](#weight)
  - [NeuralNetwork](#neuralnetwork)
  - [MLP3](#mlp3)
- [Function for Training Genetic Algorithm (GA)](#function-for-training-genetic-algorithm-(ga))
- [Comparison of Algorithms](#comparison-of-algorithms)
    - [Error curve for gradient descent](#error-curve-for-gradient-descent)
    - [Error curve for Genetic Algorithm](#error-curve-for-genetic-algorithm)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This repository explores different methods for training neural networks. We implement a genetic algorithm, a bio-inspired optimization technique, and compare it to traditional gradient descent methods.

## Classes

### Weight

The `Weight` class manages the parameters of the neural network. This class handles the initialization, updating, and management of weights, making the model's learning process more efficient.

### NeuralNetwork

The NeuralNetwork class employs a genetic algorithm for training. This evolutionary approach uses selection, crossover, and mutation to optimize the network's weights.

### MLP3

The MLP3 class is a multi-layer perceptron that uses gradient descent for training. This class updates the network's weights iteratively to minimize the loss function.

## Function for Training Genetic Algorithm (GA)

```
GA()
   initialize population 
   find fitness of population

   while (termination criteria is reached) do
      parent selection
      crossover with probability pc
      mutation with probability pm
      decode and fitness calculation
      survivor selection
      find best
   return best
```

## Comparison of Algorithms

Genetic algorithms are bio-inspired algorithms known for their ability to solve convex optimization problems. Unlike gradient-based algorithms, which often fall into local minima and may not reach the global minimum, genetic algorithms use evolutionary principles to explore the solution space more comprehensively.

While gradient-based algorithms can efficiently find solutions, they sometimes get stuck in suboptimal points. In contrast, bio-inspired algorithms like the Genetic Algorithm employ mechanisms such as selection, crossover, and mutation to escape local optima and search for more optimal solutions. This characteristic makes genetic algorithms particularly effective for complex optimization problems where a global solution is desired.

### Error curve for gradient descent
![alt text](https://github.com/BibekKoirala/GeneticNeuralNet/blob/main/GradientDescent_Loss.png?raw=true)

### Error curve for Genetic Algorithm
![alt text](https://github.com/BibekKoirala/GeneticNeuralNet/blob/main/GeneticAlgo_Loss.png?raw=true)

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes or improvements.

## License

This project is licensed under the MIT License. See the LICENSE file for details.