# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2.Import the necessary libraries(numpy,scipy.linalg)
3.Define the matrix using numpy
4.Use lu(),lu_solve(),lu_factor() to get the solutions
5.End the program
  

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Mohan K
RegisterNumber: 212225240087
*/
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
Developed by: Mohan K
RegisterNumber: 212225240087
*/
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),b)
print(x)

```

## Output:
<img width="1359" height="985" alt="Screenshot 2026-03-24 155824" src="https://github.com/user-attachments/assets/376f9e11-d3ad-4110-95e1-d8bf6b43c76f" />
<img width="1564" height="1068" alt="Screenshot 2026-03-24 155841" src="https://github.com/user-attachments/assets/8291e519-4a6c-42a6-828d-35dd4509baf8" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

