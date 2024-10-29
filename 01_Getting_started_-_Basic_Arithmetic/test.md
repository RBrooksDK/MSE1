---
layout: default
---

### Exercise 1: Recap

You are given the augmented matrix 

$$ A =
\begin{bmatrix}
    1 &  -2 &  0 &  -1 & 1\\
    -4 &  8 &  2 &  4 & -8\\
    -2 &  4 &  0 &  1 &  -2
\end{bmatrix}
$$
​

(a) What is the size of the matrix?

<details>

<br>
<summary> </summary>

$3\times5$

</details>

<br>



(b) Reduce the matrix to echelon form (either by hand or by doing seperate row operations in Python)

<details>

<br>
<summary> </summary>

Note. There are many ways to reduce the matrix to echelon form. Here is one way to do it.

$$  
\begin{bmatrix}
    1 & -2 & 0 & -1 & 1\\
    0 & 0 & 2 & 0 & -4\\
    0 & 0 & 0 & -1 & 0
\end{bmatrix}
$$

</details>

<br>

(c) Use the echelon form to find the basic variables and free variables
<details>

<br>
<summary> </summary>

The basic variables are $x_1$, $x_3$ and $x_4$ and the free variable is $x_2$

</details>

<br>

(d) Find the general solution to the system and write the basic variables in terms of the free variables

<details>

<br>
<summary> </summary>

Express $x_1, x_3$, and $x_4$ in terms of the free variable $x_2$ :
1. From Row 1: $x_1-2 x_2=1 \Rightarrow x_1=2 x_2+1$
2. From Row 2: $x_3=-2$
3. From Row 3: $x_4=0$
</details>

<br>


(e) Mark each of the following statements as TRUE or FALSE

(i)  The matrix A describes a system of five equations and three variables  
(ii)  The matrix A describes a consistent system of equations  
(iii)  A 3x5 augmented matrix can not have a unique solution  
(iv)  A 3x5 augmented matrix will always be consistent  

<details>

<br>
<summary> </summary>

(i)  The matrix A describes a system of five equations and three variables FALSE  
(ii)  The matrix A describes a consistent system of equations TRUE  
(iii)  A 3x5 augmented matrix can not have a unique solution TRUE  
(iv)  A 3x5 augmented matrix will always be consistent FALSE  

</details>

<br>


### Exercise 2: Matrix and vector equations
For each of the following systems of linear equations write it as (i) an augmented matrix (ii) a vector equation and (iii) a matrix equation.


(a) 
$$\begin{cases}
    2x_1 +3x_2 - 4x_3 =8\\
    -x_2 +x_3 + 2x_4 = -2\\
    -x_1 + 2x_4 = 3
\end{cases}$$

<details>

<br>
<summary> </summary>


(i) Augmented matrix:
$$
\begin{bmatrix}
     2 & 3 & -4 & 0 &  8\\
     0 & -1&  1 & 2 & -2\\
     -1& 0 & 0 & 2 & 3 
\end{bmatrix}
$$

(ii) Vector equation:

$$
x_1\begin{bmatrix}2\\\ 0\\\ -1\end{bmatrix} + x_2\begin{bmatrix}3\\\ -1\\\ 0\end{bmatrix}+ x_3\begin{bmatrix}-4\\\ 1\\\ 0\end{bmatrix}+ x_4\begin{bmatrix}0\\\ 2\\\ 2\end{bmatrix}=\begin{bmatrix}8\\\ -2\\\ 3\end{bmatrix}
$$

(iii) Matrix equation:
$$
\begin{bmatrix}
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
\end{bmatrix}
$$

</details>

<br>

(b)
$$\begin{cases}
    x_1 + x_2 = 2\\
    x_1 -x_2 = 4
\end{cases}$$

<details>

<br>
<summary> </summary>

(i) Augmented matrix:
$$
\begin{bmatrix}
     1 & 1 & 2\\
     1 & -1& 4
