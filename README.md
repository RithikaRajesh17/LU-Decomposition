# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1:  
Import the required libraries numpy and scipy.linalg for matrix operations and LU decomposition.

### Step 2:  
Input the matrix(or matrices) using eval(input()).  

### Step 3:  
Perform LU decomposition using lu() or solve the system of equations using lu_factor() and lu_solve().  

### Step 4:  
Display the results - print L and U matrices or solution X matrix.  
 

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

