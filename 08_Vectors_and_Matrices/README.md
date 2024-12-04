# 8. Vectors and Matrices

### Session Preparation

Brooks: [Chapter 8](https://drive.google.com/file/d/1P9eidJb5qtlZgvHCtqu4uuPa5FFU0Zpn/view?usp=sharing). You should begin reading before class as it will aid your understanding as the topics get more complex.

### Session Material

[Session notes](https://drive.google.com/file/d/1FCAtAWjoSxS66AdYO0L3W7tjd4ZHPaxJ/view?usp=sharing)

[Session Resources](https://viaucdk-my.sharepoint.com/:f:/g/personal/rib_viauc_dk/Ep-kuPOC2r5NsJOp-SzZ1U8BsPWE1ZL0SEZTvJ8NXxrsHQ?e=SrV1vE)

--------------------------

### Topic Description
Today, we will explore the fundamental concepts that form the backbone of linear algebra. We'll start with **vectors**, understanding how these entities with magnitude and direction are essential for representing data and physical quantities in multiple dimensions.

Next, we'll delve into **vector equations** to see how relationships between vectors are expressed and solved. This will naturally lead us to **matrix equations**, where we'll discover powerful methods for handling multiple equations and unknowns simultaneously.

We'll examine the **solution set of a linear system**, exploring scenarios with unique solutions, infinitely many solutions, or no solution at all. By connecting algebraic methods to geometric interpretations, we'll visualize how lines and planes intersect in space.

To better understand complex solution sets, we'll introduce the **parametric vector form**, which uses parameters to describe all possible solutions of a system clearly. Finally, we'll tackle **linear independence and dependence**, learning how these concepts determine the minimal set of vectors needed to span a space.

By the end of the session, we'll have built a strong foundation in these core concepts, preparing us for more advanced topics in linear algebra.

#### Key Concepts
- Vectors
- Vector Equations
- Matrix Equations
- Solution Set of a Linear System
- Parametric Vector Form
- Linear Independence and Dependence

--------------------------

### Exercises for recitation

#### Exercise 1: Recap

You are given the augmented matrix

$A =\begin{bmatrix}
    1 &  -2 &  0 &  -1 & 1\\
    -4 &  8 &  2 &  4 & -8\\
    -2 &  4 &  0 &  1 &  -2
\end{bmatrix}$
​

a. What is the size of the matrix? (1)
{ .annotate }

1. $3\times5$

b. Reduce the matrix to echelon form (either by hand or by doing seperate row operations in Python)

??? answer "&nbsp;"

    Note. There are many ways to reduce the matrix to echelon form. Here is one way to do it.

    $\begin{bmatrix}
        1 &  -2 &  0 &  -1 & 1 \\\
        0 &  0 &  2 &  0 & -4 \\\
        0 &  0 &  0 &  -1 &  0
    \end{bmatrix}$

c. Use the echelon form to find the basic variables and free variables

??? answer "&nbsp;"

    The basic variables are $x_1$, $x_3$ and $x_4$ and the free variable is $x_2$

d. Find the general solution to the system and write the basic variables in terms of the free variables

??? answer "&nbsp;"
    Express $x_1, x_3$, and $x_4$ in terms of the free variable $x_2$ :
    1. From Row 1: $x_1-2 x_2=1 \Rightarrow x_1=2 x_2+1$
    2. From Row 2: $x_3=-2$
    3. From Row 3: $x_4=0$

e. Mark each of the following statements as TRUE or FALSE

(i)  The matrix A describes a system of five equations and three variables (1)
{ .annotate }

1. FALSE

(ii)  The matrix A describes a consistent system of equations (1)
{ .annotate }

1. TRUE

(iii)  A 3x5 augmented matrix can not have a unique solution (1)
{ .annotate }

1. TRUE
(iv)  A 3x5 augmented matrix will always be consistent (1)
{ .annotate }

1. FALSE

#### Exercise 2: Matrix and vector equations
For each of the following systems of linear equations write it as (i) an augmented matrix (ii) a vector equation and (iii) a matrix equation.

a. $\begin{cases}
    2x_1 +3x_2 - 4x_3 =8\\
    -x_2 +x_3 + 2x_4 = -2\\
    -x_1 + 2x_4 = 3
\end{cases}$

??? answer "&nbsp;"

    (i) Augmented matrix:
    $\begin{bmatrix}
        2 & 3 & -4 & 0 &  8\\
        0 & -1&  1 & 2 & -2\\
        -1& 0 & 0 & 2 & 3 
    \end{bmatrix}$

    (ii) Vector equation:
    $x_1\begin{bmatrix}2\\\ 0\\\ -1\end{bmatrix} + x_2\begin{bmatrix}3\\\ -1\\\ 0\end{bmatrix}+ x_3\begin{bmatrix}-4\\\ 1\\\ 0\end{bmatrix}+ x_4\begin{bmatrix}0\\\ 2\\\ 2\end{bmatrix}=\begin{bmatrix}8\\\ -2\\\ 3\end{bmatrix}$

    (iii) Matrix equation:
    $\begin{bmatrix}
        2 & 3 & -4 & 0 \\
        0 & -1&  1 & 2 \\
        -1& 0 & 0 & 2 
    \end{bmatrix}
    \begin{bmatrix}
        x_1\\x_2\\x_3\\x_4
    \end{bmatrix}
    =
    \begin{bmatrix}
        8\\-2\\3
    \end{bmatrix}$

b. $\begin{cases}
    x_1 + x_2 = 2\\
    x_1 -x_2 = 4
\end{cases}$

??? answer "&nbsp;"

    (i) Augmented matrix:
    $\begin{bmatrix}
        1 & 1 & 2\\
        1 & -1& 4
    \end{bmatrix}$

    (ii) Vector equation:
    $x_1\begin{bmatrix}1\\1\end{bmatrix}+ x_2\begin{bmatrix}1\\-1\end{bmatrix}=\begin{bmatrix}2\\4\end{bmatrix}$

    (iii) Matrix equation:
    $\begin{bmatrix}
        1 & 1 \\
        1 & -1
    \end{bmatrix}
    \begin{bmatrix}
        x_1\\x_2
    \end{bmatrix}
    =
    \begin{bmatrix}
        2\\4
    \end{bmatrix}$


c.$\begin{cases}
    x_1 = 4\\
    x_2 = -1\\
    x_3 = 10
\end{cases}$

??? answer "&nbsp;"

    (i) Augmented matrix:
    $\begin{bmatrix}
        1 & 0 & 0 & 4\\
        0 & 1 & 0 & -1\\
        0 & 0 & 1 & 10
    \end{bmatrix}$

    (ii) Vector equation:
    $x_1\begin{bmatrix}1\\0\\0\end{bmatrix}+ x_2\begin{bmatrix}0\\1\\0\end{bmatrix}+x_3\begin{bmatrix}0\\0\\1\end{bmatrix}=\begin{bmatrix}4\\-1\\10\end{bmatrix}$

    (iii) Matrix equation:
    $\begin{bmatrix}
        1 & 0 & 0 \\
        0 & 1 & 0\\
        0 & 0 & 1
    \end{bmatrix}
    \begin{bmatrix}
        x_1\\x_2\\x_3
    \end{bmatrix}
    =
    \begin{bmatrix}
        4\\-1\\10
    \end{bmatrix}$

#### Exercise 3: Linear combinations
Let

$\mathbf{v}_1=\begin{bmatrix}1\\ -2\\ 4\end{bmatrix}$, $\mathbf{v}_2=\begin{bmatrix}3\\ 0\\ 2\end{bmatrix}$ and $\mathbf{v}_3=\begin{bmatrix}-1\\ 5\\ 1\end{bmatrix}$.

Calculate the linear combinations below.

a. $2\mathbf{v}_1+3\mathbf{v}_2+\mathbf{v}_3$


??? answer "&nbsp;"

    $\begin{bmatrix}10\\1\\15\end{bmatrix}$

b. $\mathbf{v}_1-\mathbf{v}_3$

??? answer "&nbsp;"

    $\begin{bmatrix}2\\-7\\3\end{bmatrix}$

c. $\frac{1}{2}\mathbf{v}_1+\frac{3}{2}\mathbf{v}_2+\mathbf{v}_3$

??? answer "&nbsp;"

    $\begin{bmatrix}4\\4\\6\end{bmatrix}$

d. Find the solution to the linear system described by the augmented matrix

\[
\begin{bmatrix}
     1 & 3 & -1 & 10 \\
     -2 & 0 & 5 & 1 \\
     4 & 2 & 1 & 15
\end{bmatrix}
\]

??? answer "&nbsp;"

    $\begin{cases}
    x_1 = 2\\
    x_2 = 3\\
    x_3 = 1
    \end{cases}$


#### Exercise 4: Parametric vector form
In the following exercises, the solution to a set of linear equations has already been found. Your job
is to write the solution on parametric vector form.

a. A system has been found to have the solution

$$
\begin{aligned}
x_1 &= 4 - x_2 \\\
x_2 &= x_2 \\\
x_3 &= -1 + 3x_2
\end{aligned}
$$

where $x_2$ is a free variable. Write the solution in parametric vector form.

??? answer "&nbsp;"
    $\left[\begin{array}{l}
    x_1 \\
    x_2 \\
    x_3
    \end{array}\right]=\left[\begin{array}{c}
    4 \\
    0 \\
    -1
    \end{array}\right]+x_2\left[\begin{array}{c}
    -1 \\
    1 \\
    3
    \end{array}\right]$

b. A system of equations has been found to have the solution

$$
\begin{aligned}
x_1 &= 5 + 4x_4 \\
x_2 &= 2 \\
x_3 &= x_3 \\
x_4 &= x_4 \\
x_5 &= -8 + x_3 - 7x_4
\end{aligned}
$$

where $x_3$ and $x_4$ are free variables. Write the solution in parametric vector form.

??? answer "&nbsp;"
    $\left[\begin{array}{l}
    x_1 \\
    x_2 \\
    x_3 \\
    x_4 \\
    x_5
    \end{array}\right]=\left[\begin{array}{c}
    5 \\
    2 \\
    0 \\
    0 \\
    -8
    \end{array}\right]+x_3\left[\begin{array}{l}
    0 \\
    0 \\
    1 \\
    0 \\
    1
    \end{array}\right]+x_4\left[\begin{array}{c}
    4 \\
    0 \\
    0 \\
    1 \\
    -7
    \end{array}\right]$


#### Exercise 5: Homogenous equation
Solve the homogenous equation $A\mathbf{x}=\mathbf{0}$ for the following matrices. Write the solution in parametric vector form.

a. $\begin{bmatrix}
    4 & -8\\
    -3 & 6\end{bmatrix}$

??? answer "&nbsp;"
    $\mathbf{x}=x_2\left[\begin{array}{l}2 \\ 1\end{array}\right]$

b. $\begin{bmatrix}
    4 & -9 & 1 \\\
    2 & -5 & 1 \\\
    -3 & 1 & 5 \end{bmatrix}$

??? answer "&nbsp;"
    $\mathbf{x}=x_3\left[\begin{array}{l}2 \\ 1 \\ 1\end{array}\right]$

c.$\begin{bmatrix}
2 & -10 & 6 \\\
1 & -5 & 3
\end{bmatrix}$

??? answer "&nbsp;"
    $\mathbf{x}=x_2\left[\begin{array}{l}5 \\ 1 \\ 0\end{array}\right]+x_3\left[\begin{array}{c}-3 \\ 0 \\ 1\end{array}\right]$

$\mathbf{x}=x_2\left[\begin{array}{l}5 \\\ 1 \\\ 0\end{array}\right]+x_3\left[\begin{array}{c}-3 \\\ 0 \\\ 1\end{array}\right]$

d. For the exercises (a)-(c) give a geometric interpretation of the solution set.

??? answer "&nbsp;"
    (a) The solution set is a line in $\mathbb{R}^2$, as it has one free variable, representing a one-dimensional subspace.  
    (b) The solution set is a line in $\mathbb{R}^3$, as it has one free variable, representing a one-dimensional subspace.  
    (c) The solution set is a plane in $\mathbb{R}^3$, as it has two free variables, representing a two-dimensional subspace.

#### Exercise 6: Linear Independence

a. For $\mathbf{a}_1 = 
        \begin{bmatrix}
            2 \\\
            3 \\\
            0
        \end{bmatrix}$,
    $\mathbf{a}_2 = 
        \begin{bmatrix}
            1\\\
            2\\\
            -5
        \end{bmatrix}$,
    $\mathbf{a}_3 = 
        \begin{bmatrix}
            4\\\
            1\\\
            2
        \end{bmatrix}$, and
    $\mathbf{b} = 
        \begin{bmatrix}
            8\\\
            6\\\
            12
        \end{bmatrix}$ 
determine if $\mathbf{b}$ is a linear combination of $\mathbf{a}_1,\mathbf{a}_2$ and $\mathbf{a}_3$.

??? answer "&nbsp;"
    Yes, since $\mathbf{b}=3\mathbf{a}_1-2\mathbf{a}_2+\mathbf{a}_3$

b.
Let $A = \begin{bmatrix}1  & -2 & 4 \\
                        0  & 4  & -5 \\
                        -3 & 6  & -12 \end{bmatrix}$ and
    $\mathbf{b}=\begin{bmatrix}1 \\\ -4 \\\ -1\end{bmatrix}$ be given.
     Determine whether $\mathbf{b}$ is a linear combination of the columns in $A$.

??? answer "&nbsp;"

    No $\mathbf{b}$ is not a linear combination of the columns of $A$

c. For $A = \begin{bmatrix}2  & -6 & 5 \\\
                        1  & -5  & 1 \\\
                        -2 & 6  & p \end{bmatrix}$ and
        $\mathbf{b}= \begin{bmatrix}3 \\\ 0 \\\ q\end{bmatrix}$ 
    determine the values of $p$ and $q$ such that $\mathbf{b}$ is not a linear combination of the columns of $A$.

??? answer "&nbsp;"
    $p=-5$ and $q\neq-3$