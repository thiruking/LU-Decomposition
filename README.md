# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Define the package as scipy.linalg import lu.
2. Get input from user and print L and U matrix by 'print' .
3. Define a package as "from scipy.linalg import lu_factor, lu_solve" and create the variable as 'X' include the package in that variable
4. print the variable 'X'

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: THIRUMALAI K
RegisterNumber: 212224240176
'''
import numpy as np
from scipy.linalg import lu
a=eval(input())
b=np.array(a,dtype=float)
p,l,u=lu(b)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: THIRUMALAI K
RegisterNumber: 212224240176
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu,solve
a=np.array(eval(input()))
b=np.array(eval(input()))
p,l,u=lu(a)
pb=p @ b
y=solve(l,pb,lower=True)
x=solve(u,y)
print(x)

```

## Output:

<img width="1440" height="822" alt="image" src="https://github.com/user-attachments/assets/d3756c13-2745-4060-ab89-ceac976708d4" />
<img width="1513" height="694" alt="image" src="https://github.com/user-attachments/assets/27d85d3e-85ab-4c86-91ad-b8f45def2720" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

