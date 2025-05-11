# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1:
Import the required module SciPy using from scipy.linalg import lu and NumPy using import numpy as np.

### Step 2:
Define the square matrix using np.array().

### Step 3:
Use the function lu() from SciPy to perform LU Decomposition.
This function returns three matrices: P (permutation matrix), L (lower triangular matrix), and U (upper triangular matrix).

### Step 4:
Store the returned values in three variables: P, L, and U.

### Step 5:
Display the matrices P, L, and U using the print() function.
### Step 6:
End the program.

## Program:
```
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
## Output:
![alt text](<Screenshot 2025-05-11 182148.png>)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

