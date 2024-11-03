# 9. Matrix Algebra and Determinants

### Session Preparation

Brooks: [Chapter 9](https://drive.google.com/file/d/1P9eidJb5qtlZgvHCtqu4uuPa5FFU0Zpn/view?usp=sharing). You should begin reading before class as it will aid your understanding as the topics get more complex.

### Session Material

[Session notes]()

[Session Resources](https://viaucdk-my.sharepoint.com/:f:/g/personal/rib_viauc_dk/EpGNNUp8hjpPn6niIxD8hT4BdSOLqNwtdY91GTRCdj7D_g?e=2DwW6Q)

--------------------------

In this session, we will delve into the foundational aspects of matrix algebra. We begin with the definitions and properties of various types of matrices, including diagonal, zero, and identity matrices. We will learn how to perform basic matrix operations such as scalar multiplication and matrix addition, and how to compute matrix multiplication using both the definition and the row-column rule. The session will also cover the concepts of powers and the transpose of a matrix. We will explore several important theorems that describe the properties of matrix operations, including the definition and properties of invertible matrices. We will learn how to compute the inverse of a matrix and understand the significance of The Invertible Matrix Theorem. Finally, we will introduce determinants for 2 x 2 matrices and provide a brief overview of eigenvalues and eigenvectors.

### Key Concepts
- Definitions of Diagonal Matrices, Zero Matrices, and Identity Matrices
- Scalar Multiplication and Matrix Addition
- Computing Matrix Multiplication (by Definition and Row-Column Rule)
- Definitions of Powers and Transpose of a Matrix
- Theorems on the Properties of Matrix Operations
- Definition of Invertible Matrix
- Additional Theorems on Invertibility 
- Computing the Inverse of a Matrix
- Determinants for 2 x 2 Matrices
--------------------------

### Exercises for recitation

[P] Means that you are advised to use Python to solve the exercise.

#### Exercise 1
a. Find the value of $h$ for which the vectors are linearly dependent. (1)
{ .annotate }

1. $$h = -4$$

$$
\left[\begin{array}{r}
2 \\
-2 \\
4
\end{array}\right],\left[\begin{array}{r}
4 \\
-6 \\
7
\end{array}\right],\left[\begin{array}{r}
-2 \\
2 \\
h
\end{array}\right]
$$

??? answer "&nbsp;"
    $h = -4$

b. Determine *by inspection* whether the following sets of vectors are linearly independent or dependent. Justify each answer.
{ .annotate }

i. $\left[\begin{array}{l}5 \\ 1\end{array}\right],\left[\begin{array}{l}2 \\ 8\end{array}\right],\left[\begin{array}{l}1 \\ 3\end{array}\right],\left[\begin{array}{r}-1 \\ 7\end{array}\right]$ (1)
{ .annotate }

1. Dependent

ii. $\left[\begin{array}{r}2 \\ -4 \\ 8\end{array}\right],\left[\begin{array}{r}-3 \\ 6 \\ -12\end{array}\right]$  (1)
{ .annotate }

1. Dependent

iii. $\left[\begin{array}{r}5 \\ -3 \\ -1\end{array}\right],\left[\begin{array}{l}0 \\ 0 \\ 0\end{array}\right],\left[\begin{array}{r}-7 \\ 2 \\ 4\end{array}\right]$  (1)
{ .annotate }

1. Dependent

iv. $\left[\begin{array}{l}3 \\ 4\end{array}\right],\left[\begin{array}{r}-1 \\ 5\end{array}\right],\left[\begin{array}{l}3 \\ 5\end{array}\right],\left[\begin{array}{l}7 \\ 1\end{array}\right]$  (1)
{ .annotate }

1. Dependent

v. $\left[\begin{array}{r}-8 \\ 12 \\ -4\end{array}\right],\left[\begin{array}{r}2 \\ -3 \\ -1\end{array}\right]$  (1)
{ .annotate }

1. Independent

vi. $\left[\begin{array}{r}1 \\ 4 \\ -7\end{array}\right],\left[\begin{array}{r}-2 \\ 5 \\ 3\end{array}\right],\left[\begin{array}{l}0 \\ 0 \\ 0\end{array}\right]$  (1)
{ .annotate }

1. Dependent

??? answer "&nbsp;"

    i. Linearly dependent

    ii. Linearly dependent

    iii. Linearly dependent

    iv. Linearly dependent

    v. Linearly independent

    vi. Linearly dependent

c. [P] Use as many columns of $A$ as possible to construct a matrix $B$ with the property that the equation $B \mathbf{x}=\mathbf{0}$ has only the trivial solution. Solve $B \mathbf{x}=\mathbf{0}$ to verify your work. (1)
{ .annotate }

   1. When reduced to echelong form, you will have pivots in columns, 1, 2, and 4. Therefore, you   can  use columns 1, 2, and 4 to construct matrix B.

    You can verify your work by solving the equation $B \mathbf{x}=\mathbf{0} which is done by finding reduced echelon form of $B$. This will give you the trivial solution.


$$A = \left[\begin{array}{rrrrr}3 & -4 & 10 & 7 & -4 \\ -5 & -3 & -7 & -11 & 15 \\ 4 & 3 & 5 & 2 & 1 \\ 8 & -7 & 23 & 4 & 15\end{array}\right]$$

??? answer "&nbsp;"

    When reduced to echelong form, you will have pivots in columns, 1, 2, and 4. Therefore, you can use columns 1, 2, and 4 to construct matrix B.

    You can verify your work by solving the equation $B \mathbf{x}=\mathbf{0} which is done by finding reduced echelon form of $B$. This will give you the trivial solution.

2.1: 1, 2, 10, 13, 40, 41   
2.2: 9, 30, 31, 32   
​2.3: 11, 12, 15, 17  

#### Exercise 2

Compute each matrix sum or product if it is defined. If an expression is undefined, explain why. Let

$$
\begin{aligned}
& A=\left[\begin{array}{rrr}
2 & 0 & -1 \\
4 & -5 & 2
\end{array}\right], \quad B=\left[\begin{array}{rrr}
7 & -5 & 1 \\
1 & -4 & -3
\end{array}\right], \\
& C=\left[\begin{array}{rr}
1 & 2 \\
-2 & 1
\end{array}\right], \quad D=\left[\begin{array}{rr}
3 & 5 \\
-1 & 4
\end{array}\right], \quad E=\left[\begin{array}{r}
-5 \\
3
\end{array}\right]
\end{aligned}
$$

1. $-2 A, B-2 A, A C, C D$
2. $A+3 B, 2 C-3 E, D B, E C$
