### Types:

$\rightarrow$ Row Matrix - A matrix having a single row
   
   Example - $\begin{bmatrix} 2 & 3 & 4 \end{bmatrix}$
   

$\rightarrow$ Column matrix - A matrix having only a single column 
   
   Example - $\begin{bmatrix} 5 \\ 2 \\ 1\end{bmatrix}$
   
   
$\rightarrow$ Square matrix : A matrix having equal number of rows and column 
   Example - $\begin{bmatrix} 2 & 0 & -1 \\ 5 & 3 & 2 \\ 1 & 7 & 3\end{bmatrix}$

$\rightarrow$ Rectangular matrix - A matrix having unequal number of rows and columns.
   Example - $\begin{bmatrix} 2 & 0 & -1 \\ 1 & 7 & 3\end{bmatrix}$

$\rightarrow$ Null matrix - If all elements of a matrix is zero it is called null or zero matrix and it is shown by 0
  
  Example - $\begin{bmatrix}0 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 0\end{bmatrix}$

$\rightarrow$ Diagonal matrix - A square matrix in which all the elements except the main diagonal are zero.
   
   Example - $\begin{bmatrix}2 & 0 & 0 \\ 0 & 3 & 0 \\ 0 & 0 & 5\end{bmatrix}$
   
$\rightarrow$ Scalar matrix - In a diagonal matrix if all elements are equal the matrix is Scalar.

   Example - $\begin{bmatrix}3 & 0 & 0 \\ 0 & 3 & 0 \\ 0 & 0 & 3\end{bmatrix}$

$\rightarrow$ Unit/Identity matrix - A diagonal matrix whose all element on the main diagonal are equal to one. The unit matrix is usually shown by letter I.

   Example - $I$ = $I_{3}$ = $\begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1\end{bmatrix}$

$\rightarrow$ Transpose matrix - if the rows and columns of a matrix A are interchanged then the resulting matrix is called transpose of A matrix. It is denoted by $A'$/ $A^T$ 

   Example - $A$ = $\begin{bmatrix}3 & 2 & 6 \\ 1 & 5 & 0 \\ 4 & 3 & 2\end{bmatrix}$   $A' = A^T \begin{bmatrix} 3 & 1 & 4 \\ 2 & 5 & 3 \\ 6 & 0 & 2\end{bmatrix}$

$\rightarrow$ Symmetric Matrix - A matrix is Symmetric when $A = A^T$

   Example - $A = \begin{bmatrix} 1& 2 \\ 2 & 4\end{bmatrix} \; ,A^T = \begin{bmatrix}1 & 2 \\ 2 & 4\end{bmatrix}$  
   
   $B = \begin{bmatrix} 3 &1&2\\1&0&-1\\2&-1&5\end{bmatrix} \;,B^T = \begin{bmatrix}3&1&2\\1&0&-1\\2&-1&5\end{bmatrix}$

$\rightarrow$ Skew symmetric matrix - A matrix A is called skew-symmetric if $A = -A^T.$ 

   Example - $A = \begin{bmatrix}0&-1\\1&0\end{bmatrix} \; ,A^T = \begin{bmatrix} 0&1\\-1&0\end{bmatrix}$
* Diagonal must be 0.

### Operation of matrixes:

$\rightarrow$ Addition and subtraction.
= Let, A and B are two matrixes. If A+B are equal 

<u>Example</u>

$\begin{bmatrix} 2&0&-7 \\ 3&2&5\end{bmatrix}_{2X3} \;\;+\;\;\begin{bmatrix}1&-5&-2 \\-1&0&3\end{bmatrix}_{2X3}\;\;\Rightarrow\;\;\begin{bmatrix}3&-5&-9\\2&2&8\end{bmatrix}_{2X3}$

The Operations Addition are commutative
  $\rightarrow$ Multiplication.
  = Let, A and B are two matrixes of order $nXm$ and $pXq$ , if the multiplication operation that is AB valid then $\boxed{m = p}$ 
 $\star\star$
Q) A and B are two matrixes of order $5X1$ and $1X4$ , Justify whether     $AB$ is possible or not. If $AB$ is possible then find the order of $AB$.         Justify the multiplication $BA$ is possible or not.

Ans. $5 \overset{A}{X}\boxed{1\;\;=\;\;1}\overset{B}{X}4 = 5X4$ 

Since, the no if columns of matrics A equal to the no. of rows on matrics B $\therefore$ The multiplication $AB$ is possible.

The order of $AB$ is 5X4 
   
   $\;\;\;\;\;1\overset{B}{X}\boxed{4\;\;\neq\;\;5}\overset{A}{X}1$

Since, the no of columns of matrics B is not equal to the no of rows of matrics A $\therefore$ The multiplication $BA$ is not possible.

<u>Example</u>

$A\;\;=\;\;\;\;\;\begin{bmatrix}2&-1\\\hline0&3\\5&2\end{bmatrix}_{3X2}\;\;\;B\;\;=\;\;\begin{bmatrix}1 &\mid& 3 & 0 \\ 2 &\mid&-1 & 4 \end{bmatrix}_{2X3}$

$\mathcal{AB}\;\;=\;\;\begin{bmatrix}(2X1)+(-1)X2&2X3+(-1)X(-1)&2X0+(-1)X4\\0X1+3X2&0X3+3X(-1)&0X0+3X4\\5X1+2X2&5X3+2(-1)&5X0+2X4\end{bmatrix}$