\end{bmatrix}
$$

(ii) Vector equation:
$$
x_1\begin{bmatrix}1\\1\end{bmatrix}+ x_2\begin{bmatrix}1\\-1\end{bmatrix}=\begin{bmatrix}2\\4\end{bmatrix}
$$

(iii) Matrix equation:
$$
\begin{bmatrix}
     1 & 1 \\
     1 & -1
\end{bmatrix}
\begin{bmatrix}
     x_1\\x_2
\end{bmatrix}
=
\begin{bmatrix}
     4\\2
\end{bmatrix}
$$

</details>

<br>

(c)
$$\begin{cases}
    x_1 = 4\\
    x_2 = -1\\
    x_3 = 10
\end{cases}$$

<details>

<br>
<summary> </summary>

(i) Augmented matrix:
$$
\begin{bmatrix}
     1 & 0 & 0 & 4\\
     0 & 1 & 0 & -1\\
     0 & 0 & 1 & 10
\end{bmatrix}
$$

(ii) Vector equation:
$$
x_1\begin{bmatrix}1\\0\\0\end{bmatrix}+ x_2\begin{bmatrix}0\\1\\0\end{bmatrix}+x_3\begin{bmatrix}0\\0\\1\end{bmatrix}=\begin{bmatrix}4\\-1\\10\end{bmatrix}
$$

(iii) Matrix equation:
$$
\begin{bmatrix}
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
\end{bmatrix}
$$

</details>

<br>


### Exercise 3: Linear combinations
Let

$\mathbf{v}_1=\begin{bmatrix}1\\\ -2\\\4\end{bmatrix}$, $\mathbf{v}_2=\begin{bmatrix}3\\\0\\\2\end{bmatrix}$ and $\mathbf{v}_3=\begin{bmatrix}-1\\\5\\\1\end{bmatrix}$.

Calculate the linear combinations below.

(a) $2\mathbf{v}_1+3\mathbf{v}_2+\mathbf{v}_3$


<details>

<br>
<summary> </summary>

$\begin{bmatrix}10\\\1\\\15\end{bmatrix}$

</details>

<br>


(b) $\mathbf{v}_1-\mathbf{v}_3$

<details>

<br>
<summary> </summary>

$\begin{bmatrix}2\\\ -7\\\3\end{bmatrix}$

</details>

<br>

(c) $\frac{1}{2}\mathbf{v}_1+\frac{3}{2}\mathbf{v}_2+\mathbf{v}_3$

<details>

<br>
<summary> </summary>

$\begin{bmatrix}4\\\4\\\6\end{bmatrix}$

</details>

<br>

(d) Find the solution to the linear system described by the augmented matrix

$
\begin{bmatrix}
     1 & 3 & -1 & 10\\\
     -2 & 0 & 5 & 1\\\
     4 & 2 & 1 & 15
\end{bmatrix}
$


<details>

<br>
<summary> </summary>

$\begin{cases}
x_1 = 2\\\
x_2 = 3\\\
x_3 = 1
\end{cases}$

</details>

<br>


### Exercise 4: Parametric vector form
In the following exercises, the solution to a set of linear equations has already been found. Your job
is to write the solution on parametric vector form.

(a) A system has been found to have the solution

$
\begin{aligned}
x_1 &= 4 - x_2 \\\\
x_2 &= x_2 \\\\
x_3 &= -1 + 3x_2
\end{aligned}
$

where $x_2$ is a free variable. Write the solution in parametric vector form.

<details>

<br>
<summary> </summary>

$
\left[\begin{array}{l}
x_1 \\\
x_2 \\\
x_3
\end{array}\right]=\left[\begin{array}{c}
4 \\\
0 \\\
-1
\end{array}\right]+x_2\left[\begin{array}{c}
-1 \\\
1 \\\
3
\end{array}\right]
$

</details>

<br>

(b) A system of equations has been found to have the solution

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

<details>

