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

### Algorithm
### Step 1:
Import the required modules:

Use import numpy as np to work with arrays.

Use from scipy.linalg import lu_factor, lu_solve to access LU decomposition and solution functions.

### Step 2:
Take input for the coefficient matrix A using eval(input()) and convert it into a NumPy array using np.array().

### Step 3:
Take input for the right-hand side matrix or vector B using eval(input()) and convert it into a NumPy array using np.array().

### Step 4:
Call the lu_factor(A) function:

It returns two values:

lu: Combined LU decomposition of matrix A

piv: Pivot indices for partial pivoting

### Step 5:
Use lu_solve((lu, piv), B) to solve the system of equations.
AX=B using the LU decomposition.

### Step 6:
Store the result in a variable (e.g., result), which contains the solution vector or matrix.
### Step 7:
Display the result using the print() function.
### Step 8:
End the program.

### Program:
```
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
piv,lu=lu_factor(A)
result=lu_solve((piv,lu),B)
print(result)
```

### Output:
![alt text](<Screenshot 2025-05-24 110008.png>)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

