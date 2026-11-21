# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries(numpy,scipy.linalg)
3. Use lu(),lu_solve(),lu_factor() to get the solutions
4. End the program

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: R.TEJASWINI
RegisterNumber: 212224230218
*/
```
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
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
Developed by: R.TEJASWINI
RegisterNumber: 212224230218
*/
```
```
# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),B)
print(X)
```
## Output:

<img width="1070" height="973" alt="image" src="https://github.com/user-attachments/assets/9f6cefd1-6de6-4cd7-8300-610e857117d4" />

<img width="862" height="950" alt="image" src="https://github.com/user-attachments/assets/bce4d79d-88aa-4d26-96c8-f66c16a08834" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

