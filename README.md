# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### 1.Start the program and import the required libraries (NumPy and SciPy).
### 2.Define the matrix using NumPy.
### 3.Use lu() to perform LU decomposition and display the lower and upper triangular matrices.
### 4.Use lu_factor() and lu_solve() to factorize the matrix and solve the system of equations.
### 5.Display the solution and end the program.


## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Padmesh sivaram R
RegisterNumber: 212225240103
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]='1'
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Padmesh sivaram R
RegisterNumber:  212225240103
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,p=lu_factor(A)
x=lu_solve((lu,p),B)
print(x)


```

## Output:

<img width="1249" height="580" alt="Screenshot 2026-05-14 113959" src="https://github.com/user-attachments/assets/4bbb1826-0e7a-46f6-ad79-80579560cf8e" />
<img width="1232" height="237" alt="Screenshot 2026-05-14 114006" src="https://github.com/user-attachments/assets/0a23c69e-4033-48fc-a5c8-c2808f131b57" />






## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

