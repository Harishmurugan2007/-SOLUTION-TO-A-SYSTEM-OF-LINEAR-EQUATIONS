# -SOLUTION-TO-A-SYSTEM-OF-LINEAR-EQUATIONS
## Aim:
To write a python program to find a solution to a system of linear equations.
## Equipment’s required:
1. 	Hardware – PCs
2. 	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1: 
Import the numpy module to use the built-in functions for calculation
### Step 2: 
Prepare the lists from each linear equations and assign in np.array()
### Step 3: 
Using the np.linalg.solve(), we can find the solutions.
### Step 4: 
End the program
## Program:
        # Program to find the solution for the given linear equations.
        # Developed by: Harish M
        # RegisterNumber: 24006510

        import numpy as np

        # Coefficient matrix for the system x - 3y = 0, 3x + y = 10
        A = np.array([[1, -3], 
                    [3, 1]])

        # Constant terms
        B = np.array([0, 10])

        # Solve the system of equations
        try:
            solution = np.linalg.solve(A, B)
            # Display the solution
            print(f"{solution}")
        except np.linalg.LinAlgError:
            print("The system of equations does not have a unique solution.")

## Output:
![Result](<Screenshot 2024-12-10 202858.png>)
## Result: 
Thus the solutions for the linear equations are successfully solved using python program

