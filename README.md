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
## Step 1:
Import the required modules:

Use from scipy.linalg import lu to import the LU decomposition function from the SciPy library.

Use import numpy as np to import the NumPy library for numerical operations.

### Step 2:
Define the input matrix (it must be a square matrix) using np.array().

### Step 3:
Call the lu() function by passing the defined matrix as an argument.
This function will return three matrices:

P: Permutation matrix

L: Lower triangular matrix

U: Upper triangular matrix

### Step 4:
Store the output of the lu() function into three variables: P, L, and U.

### Step 5:
Display the matrices P, L, and U using the print() function.

### Step 6:
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