<br>
<summary> </summary>

$$
\left[\begin{array}{l}
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
\end{array}\right]
$$

</details>

<br>


### Exercise 5: Homogenous equation
Solve the homogenous equation $A\mathbf{x}=\mathbf{0}$ for the following matrices. Write the solution in parametric vector form.

(a)
$$
\begin{bmatrix}
    4 & -8\\
    -3 & 6
\end{bmatrix}
$$

<details>

<br>
<summary> </summary>

$\mathbf{x}=x_2\left[\begin{array}{l}2 \\\ 1\end{array}\right]$

</details>
<br>

(b)
$
\begin{bmatrix}
    4 & -9 & 1 \\\
    2 & -5 & 1 \\\
    -3 & 1 & 5
\end{bmatrix}
$

<details>

<br>
<summary> </summary>

$\mathbf{x}=x_3\left[\begin{array}{l}2 \\\ 1 \\\ 1\end{array}\right]$

</details>
<br>

(c)
$
\begin{bmatrix}
2 & -10 & 6 \\\
1 & -5 & 3
\end{bmatrix}
$

<details>

<br>
<summary> </summary>

$\mathbf{x}=x_2\left[\begin{array}{l}5 \\\ 1 \\\ 0\end{array}\right]+x_3\left[\begin{array}{c}-3 \\\ 0 \\\ 1\end{array}\right]$

</details>
<br>

(d) For the exercises (a)-(c) give a geometric interpretation of the solution set.

<details>

<br>
<summary> </summary>

(a) The solution set is a line in $\mathbb{R}^2$, as it has one free variable, representing a one-dimensional subspace.  
(b) The solution set is a line in $\mathbb{R}^3$, as it has one free variable, representing a one-dimensional subspace.  
(c) The solution set is a plane in $\mathbb{R}^3$, as it has two free variables, representing a two-dimensional subspace.

</details>
<br>


### Exercise 6: Linear Independence

a. For $$\mathbf{a}_1 = 
        \begin{bmatrix}
            2 \\\
            3 \\\
            0
        \end{bmatrix}$$,
    $$\mathbf{a}_2 = 
        \begin{bmatrix}
            1\\\
            2\\\
            -5
        \end{bmatrix}$$,
    $$\mathbf{a}_3 = 
        \begin{bmatrix}
            4\\\
            1\\\
            2
        \end{bmatrix}$$, and
    $$\mathbf{b} = 
        \begin{bmatrix}
            8\\\
            6\\\
            12
        \end{bmatrix}$$ 
determine if $\mathbf{b}$ is a linear combination of $\mathbf{a}_1,\mathbf{a}_2$ and $\mathbf{a}_3$.

<details>

<br>
<summary> </summary>

Yes, since $\mathbf{b}=3\mathbf{a}_1-2\mathbf{a}_2+\mathbf{a}_3$

</details>

<br>

b.
Let $$A = \begin{bmatrix}1  & -2 & 4 \\
                        0  & 4  & -5 \\
                        -3 & 6  & -12 \end{bmatrix}$$ and
    $\mathbf{b}=\begin{bmatrix}1 \\\ -4 \\\ -1\end{bmatrix}$ be given.
     Determine whether $\mathbf{b}$ is a linear combination of the columns in $A$.

<details>

<br>
<summary> </summary>

No $\mathbf{b}$ is not a linear combination of the columns of $A$

</details>

<br>

c. For $$A = \begin{bmatrix}2  & -6 & 5 \\\
                        1  & -5  & 1 \\\
                        -2 & 6  & p \end{bmatrix}$$ and
        $\mathbf{b}= \begin{bmatrix}3 \\\ 0 \\\ q\end{bmatrix}$ 
    determine the values of $p$ and $q$ such that $\mathbf{b}$ is a not a linear combination of the columns of $A$.
    
<details>

<br>
<summary> </summary>

$p=-5$ and $q\neq-3$

</details>

<br>