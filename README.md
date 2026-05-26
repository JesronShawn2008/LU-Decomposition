# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. 
2. 
3. 
4. 

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

