# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. First, import the lu_factor and lu_solve functions from the scipy.linalg module. These functions are used to perform LU decomposition and solve linear systems using LU decomposition, respectively.
2. Use the eval(input()) function to take user inputs for matrix a (the coefficient matrix) and vector b (the right-hand side vector). These inputs should be entered in a format that Python can interpret as arrays, like lists of numbers.
3. Use lu_factor(a) to compute the LU decomposition of matrix a
4. Use lu_solve((lu, piv), b) to solve the linear system 
𝐴
𝑥
=
𝑏
Ax=b where A is the matrix a, x is the solution vector, and b is the right-hand side vector. This function returns the solution vector X.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: 
RegisterNumber: 
'''
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
/*
Program to find the L and U matrix.
Developed by: 
RegisterNumber: 
*/
```
(ii) To find the LU Decomposition of a matrix
```

/*
Program to find the LU Decomposition of a matrix.
Developed by: 
RegisterNumber: 
*/
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv = lu_factor(a)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:

![Screenshot 2024-12-15 015328](https://github.com/user-attachments/assets/034f4021-569d-4b01-87f3-faa386e02abd)

![Screenshot 2024-12-15 015311](https://github.com/user-attachments/assets/58bf888c-ed5c-46fd-bf55-8fb149dd46aa)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

