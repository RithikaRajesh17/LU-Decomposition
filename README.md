# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## i) Algorithm to Find the L and U Matrix
### Step 1:  
Import the required libraries numpy and scipy.linalg for matrix operations and LU decomposition.

### Step 2:  
Input the matrix using eval(input()).

### Step 3:  
Perform LU decomposition using lu() which returns the permutation matrix P, lower triangular matrix L, and upper triangular matrix U.

### Step 4:  
Display the results – print the L and U matrices.

## ii) Algorithm to Find the LU Decomposition and Solve the System
### Step 1:  
Import the required libraries numpy and scipy.linalg for matrix operations and solving linear equations.

### Step 2:  
Input the coefficient matrix A and the constant matrix (vector) b using eval(input()).

### Step 3:  
Perform LU decomposition using lu_factor(A), and solve the system of equations using lu_solve((lu, piv), b).

### Step 4:  
Display the result – print the solution matrix/vector X.





## Program:
(i) To find the L and U matrix
``` python


Program to find the L and U matrix.
Developed by: Rithika R
RegisterNumber: 212224240136

import numpy as np
from scipy.linalg import lu

A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

```

(ii) To find the LU Decomposition of a matrix

```python

Program to find the LU Decomposition of a matrix.
Developed by: Rithika R
RegisterNumber: 212224240136

import numpy as np
from scipy.linalg import lu_factor,lu_solve

A = np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)


```


## Output:
(i) L and U matrix

![image](https://github.com/user-attachments/assets/6d159b72-3904-4f5c-80b8-5bdce0b3fb8d)
(ii) LU Decomposition of a matrix

![Screenshot 2025-04-26 185636](https://github.com/user-attachments/assets/55e9be43-2990-476b-8f8a-e1d876a002cf)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

