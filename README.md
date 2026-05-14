# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### step1.Start the program and import the required libraries (NumPy and SciPy). 
### step2.Define the matrix using NumPy. 
### step3.Use lu() to perform LU decomposition and display the lower and upper triangular matrices.
### step4.Use lu_factor() and lu_solve() to factorize the matrix and solve the system of equations.
### step5.Display the solution and end the program.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: SHRIHARI M
RegisterNumber: 212225230265 
'''
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
'''Program to solve a matrix using LU decomposition.
Developed by: SHRIHARI M
RegisterNumber: 212225230265
'''
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
![lu decomposition]()
<img width="1217" height="454" alt="image" src="https://github.com/user-attachments/assets/0bdbbff2-d7b1-42b6-b483-91300af6204d" />
<img width="1004" height="188" alt="image" src="https://github.com/user-attachments/assets/d29e309e-f59c-49e2-b742-656f7bf31d54" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

