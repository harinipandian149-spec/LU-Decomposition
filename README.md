# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
## 5a
1. import the required numpy and scipy libraries.
2. get the input from the user 
3. use the lu() function to decompose the matrix into lower
  triangular(L) and upper triangular(U) matrices.
4. display the matrices as output

## 5b
1. import the required numpy and scipy libraries.
2. get the input from the user 
3. use lu_factor and lu_solve to factorise and solve the matrix
4. display the matrices as output.

## Program:
(i)5a. To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Harini P
RegisterNumber: 26008597
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
(ii)5b. To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Harini P
RegisterNumber:26008597 
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
l,p=lu_factor(a)
x=lu_solve((l,p),b)
print(x)
```

## Output:
## 5a.
<img width="1306" height="821" alt="Screenshot 2026-10-15 081749" src="https://github.com/user-attachments/assets/a3e3524d-e2b6-4b64-b623-7c419293315a" />



## 5b.
<img width="1255" height="821" alt="Screenshot 2026-10-15 081808" src="https://github.com/user-attachments/assets/506f13ed-91d0-4eb6-8550-3991a110d30c" />






## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

