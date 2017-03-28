Notes on this from: /Users/austinbrian/dev/DC-DSI4/curriculum/linear-algebra/01-week-matrices/dsi4-linalg-1.pdf

Matrix addition
* Matricies must be identical dimensions
* Element-wise addition, so the top-left is added to the top-left and so on

Scalar multiplication
* A multiple scaling number applies to each number individual number in the matrix

Matrix multiplication
* The number of columns in the first matrix must equal the number of rows in the second matrix
* Addition works like you "say" the name :
  * First row x first column = top left element
    * multiply the entries piece wise, so top left by top left, then add to multiplied top right by bottom left

Matrix transposition
* This flips a matrix on its bottom-right-to-top-left axis
  * Those values stay the same, while the others flip location

Inverse of matrix
* The main property of an inverse matrix is that when multiplied by the un-inverse of itself is the identity matrix (I)
  * $A$
  * Identity matrix has one on the bottom-right-to-top left diagonal and zeros everywhere else
* After a matrix is transposed, it is no longer invertable

Determinant of a Matrix
* Will almost always be done by computers
* Determinant helps us find the identity matrix

Classes of Matrices
* Row vector: one row only
* Column vector: one column only
* Square matrix: same number of rows and columns
* Symmetric matrix: Transpose of a matrix is the same as the matrix - e.g., correlation matrix
* Upper triangular: upper right values are the only nonzero values, everything below or on the diagonal is zero
* Lower triangular: nonzero values are below the diagonal, and everything above (or on) the diagonal is zero
* Orthogonal matrix: a matrix's transpose is equal to its identity
