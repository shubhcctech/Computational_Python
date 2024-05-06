<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   
</head>

<body>
    <h1>Lagrange Interpolation for Pressure Estimation README</h1>
    <h2>Overview:</h2>
    <p>Interpolation is a mathematical technique used to estimate values between known data points. One common method is Lagrange interpolation, which constructs a polynomial function passing through a set of data points. This README provides an overview of Lagrange interpolation and explains the provided Python code, which demonstrates the estimation of pressure values at given temperature points using Lagrange interpolation.</p>
    <h2>Explanation of Lagrange Interpolation:</h2>
    <p>Lagrange interpolation constructs a polynomial function, denoted as P(x), that passes through a given set of data points (x_i, y_i), where i = 0, 1, 2, ..., n-1. The Lagrange interpolation polynomial is defined as:</p>
    <p>P(x) = ∑_{i=0}^{n-1} y_i * l_i(x)</p>
    <p>where l_i(x) are the Lagrange basis polynomials defined as:</p>
    <p>l_i(x) = ∏_{j=0, j ≠ i}^{n-1} (x - x_j) / (x_i - x_j)</p>
    <h2>Explanation of Provided Python Code:</h2>
    <p>The provided Python code demonstrates Lagrange interpolation for estimating pressure values at given temperature points. Here's a breakdown of the code:</p>
    <ul>
        <li><strong>lagrange_interpolation Function:</strong> Implements Lagrange interpolation. It takes three parameters: x (Array of x-coordinates), y (Array of y-coordinates), and x_val (Value at which interpolation is to be performed).</li>
        <li><strong>Data Points:</strong> Defines arrays temperature and pressure representing known temperature-pressure data points.</li>
        <li><strong>User Input:</strong> Prompts the user to input a list of temperatures at which pressure is to be calculated.</li>
        <li><strong>Interpolation:</strong> Calls the Lagrange interpolation function with the temperature and pressure data along with the user-input temperature points.</li>
        <li><strong>Plotting:</strong> Plots the known data points as dots and the interpolated points as a continuous line for visualization.</li>
    </ul>
    <h2>How to Use:</h2>
    <ol>
        <li>Ensure you have Python installed on your system. Install the required libraries: numpy and matplotlib.</li>
        <li>Copy the provided code into a Python file (e.g., interpolation_example.py).</li>
        <li>Run the Python script. Enter the temperatures at which you want to interpolate pressures when prompted.</li>
        <li>View the plotted graph showing the original data points and the interpolated points.</li>
    </ol>
   
</body>

</html>
