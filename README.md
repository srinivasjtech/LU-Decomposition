# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

1. Read the input matrix (and right-hand side vector for solving equations) from the user.
2. Convert the given input into a NumPy array.
3. Apply LU decomposition to factorize the matrix into Lower triangular matrix (L) and Upper triangular matrix (U).
4. Display the L and U matrices, and if required, solve the system of linear equations using the decomposed matrices.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Srinivas J
RegisterNumber: 212225230276'''
import numpy as np
from scipy.linalg import lu
a=eval(input())
p,l,u=lu(a)
print(l)
print(u)

```

(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: Srinivas J
RegisterNumber: 212225230276
'''
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
b=np.array(eval(input()))
p,l,u=lu(a)
i=np.linalg.solve(l,p@b)
c=np.linalg.solve(u,i) 
print(c)

```

## Output:
(i) To find the L and U matrix

<img width="1842" height="839" alt="Screenshot 2026-03-08 091150" src="https://github.com/user-attachments/assets/2b9de816-9673-42db-a27a-854c12a7d7b3" />


(ii) To find the LU Decomposition of a matrix

<img width="1439" height="796" alt="Screenshot 2026-03-08 091210" src="https://github.com/user-attachments/assets/fab5e1e3-c48d-4faf-989f-e43202d81835" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

