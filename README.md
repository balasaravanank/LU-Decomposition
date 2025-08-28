# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner



## Algorithm

1. Input the matrix $A$ (and vector $b$ if solving equations).
2. Decompose $A$ into $L$ and $U$ using LU decomposition.
3. Display $L$ and $U$.
4. If $b$ is given, solve $Ax = b$ using forward and backward substitution to find $x$.

## Program:
(i) To find the L and U matrix
```python
/*
Program to find L and U matrix using LU decomposition.
Developed by: BALA SARAVANAN K
RegisterNumber: 212224230031
*/

import numpy as np
from scipy.linalg import lu

A = np.array(eval(input()))

p,l,u = lu(A)

print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```python
/*
Program to solve a matrix using LU decomposition.
Developed by: BALA SARAVANAN K
RegisterNumber: 212224230031
*/

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor, lu_solve 

a = np.array(eval(input()))
b = np.array(eval(input()))


l,p = lu_factor(a)
x = lu_solve((l,p),b)

print(x) 
```

## Output:
<img width="2508" height="1614" alt="Screenshot 2025-08-28 093605" src="https://github.com/user-attachments/assets/81553fd2-8dba-4c1d-9e30-8879a55b04c6" />
<img width="2515" height="1217" alt="Screenshot 2025-08-28 093617" src="https://github.com/user-attachments/assets/cb51db79-5ee7-4ee4-ab8f-1e233c278aa0" />




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

