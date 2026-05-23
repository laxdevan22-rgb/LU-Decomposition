# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the required libraries such as NumPy and SciPy.
2. Create and store the matrix using a NumPy array.
3. Apply LU Decomposition using the scipy.linalg.lu() function.
4. Display the Lower triangular matrix (L), Upper triangular matrix (U), and Permutation matrix (P).

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: V.lakshita Rai
RegisterNumber: 212225220054
'''
import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"

import numpy as np
from scipy.linalg import lu

A = np.array(eval(input()))

P, L, U = lu(A)

print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: V.Lakshita Rai
RegisterNumber:212225220054 
'''
import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"

import numpy as np
from scipy.linalg import lu_factor, lu_solve

A = np.array(eval(input()))
B = np.array(eval(input()))

lu, piv = lu_factor(A)

X = lu_solve((lu, piv), B)

print(X)

```

## Output:
<img width="1230" height="586" alt="image" src="https://github.com/user-attachments/assets/0fe27aed-a32f-4e5f-b3fa-54305f46a621" />
<img width="1244" height="340" alt="image" src="https://github.com/user-attachments/assets/55fef3c2-073e-493c-9c74-12baefa96e72" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

