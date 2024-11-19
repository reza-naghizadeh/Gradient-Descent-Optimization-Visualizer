# Gradient Descent Optimization Visualizer

This repository contains a MATLAB implementation of the **Gradient Descent** algorithm to minimize a quadratic function. The script visualizes the optimization process by plotting the path of the algorithm as it converges to the function's minimum point.

This code was developed as part of our Optimization course project at IASBS, in collaboration with my groupmate, [Erfan Faridi](https://github.com/erfanfaridii/).

## Features

- **Contour Plot Visualization**: Displays the contour plot of the quadratic function and the optimization path.
- **Gradient Descent Algorithm**: Implements the standard gradient descent update rule to iteratively find the minimum.
- **Learning Rate Control**: Uses a fixed learning rate to adjust the step size in each iteration.
- **Convergence Check**: Iterates until the change in the function's value is below a specified threshold.
- **Detailed Results**: Outputs the number of iterations, the minimum point, and the function value at the minimum.

## Prerequisites

- MATLAB R2016b or later.
- Symbolic Math Toolbox.

## Getting Started

### Clone the Repository
```bash
git clone https://github.com/username/Gradient-Descent-Optimization-Visualizer.git
cd Gradient-Descent-Optimization-Visualizer
```

### Run the Script

1. Open `gradient_descent_visualizer.m` in MATLAB.
2. Run the script.

### Output

- The script will display:
  - The number of iterations it took to converge.
  - The coordinates of the minimum point found by the algorithm.
  - The final value of the function at the minimum.
- A contour plot showing the optimization path and the points visited by the gradient descent algorithm.

## Customization

- **Initial Point**: Modify the initial point `x` in the script:
  ```matlab
  x = [-2, 2.5];
  ```

- **Learning Rate**: Adjust the learning rate to control the step size:
  ```matlab
  learningRate = 0.01;
  ```

- **Tolerance**: Change the stopping criteria based on the desired accuracy:
  ```matlab
  if (errorAmountx1 < 10e-4 && errorAmountx2 < 10e-4)
  ```

- **Function**: Replace the function `f` with any quadratic function:
  ```matlab
  f(x1, x2) = (10 * x1 ^ 2) - (4 * x1 * x2) + (x2 ^ 2);
  ```

## Example Output

The script minimizes the function:

\[
f(x_1, x_2) = 10x_1^2 - 4x_1x_2 + x_2^2
\]

and outputs the following:
- The number of iterations taken to reach convergence.
- The coordinates of the minimum point.
- The function value at the minimum.
- A contour plot with the optimization path overlaid.

## Acknowledgments

- MATLAB Documentation: [Symbolic Math Toolbox](https://www.mathworks.com/products/symbolic.html)
- Gradient Descent: [Wikipedia](https://en.wikipedia.org/wiki/Gradient_descent)
