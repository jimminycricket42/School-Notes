---
aliases: [ ]
tags: [GR10/Q4 apm ]
created: 24/10/2022 - 19:00
modified: 25/10/2022 - 07:16
---
# Matrices
A Matrix is an *ordered* array of numbers. These numbers can be manipulated through addition, subtraction, multiplication, or division, the same as any other number. However matrices have special properties that allow them to be used in interesting ways. ^blurb

## Ordering Matrices
Matrices have an order, defined by the columns and the rows. This order is linked to the size of the matrix. 

$$
\mathbf{x} = \begin{Bmatrix} 1 & 2 & 4 & 9 \\ 5 & 5 & 3 & 1 \\ 3 & 4 & 1 & 0 \end{Bmatrix}
$$

in this case we have three rows, and 4 columns. We can say:

$$ \mathbf{x} = 3 \times 4 $$

> [!Note]
> Rows always come before columns. 

### Positions in a Matrix (Members)
The positions of numbers in a matrix are denoted using subscript and the variable assigned to the matrix. Each position is called a *member* of a matrix
$$
\begin{gather}
\\& \mathbf{x} = 
\begin{Bmatrix}
a & b & c \\
d & e & f \\
\end{Bmatrix}
\\& \textrm{Order of: } x = 2\times3
\\& x_{2;3} = f
\\& x_{1;1} = a
\\& x_{2;2} = e
\end{gather}
$$

### Special matrix structures
There are many shapes of matrices, but there are 3 types that we exclusively define:
- Row Matrices
- Column Matrices
- Square Matrices

#### Row Matrices 
$$
\mathbf{x} =
\begin{Bmatrix}
a & b & c 
\end{Bmatrix}
$$

In this matrix there is only one row, so the order is always:
$$
\begin{gather}
\mathbf{x} = n \times 1
\\ \textrm{Row} = 1
\\ \textrm{Column} = -\infty < n < \infty 
\end{gather}
$$

#### Column Matrices 
$$
\mathbf{x} =
\begin{Bmatrix}
a \\ b \\ c 
\end{Bmatrix}
$$

In this matrix there is only one column, so the order is always:
$$
\begin{gather}
\mathbf{x} = n \times 1
\\ \textrm{Row} = -\infty < n < \infty 
\\ \textrm{Column} = 1 
\end{gather}
$$

#### Square Matrices 
$$
\mathbf{x} =
\begin{Bmatrix}
a & b & c \\
d & e & f \\
g & h & I \\
\end{Bmatrix}
$$

In this matrix there are the same amount of columns as there are rows, so we can say: 
$$
\begin{gather}
\mathbf{x} = n \times n
\\ \textrm{Row} = \textrm{Column} 
\end{gather}
$$

## Special Matrices
We look at a few different examples of special matrices:
- Diagonal Matrix
- Identity Matrix
- Zero Matrix
- Equal Matrices

