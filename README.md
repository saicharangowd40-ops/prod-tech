# prod-techFactory Production Planner (A7)

1. Project Title

Factory Production Planner (A7)

2. Project Description

Factory Production Planner is a B.Tech Mathematics mini project that uses linear algebra and matrix methods to solve a real-world factory production problem.

A factory produces three different products using three different machines. Each machine has a limited number of working hours, and each product requires a different amount of time on each machine.

The project creates a mathematical system of linear equations and uses matrix rank analysis to determine whether the system is consistent. If the system is consistent, the program calculates the required production quantities. If the system is inconsistent, the program identifies the possible machine bottleneck.

3. Problem Statement

«A factory makes 3 products using 3 machines. Each machine has limited hours. Each product needs different time on each machine. Set up the system, find production quantities, and if the system is inconsistent, identify which machine is the bottleneck.»

4. Objectives

The main objectives of this project are:

- To represent a real-world factory problem mathematically.
- To form a system of linear equations.
- To represent the equations using matrices.
- To calculate the rank of the coefficient matrix.
- To calculate the rank of the augmented matrix.
- To check whether the system is consistent.
- To calculate production quantities when a unique solution exists.
- To identify possible bottlenecks when the system is inconsistent.
- To demonstrate the practical application of linear algebra.

5. Mathematical Concept

The project uses the matrix equation:

AX = B

Where:

- A = Coefficient matrix representing machine time required by products.
- X = Production quantity vector.
- B = Available machine-hours vector.

For three products and three machines:

[
A =
\begin{bmatrix}
a_{11} & a_{12} & a_{13}\
a_{21} & a_{22} & a_{23}\
a_{31} & a_{32} & a_{33}
\end{bmatrix}
]

[
X =
\begin{bmatrix}
x\
y\
z
\end{bmatrix}
]

[
B =
\begin{bmatrix}
b_1\
b_2\
b_3
\end{bmatrix}
]

Therefore:

[
AX=B
]

6. Consistency and Rank Analysis

The program compares:

[
Rank(A)
]

and

[
Rank([A|B])
]

where "[A|B]" is the augmented matrix.

Consistent System

If:

[
Rank(A)=Rank([A|B])
]

the system is consistent and a solution exists.

Inconsistent System

If:

[
Rank(A)\neq Rank([A|B])
]

the system is inconsistent.

This means the given machine-hour requirements cannot be satisfied simultaneously.

7. Input Variables

The program takes the following inputs:

Machine Availability

- Machine 1 available hours
- Machine 2 available hours
- Machine 3 available hours

Product Requirements

For each product, the user enters the number of hours required on each machine.

For example:

- Product 1 → Machine 1, Machine 2, Machine 3
- Product 2 → Machine 1, Machine 2, Machine 3
- Product 3 → Machine 1, Machine 2, Machine 3

8. Algorithm

The program follows these steps:

1. Start the program.
2. Read available hours for the three machines.
3. Read machine-time requirements for the three products.
4. Create the coefficient matrix "A".
5. Create the available-hours vector "B".
6. Create the augmented matrix "[A|B]".
7. Calculate "Rank(A)".
8. Calculate "Rank([A|B])".
9. Compare the two ranks.
10. If the system is consistent, solve "AX = B".
11. Display the production quantities.
12. Calculate machine utilization.
13. If the system is inconsistent, report the inconsistency and possible bottleneck.
14. Display the final result.

9. Technologies Used

- Python
- NumPy
- Linear Algebra
- Matrix Rank Analysis
- Google Colab / Jupyter Notebook

10. Python Libraries

The main Python library used is:

import numpy as np

NumPy is used for:

- Creating matrices
- Calculating matrix rank
- Solving systems of linear equations
- Performing matrix multiplication
- Performing numerical calculations

11. Expected Output

The program displays:

- Coefficient matrix "A"
- Available-hours matrix/vector "B"
- Augmented matrix "[A|B]"
- Rank of "A"
- Rank of "[A|B]"
- Consistency result
- Production quantities
- Machine usage
- Possible bottleneck information

12. Real-World Application

This mathematical model can be applied to manufacturing and production planning.

Examples include:

- Manufacturing industries
- Steel production
- Automobile manufacturing
- Food production
- Textile industries
- Small-scale factories
- Bakery production planning

The model helps understand how limited machine resources affect production.

13. Advantages

- Simple mathematical model.
- Uses real-world factory data.
- Demonstrates practical use of matrices.
- Automatically checks system consistency.
- Calculates production quantities.
- Helps identify resource constraints.
- Easy to implement using Python.

14. Limitations

- The current model considers only three products and three machines.
- It assumes fixed machine requirements.
- It does not consider product profit or cost optimization.
- Production quantities may need additional constraints to be physically meaningful.
- Real factories may require more advanced optimization techniques.

15. Future Scope

The project can be improved by adding:

- Graphical User Interface (GUI)
- More products and machines
- Production cost calculation
- Profit maximization
- Machine utilization charts
- Automatic bottleneck detection
- Sensitivity analysis
- Database support
- Interactive dashboards

16. Conclusion

The Factory Production Planner demonstrates how linear algebra and matrix rank analysis can solve practical production-planning problems.

By converting factory machine requirements into a system of linear equations, the project determines whether the production plan is mathematically feasible. When a solution exists, the required production quantities can be calculated. When the system is inconsistent, the project helps identify resource constraints and possible bottlenecks.

This project connects mathematical concepts such as matrices, systems of equations, consistency, and rank with a practical industrial application.

17. Project Structure

Factory-Production-Planner/
│
├── factory_production_planner.py
├── README.md
└── screenshots/
    ├── input.png
    ├── matrix_output.png
    └── result.png

18. How to Run

Step 1

Install Python.

Step 2

Install NumPy:

pip install numpy

Step 3

Run the Python program:

python factory_production_planner.py

Step 4

Enter the machine hours and product requirements when prompted.

Step 5

View the matrix, rank, consistency, production quantity, and bottleneck results.

---

Author

B.Tech Mathematics Mini Project

Project: Factory Production Planner (A7)

Mathematical Concept: Consistency and Rank Analysis
