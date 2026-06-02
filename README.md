# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Read the input matrix A (and the right-hand side vector b if solving a linear system) and convert them into NumPy arrays.
2. Use the LU factorization function (lu_factor or lu) to decompose the matrix A into a lower triangular matrix L, an upper triangular matrix U, and a permutation/pivot matrix/vector (P or piv) that tracks row interchanges.
3. Pass the factorized components (lu, piv) along with the vector $b$ into the LU solver (lu_solve) to calculate the solution vector X.
4. Print the computed results, which will output either the individual matrices (L and U) or the final solution vector X depending on the experiment's specific objective.

## Program:
(i) To find the L and U matrix
```
/*
'''Program to find L and U matrix using LU decomposition.
Developed by: JESRON SHAWN C J
RegisterNumber: 212225100019
'''
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U = lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to solve a matrix using LU decomposition.
Developed by: JESRON SHAWN C J
RegisterNumber: 212225100019
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu,piv),b)
print(X)
```

## Output:

<img width="1207" height="456" alt="image" src="https://github.com/user-attachments/assets/adcfa5df-4cd4-4138-8b49-a48b53ad0eaa" />


<img width="1224" height="319" alt="image" src="https://github.com/user-attachments/assets/8bf1bd21-b388-495f-96ff-f9df2549fbb2" />




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