### Diagonal Matrices
Diagonal matrices are [[#Square Matrices]] where every number not along the leading diagonal is 0. The leading diagonal is the diagonal that goes from the top left to the bottom right directly. 

$$
\begin{Bmatrix}
a & 0 & 0 \\
0 & b & 0 \\
0 & 0 & c \\
\end{Bmatrix}
$$

> [!Note]
> a; b; and c can be 0, but if all three are zero than the matrix is a [[#Zero Matrix]]

### Identity Matrix
Identity Matrices are the identies of multiplication for a matrix, meaning, any matrix multiplied by this matrix is equal to itself. Identity matrices are [[#Diagonal Matrices]] and [[#Square Matrices]]

$$
\begin{Bmatrix}
1 & 0 \\
0 & 1 \\
\end{Bmatrix}
$$

> [!note] 📔 Identity of a Matrix
> As discussed earlier, the matrix below is the [[#Identity Matrix|multiplication identity of any matrix]], and we can test this through the [[#Multiplication of Matrices]]
> 
> $$\begin{Bmatrix}
a & b & c \\
d & e & f \\
\end{Bmatrix} \times \begin{Bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{Bmatrix} = \begin{Bmatrix}
a(1) + b(0) + c(0) & a(0) + b(1) + c(0) & a(0) + b(0) + c(1) \\
d(1) + e(0) + f(0) & d(0) + e(1) + f(0) & d(0) + e(0) + f(1) \\
\end{Bmatrix} = \begin{Bmatrix}
a & b & c \\
d & e & f \\
\end{Bmatrix}$$

### Zero Matrix
Zero Matrices are square matrices where every contained value is 0

$$
\mathbf{b} = 
\begin{Bmatrix}
0 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 0 \\
\end{Bmatrix}
$$

### Equal Matrices
Equal matrices are when two matrices are the exact same at every index point. 

$$ \begin{gather}
\\& \mathbf{a} = 
\begin{Bmatrix}
a & b & c \\
d & e & f \\
\end{Bmatrix}
\\& \mathbf{b} = 
\begin{Bmatrix}
a & b & c \\
d & e & f \\
\end{Bmatrix}
\\& a = b
\end{gather}
$$

## Operations with matrices
We look at:
- Addition and subtraction
- Multiplication and division by a [[Vectors and Scalar|scalar]]
- Multiplication by another Matrix

### Addition and Subtraction with Matrices
Addition and subtraction with matrices is very similar to linear addition and subtraction. It relies on two matrices having the same [[#Ordering Matrices|order]]. To add or subtract matrices you add each position with it’s correlating position in the other matrix, and put that into the resultant matrix. 

$$\begin{gather}
\begin{Bmatrix}
a & b & c \\
d & e & f \\
\end{Bmatrix}
+
\begin{Bmatrix}
g & h & i \\
j & k & l \\
\end{Bmatrix}
=
\begin{Bmatrix}
a + g & b + h & c + i \\
d + k & e + k & f + l \\
\end{Bmatrix}

\end{gather}
$$

> [!example]+ 💡 Example: addition of matrices
> 
> $$\begin{Bmatrix}
1 & 3 & 4 \\
9 & 7 & 5 \\
\end{Bmatrix} +
\begin{Bmatrix}
2 & 9 & 3 \\
7 & 1 & 5 \\
\end{Bmatrix}
= \begin{Bmatrix}
1 + 2 & 3 + 9 & 4 + 3 \\
9 + 7 & 7 + 1 & 5 + 5 \\
\end{Bmatrix} =
\begin{Bmatrix}
3 & 12 & 7 \\
9 & 8 & 10 \\
\end{Bmatrix}$$

> [!example]+ 💡 Example: Subtraction of matrices
> 
> $$\begin{Bmatrix}
1 & 3 & 4 \\
9 & 7 & 5 \\
\end{Bmatrix} -
\begin{Bmatrix}
2 & 9 & 3 \\
7 & 1 & 5 \\
\end{Bmatrix}=
\begin{Bmatrix}
1 - 2 & 3 - 9 & 4 - 3 \\
9 - 7 & 7 - 1 & 5 - 5 \\
\end{Bmatrix}=
\begin{Bmatrix}
1 & -6 & 1 \\
2 & 6 & 0 \\
\end{Bmatrix}$$

### Multiplication and Division of a matrix by a Scalar
Multiplication and division of a matrix by a [[Vectors and Scalar|scalar]] is as easy as multiplying multiple numbers by a single term. You take each number in the matrix and multiply it by the number outside the matrix. 

$$n \times \begin{Bmatrix}
a & b & c \\
d & e & f \\
\end{Bmatrix} = \begin{Bmatrix}
na & nb & nc \\
nd & ne & nf \\
\end{Bmatrix}
$$

> [!example]+ 💡 Example of multiplication of matrices by a scalar
> 
> $$ 7 \times \begin{Bmatrix}
1 & 3 & 5 \\
9 & 4 & 2 \\
\end{Bmatrix} = \begin{Bmatrix}
(7)1 & (7)3 & (7)5 \\
(7)9 & (7)4 & (7)2 \\
\end{Bmatrix} = \begin{Bmatrix}
7 & 21 & 35 \\
63 & 28 & 14 \\
\end{Bmatrix}$$

> [!example]+ 💡 Example of Division of matrices by a scalar
> 
> $$7 \div \begin{Bmatrix}
1 & 3 & 5 \\
9 & 4 & 2 \\
\end{Bmatrix} = \begin{Bmatrix}
\frac{7}{1} & \frac{7}{3} & \frac{7}{5} \\
\frac{7}{9} & \frac{7}{4} & \frac{7}{2} \\
\end{Bmatrix}$$

> [!note]
> You can simplify the fraction, but it is often acceptable to leave it as surds. 

### Multiplication of Matrices 
When multiplying matrices, we multiply the members of the rows by the members of the other matrix’s columns.. This means that one matrix must have the same amount of rows as the other matrix has columns, otherwise multiplication of matrices is not possible. Multiplying matrices also gives us a *dot product*, in which the vector value of multiple members is turned into a single scalar value through multiplication of two members. See [Dot Product](https://www.mathsisfun.com/algebra/vectors-dot-product.html) for more information on dot products. 

$$\begin{Bmatrix}
a & b & c \\
d & e & f \\
\end{Bmatrix} \times \begin{Bmatrix}
g & h \\
i & j \\
k & l \\
\end{Bmatrix} = \begin{Bmatrix}
ag + bi + ck & ah + bj + cl\\
dg + ei + fk & dh + ej + fl\\
\end{Bmatrix}
$$

> [!example]+ 💡 Example of A matrix multiplied by another matrix
> 
> $$\begin{Bmatrix}
1 & 3 & 4 \\
2 & 7 & 5 \\
\end{Bmatrix} \times \begin{Bmatrix}
4 & 6  \\
7 & 4  \\
8 & 2  \\
\end{Bmatrix} = \begin{Bmatrix}
1(4) + 3(7) + 4(8) & 1(6) + 3(4) + 4(2) \\
2(4) + 7(7) + 5(8) & 2(6) + 7(4) + 5(2) \\
\end{Bmatrix} = \begin{Bmatrix}
57 & 26 \\
97 & 50 \\
\end{Bmatrix}$$


> [!note] 📔 Division of a matrix
> 
> Division is the same as multiplication by the inverse of a number, the same goes for matrices. Division of a matrix is the same as multiplication by the [[#inverse of a matrix]]

> [!info] 📔 Identity of a Matrix
> As discussed earlier, the matrix below is the [[#Identity Matrix|multiplication identity of any matrix]], and we can test this through the [[#Multiplication of Matrices]]
> 
> $$\begin{Bmatrix}
a & b & c \\
d & e & f \\
\end{Bmatrix} \times \begin{Bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{Bmatrix} = \begin{Bmatrix}
a(1) + b(0) + c(0) & a(0) + b(1) + c(0) & a(0) + b(0) + c(1) \\
d(1) + e(0) + f(0) & d(0) + e(1) + f(0) & d(0) + e(0) + f(1) \\
\end{Bmatrix} = \begin{Bmatrix}
a & b & c \\
d & e & f \\
\end{Bmatrix}$$


## Determinant of a 2x2 Matrix
The determinant of a 2x2 matrix is as simple as swapping multiplying x<sub>1,1</sub> and x<sub>2,2</sub> and subtracting x<sub>1,2</sub>⋅x<sub>2,1</sub>

$$
\begin{gather}
\begin{Bmatrix}
a & b & \\
d & e & \\
\end{Bmatrix}
\\ \textrm{Determinant} = a \times e - b \times d
\end{gather}
$$

## Inverse of 2x2 Matrices
Inverse matrices rely on the concept of *multiplicative inverses*, where:
$$ a \times b = 1 $$
This can be simplified to: 
$$ a \times a^{-1} = 1$$
1 is the multiplication identity for linear factors. Which we can apply to matrices, using the [[#Identity Matrix]]
$$ 
\begin{gather}
\\& \mathbf{x} = 
\begin{Bmatrix}
a & b \\
d & e \\
\end{Bmatrix}
\\& \mathbf{x} \times \mathbf{x}^{-1} = \begin{Bmatrix}
1 & 0  \\
0 & 1 \\
\end{Bmatrix}
\end{gather}
$$

To find the values contained by the inverse matrix, we must first find the [[#Determinant of a 2x2 Matrix|Determinant of the Matrix]].

$$
\begin{gather}
\begin{Bmatrix}
a & b \\
c & d \\
\end{Bmatrix}
\\ \textrm{Determinant} = a \times d - b \times c
\end{gather}
$$

Then we can swap the two values in the leading diagonal of the matrix, and change the signs of the other values (in this case I’m not sure why, I’m assuming ill learn it later but ill put a todo here)

%%TODO: figure out why the fuck we do it like this %%

$$ \begin{gather}
\textrm{let: } a \times d - b \times c = k
\\\mathbf{x}^{-1} =  k^{-1} \times \begin{Bmatrix}
d & -b \\
-c & a \\
\end{Bmatrix} = \begin{Bmatrix}
k^{-1}d & k^{-1}(-b) \\
k^{-1}(-c) & k^{-1}a  \\
\end{Bmatrix}
\end{gather} $$

So to summarize the method of finding an inverse:
1. Equate the matrix and its inverse to the identity matrix
2. Find the determinant of the matrix
3. Swap the x<sub>1,1</sub> and x<sub>2,2</sub> values
4. Swap the signs of the x<sub>1,2</sub> and x<sub>2,1</sub> values
5. Multiply the swapped matrix with the inverse of the determinant to find the inverse of the matrix. 

> [!example]+ 💡 Example
> 
> $$ 
\begin{gather}
\\\textrm{Initial Equation: }& \mathbf{x} = 
\begin{Bmatrix}
1 & 3 \\
7 & 4 \\
\end{Bmatrix}
\\& \mathbf{x} \times \mathbf{x}^{-1} = \begin{Bmatrix}
1 & 0  \\
0 & 1 \\
\end{Bmatrix}
\\ \textrm{Determinant} & 1 \times 4 - 7 \times 3 = -17
\\ \textrm{Swapped Matrix} & \begin{Bmatrix}
4 & -3 \\
-7 & 1 \\
\end{Bmatrix}
\\\textrm{inverse} & x^{-1} = -17^{-1} \begin{Bmatrix}
4 & -3 \\
-7 & 1 \\
\end{Bmatrix} = \begin{Bmatrix}
\frac{4}{-17} & \frac{-3}{-17} \\
\frac{-7}{-17} & \frac{1}{-17} \\
\end{Bmatrix}
\end{gather}$$

## Solving Equations With Matrices
To solve for a variable in a matrix, you must simplify the two matrices into a single matrix with all equations contained within, and the answer those matrices must correct to. From there you can break up the matrices and solve for each variable

> [!example]+ 💡 Example of solving an addition equation with matrices. 
> 
> $$ \begin{gather}
\begin{Bmatrix}
a & 2  \\
-1 & 4  \\
\end{Bmatrix} - 2 \begin{Bmatrix}
2 & -1  \\
-2 & b  \\
\end{Bmatrix} = \begin{Bmatrix}
-7 & 4 \\
3 & 4a \\
\end{Bmatrix} 
\\ \begin{Bmatrix}
a - 4 = -7 & 2 - (-2) = 4 \\
-1 - (-4) = 3 & 4 + 2b = 4a \\
\end{Bmatrix}
\\ \textrm{Finding } a: a - 4 = -7 \therefore a = -3 \\ \textrm{Finding } b: 4 - 2b = 4a \therefore b = +6 + 2 = 8 
\end{gather} $$

### Simultaneous Equations as Matrices
If given two simultaneous equations, you can turn them into matrices by equating the constant terms to the coefficients multiplied by the variables. 

$$
\begin{gather}
ax + by = c & dx + ey = f
\\ \begin{Bmatrix}
a & b \\
d & e \\
\end{Bmatrix} \times \begin{Bmatrix}
x \\
y \\
\end{Bmatrix} = \begin{Bmatrix}
c \\
f \\
\end{Bmatrix}
\end{gather}$$

> [!example]+ 💡 Example
> 
> $$\\\begin{gather}
3x + -2y = 1 \\ -x + 4y = 3
\\ \begin{Bmatrix}
3 & -2 \\
-1 & 4 \\
\end{Bmatrix} \times \begin{Bmatrix}
x \\
y \\
\end{Bmatrix} = \begin{Bmatrix}
1 \\
3 \\
\end{Bmatrix}
\\ invert the Coefficient matrix: 
\end{gather}$$