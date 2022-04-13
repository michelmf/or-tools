# OR-Tools - Assignment

Assignment for the Linear Programming class @ CEFET/PPCIC. This assignment aims to present a numerical solver and how to use it to tackle small and medium-size problems. 

## About OR-Tools

From the official [website](https://developers.google.com/optimization): 

> OR-Tools is an open-source software suite for optimization, tuned for tackling the world's most challenging problems in [vehicle routing](https://developers.google.com/optimization/routing), [flows](https://developers.google.com/optimization/flow), [integer and linear programming](https://developers.google.com/optimization/lp), and [constraint programming]().
>
> After modeling your problem in the programming language of your choice, you can use a half dozen solvers to solve it: commercial solvers such as Gurobi or CPLEX, or open-source solvers such as SCIP, GLPK, or Google's GLOP and award-winning CP-SAT.

This repo contains some examples of using OR-Tools with Python Programming Language and the GLOP Solver.

## How to install OR-Tools

OR-Tools is available in different programming languages such as C++, Python, Java, and C#. In this assignment, I am focusing on the Python programming language. Getting the package is straightforward using pip:

> python -m pip install --upgrade --user ortools

For more installation options or different languages, this [link](https://developers.google.com/optimization/install) is helpful. 

## Solving linear programming Problems with OR-Tools

OR-Tools provides a wrapper (MPSolver) to use different solvers, including GLOP. Below is the list of LP solvers available in OR-Tools:

* Clp 
* CPLEX
* GLOP
* GLPK
* Gurobi
* PDLP
* Xpress

Some solvers implement the Simplex Algorithm, while others implement Interior-Point or First-order methods. For further information about it, check the following [link](https://developers.google.com/optimization/lp/lp_advanced).

## Examples

Here some examples to understand the or-tools syntax to tackle LP problems. The notebooks and examples are written in portuguese. 

* example1.ipynb - First example showing how to solve a simple linear programming problem with two variables using GLOP and the Graphical Method.
* example2.ipynb - Classic optimization example where one needs to maximize the profit with furniture sales by choosing the best combination of each product.
* example3.ipynb - TBD...

## Requirements

To run the examples/notebooks, one needs the following packages:

* ortools
* NumPy
* scipy
* matplotlib
* plotly

## References

* Official website: https://developers.google.com/optimization
* OR-Tools project: https://github.com/google/or-tools#codemap
* GLOP Source Code: https://github.com/google/or-tools/tree/stable/ortools/glop