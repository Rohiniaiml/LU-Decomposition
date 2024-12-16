# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. mIport numpy as np: This imports the NumPy library
2. From scipy.linalg import lu: This imports the LU decomposition function from SciPy's linear algebra module, which allows you to compute the LU decomposition of a matrix.

3. Evaluates the input string and converts it into a valid Python object. In this case, it's assumed that the user inputs a matrix in a format like [[1, 2], [3, 4]].
4. np.array(): This converts the evaluated input into a NumPy array, representing the matrix A.
5. End this program

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: 
RegisterNumber: 
*/
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
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
![Screenshot 2024-12-16 131912](https://github.com/user-attachments/assets/12ddbc7b-0a28-41da-8665-136b1f6e7ea3)
![Screenshot 2024-12-16 131931](https://github.com/user-attachments/assets/52f3dde3-73d9-4743-b562-c4beadbf4bd7)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

