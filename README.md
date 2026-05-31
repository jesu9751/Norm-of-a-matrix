# Norm of a matrix
## Aim
To write a program to find the 1-norm, 2-norm and infinity norm of the matrix and display the result in two decimal places.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
	1. Get the input matrix using np.array()   
    2. Find the 2-norm of the matrix using np.linalg.norm()
	3. Print the norm of the matrix in two decimal places.
## Program:
```Python
# Register No:212225040154
# Developed By:Jesu Joyal J
# 1-Norm of a Matrix
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"

A=eval(input())
rows=len(A)
cols=len(A[0])
max_sum=0
for j in range(cols):
    col_sum=0
    for i in range(rows):
        col_sum += abs(A[i][j])
    if col_sum > max_sum:
        max_sum = col_sum
print("{:.2f}".format(max_sum))        



# 2-Norm of a Matrix
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
matrix = eval(input())
norm = np.linalg.norm(matrix,2)
print(f"{norm:.2f}")





# Infinity Norm of a Matrix

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
matrix=eval(input())
norm = np.linalg.norm(matrix,np.inf)
print(f"{norm:.2f}")







# 2-Norm of a Matrix




# Infinity Norm of a Matrix





```
## Output:
### 1-Norm of a Matrix

<img width="760" height="813" alt="image" src="https://github.com/user-attachments/assets/b562d8ec-737c-4e62-819b-7b138dbc78e9" />

### 2-Norm of a Matrix

<img width="759" height="884" alt="image" src="https://github.com/user-attachments/assets/3f5d1682-acb0-4e45-82a1-21afafe83731" />


### Infinity Norm of a Matrix

<img width="680" height="902" alt="image" src="https://github.com/user-attachments/assets/d987eb88-76c6-463c-8094-9ee34cdf93c7" />



## Result
Thus the program for 1-norm, 2-norm and Infinity norm of a matrix are written and verified.