$\;\;\;\;\;\;\;\;=\;\;\begin{bmatrix}0&7&-4\\6&-3&12\\9&13&8\end{bmatrix}_{3X3}$

$\mathcal{BA}\;\;=\;\;\begin{bmatrix}2+0+0&-1+9+0\\4-0+20&-2-3+8\end{bmatrix}\;\;\;=\begin{bmatrix}2&8\\24&3\end{bmatrix}_{2X2}$


$\rightarrow$ Here $\boxed{\mathcal{AB}\;\;\neq\;\;\mathcal{BA}}\;\;\;\therefore$  A and B are not commutative.

Q) $\mathcal{A}\;\;=\;\;\begin{bmatrix}2&0\\1&2\end{bmatrix}\;\;;\;\;\mathcal{B}\;\;=\;\;\begin{bmatrix}3&1\\5&0\end{bmatrix}\;\;;\;\;\mathcal{C}\;\;=\;\;\begin{bmatrix}7&2\\-5&-1\end{bmatrix}$ prove that 

$i\rangle$ (AB)C = A(BC) (Associative) 

$\mathcal{AB}\;\;=\;\;\begin{bmatrix}6+0&2+0\\3+10&1+0\end{bmatrix}\;\;=\;\;\begin{bmatrix}6&2\\13&1\end{bmatrix}^{AB}\begin{bmatrix}7&2\\-5&-1\end{bmatrix}^C\;\;=\;\;\begin{bmatrix}42+(-10)&12-2\\91-5&26-1\end{bmatrix}$
$\;\;\;\;\;\;\;\;=\;\;\begin{bmatrix}32&10\\86&25\end{bmatrix}$  

$\mathcal{BC}\;\;=\;\;\begin{bmatrix}21-5&6-1\\35-0&10-0\end{bmatrix}\;\;=\begin{bmatrix}16&5\\35&10\end{bmatrix}^{BC}$

$\mathcal{A(BC)}\;\;=\;\;\begin{bmatrix}2&0\\1&2\end{bmatrix}\begin{bmatrix}16&5\\35&10\end{bmatrix}\;\;=\;\;\begin{bmatrix}32+0&10+0\\16+70&5+20\end{bmatrix}\;\;=\;\;\begin{bmatrix}32&10\\86&25\end{bmatrix}$

$\therefore$ proved that (AB)C = A(BC) (Associative) 

## Determinant

If atleast two rows or columns are equal in any determinant then the value of that determinant is equal to '0'

Example:

$\begin{vmatrix}+5&-3&+2\\\hline-4&+0&-1\\-3&-2&+5\end{vmatrix}$ = 50(0+2)- 3(20-3)+2(8-0) =10- 51 + 16 = 26-51 = -25

<font color="chartreuse"><u>Formula</u></font> = $(-1)^{row+column}$ .
<font color ="seafoam"><u>Minors</u></font> - 
minor of (5)      minor of (3)     minor of (2)
= $\begin{vmatrix}0&-1\\2&5\end{vmatrix}\;\;\;\;\;\;\;\;\;\;\;-\begin{vmatrix}4&-1\\-3&5\end{vmatrix}\;\;\;\;\;\;\;\;\;\;\begin{vmatrix}4&0\\-3&2\end{vmatrix}$  
$= 2\;\;\;\;\;\;\;\;\;\;\;\;\;$ $\;\;\;\;\;\;\;\;=-17\;\;\;\;\;\;\;\;\;\;\;\;$ $\;\;\;\;\;=8$      
minor of (4)       minor of (0)    minor of (-1)
= $\begin{vmatrix}-3&2\\2&5\end{vmatrix}\;\;\;\;\;\;\;\;\;\;\;\;\begin{vmatrix}5&2\\-3&5\end{vmatrix}\;\;\;\;\;\;\;\;\;\;\;\;-\begin{vmatrix}5&3\\-3&7\end{vmatrix}$  
$= -11\;\;\;\;\;\;\;\;\;\;\;\;\;$ $\;\;\;\;=31\;\;\;\;\;\;\;\;\;\;\;\;$ $\;\;\;\;\;=8$  

minor of (-3)       minor of (2)    minor of (-5)
= $\begin{vmatrix}3&2\\0&-1\end{vmatrix}\;\;\;\;\;\;\;\;\;\;\;\;-\begin{vmatrix}5&2\\-4&-1\end{vmatrix}\;\;\;\;\;\;\;\;\;\;\;\;\begin{vmatrix}5&3\\4&0\end{vmatrix}$  
$= 2\;\;\;\;\;\;\;\;\;\;\;\;\;$ $\;\;\;\;\;\;\;\;\;\;=-17\;\;\;\;\;\;\;\;\;\;\;\;$ $\;\;\;\;\;\;=8$  

$-$Determinant of a matrix A is the determinant of transpose of that matrix.
$det(\mathcal{A}) = det(\mathcal{A}^\mathcal{T})$

$\begin{bmatrix}\frac{5}{3}&\frac{8}{3}&3\end{bmatrix}$

$\square$ Minors of Determinants are applicable for only square matrix

A = $\begin{bmatrix}0&-3&1\\2&-2&2\\5&0&5\end{bmatrix}$ minor of 0 = $\begin{bmatrix}-2&2\\0&5\end{bmatrix}$ minor of -3 = $-\begin{bmatrix}2&2\\5&5\end{bmatrix}$ = 0 

minor of 1 $\begin{bmatrix}2&-2\\5&0\end{bmatrix}$ = 10

