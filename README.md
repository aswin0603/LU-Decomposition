# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the NumPy module for calculation.
2. From scipy.linalg module, import lu that is used to find the LU Decomposition.
3. To find the L and U matrix, prepare the matrix using np.array() and use the function lu().
4. To find the LU Decomposition of the matrix, prepare the matrix using np.array() and use lu_factor() and lu_solve() functions to get the decomposed matrix.
5. Print the result and end the program.

## Program:
(i) To find the L and U matrix
```python
'''
Program to find the L and U matrix.
Developed by: Aswin B
RegisterNumber: 24900642
'''
import numpy as np
from scipy.linalg import lu
a = np.array(eval(input()))
P,L,U = lu(a)
print (L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```python
'''
Program to find the LU Decomposition of a matrix.
Developed by: Aswin B
RegisterNumber: 24900642
'''
import numpy as np
from scipy.linalg import lu_factor, lu_solve
a = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(a)
x = lu_solve((lu , piv),b)
print (x)

```

## Output:

### Output 1:
![Record 05-01](https://github.com/user-attachments/assets/00f7832f-89b1-4953-9a96-65d56d34ba06)

### Output 2:
![Record 05-02](https://github.com/user-attachments/assets/404ba9da-fadd-4a10-99bc-3e7ebaab1a1f)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

