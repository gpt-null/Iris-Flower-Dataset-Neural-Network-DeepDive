# Iris Flower Dataset Neural Network 

![top language](https://img.shields.io/github/languages/top/gpt-null/template)
![code size](https://img.shields.io/github/languages/code-size/gpt-null/template)
![last commit](https://img.shields.io/github/last-commit/gpt-null/template)
![issues](https://img.shields.io/github/issues/gpt-null/template)
![contributors](https://img.shields.io/github/contributors/gpt-null/template)
![License](https://img.shields.io/github/license/gpt-null/template)

##### **A Statquest implementation of [Neural Networks Pt. 4: Multiple Inputs and Outputs](https://www.youtube.com/watch?v=83LYR-1IcjA&list=PLblh5JKOoLUIxGDQs4LFFD--41Vzf-ME1&index=9)** see the video to better understand the process of this repo

## Description
This project explores the underlying mathematics of neural networks by implementing a simple classifier for the Iris dataset with manually set weights and biases. See each calculation with Linear and ReLU to see the math behind the model.

![alt text](assets/iris_dataset_image.png)

## TLDR
**A custom Neural network but instead of traning it i manually set the parameters to see the data flow through the model to see the underlying math.**

## Project Overview

Rather than allowing a neural network to learn weights through training, this project:
- Sets weights and biases manually
- Implements custom linear transformations and ReLU activation functions
- Visualizes decision boundaries in 3D space
- Demonstrates how each component affects the final classification results

## Neural Network Architecture

The model has a simple architecture:
- **Input Layer**: 2 nodes (petal_width, sepal_width)
- **Hidden Layer**: 2 nodes with ReLU activation
- **Output Layer**: 3 nodes (one for each Iris species: Setosa, Versicolor, Virginica)

![alt text](assets/output-onlinepngtools.png)

## Custom Implementation Details

The neural network uses:

1. **Manual Weight Initialization**:
   ```python
   # First layer weights and biases
   weights1 = [[-2.5, 0.6],
               [-1.5, 0.4]]
   bias1 = [1.6, 0.7]
   
   # Second layer weights and biases
   weights2 = [[-0.1, 1.5],
               [2.4, -5.2],
               [-2.2, 3.7]]
   bias2 = [0.0, 0.0, 1.0]
   ```

2. **Custom Linear Transformation**:
   - Matrix multiplication of inputs with weights
   - Addition of bias term
   
3. **Custom ReLU Activation**:
   - Element-wise function that returns max(0, x)
   - Implemented manually to show the computation

## Visualizations

The project includes comprehensive 3D visualizations showing:
- Probability surfaces for each class
- Decision boundaries between the three species
- How the feature space is divided based on the manually selected weights

![assets/](assets/output.png)

## Key Insights

This implementation demonstrates:
- How matrix operations and activation functions transform data through the network
- The impact of specific weight values on classification boundaries
- How a simple network with just 2 inputs and 2 hidden neurons can effectively separate the Iris classes
- The mathematical operations underlying "black box" neural networks




### LICENSE

```markdown
MIT License

Copyright (c) [year] [fullname]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```