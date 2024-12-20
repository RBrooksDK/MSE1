## Exercises: Linear Equations in Linear Algebra



### Exercise 1: Recap Conditional Probability
In a town of 20,000 people, a crime was committed. Evidence suggests that the perpetrator must be someone from the town. The police have found blood at the crime scene, and they are sure that this blood belongs to the perpetrator. The probability that a random innocent person matches the blood type of the evidence is 0.01. 

a. What is the probability that a random person from town is guilty?

<details>

<br>
<summary> </summary>

$\frac{1}{20000}=0.00005$

</details>

<br>

b. What is the probability that a random person from town is guilty given that the person matches the blood type of the evidence?

<details>

<br>
<summary> </summary>

$0.00498 = 0.498$%

</details>

<br>

From the blood sample it is possible to extract a DNA profile such that the probability that a random innocent person will match the DNA profile is 0.0001.

c. What is the probability that a random person from town is guilty given that the person matches the DNA-profile of the evidence?

<details>

<br>
<summary> </summary>

$0.333 = 33.3$%

</details>

<br>

### Exercise 2: Echelon and Reduced Echelon Form
Determine whether the following matrices are in reduced echelon form, echelon form, or neither.

a.
```math
\begin{bmatrix} 1 & 0 & 2 & 1\\ 
                0 & 1 & -3 & 0\end{bmatrix}
```

b.
```math
\begin{bmatrix} 1 & 2 & -2 & 5\\
                0 & 1 &  0 & -1\\
                0 & 0 &  1 & 3 \\ 
                0 & 0 &  0 & 1\end{bmatrix}
```

c.
```math
\begin{bmatrix} -1 & 0\\
                0 & 4\\
                0 & 0 \end{bmatrix}
```

d.
```math
\begin{bmatrix} 1 & 0 & 1 & 0 & -1\\
                0 & 1 & 1 & 0 & 0\\
                0 & 0 & 0 & 0 & 0\\
                0 & 0 & 0 & 1 & -1\end{bmatrix}
```

e.
```math
\begin{bmatrix} 0 & 3 & 0 & 4\\
                0 & 0 & -2 & -2\\
                0 & 0 & 0 & 7\end{bmatrix}
```

f.
```math
\begin{bmatrix} 1 & 0 & 0 & 1\\
                0 & 0 & 1 & -2\\
                0 & 0 & 0 & 1\end{bmatrix}
```

<details>

<br>
<summary> </summary>

a. reduced echelon form 

b. echelon form

c. echelon form

d. neither

e. echelon form

f. echelon form

</details>

<br>



### Exercise 3: Row operations
Explain which row operations are used in the calculations below.

a.
```math
\begin{bmatrix}
    4 & -3 & 1 & 2 \\
    3 & 1 & -5 & 6 \\
    1 & 1 & 2 & 4 \\
    \end{bmatrix}
    \sim
\begin{bmatrix}
    1 & 1 & 2 & 4 \\
    3 & 1 & -5 & 6 \\
    4 & -3 & 1 & 2 \\
    \end{bmatrix}
```

<details>
<br>
<summary></summary>

Swap: $r_1 \leftrightarrow r_3$

</details>
<br>

b.
```math
\begin{bmatrix}
    1 & 1 & 2 & 4 \\
    3 & 1 & -5 & 6 \\
    4 & -3 & 1 & 2 \\
    \end{bmatrix}
    \sim
    \begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & -2 & -11 & -6 \\
    4 & -3 & 1 & 2 \\
    \end{bmatrix}
```

<details>
<br>
<summary></summary>

Replacement: $r_2 \rightarrow r_2 - 3r_1$

</details>
<br>

c.
```math
\begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & -2 & -11 & -6 \\
    4 & -3 & 1 & 2 \\
    \end{bmatrix}
    \sim
    \begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & -2 & -11 & -6 \\
    0 & -7 & -7 & -14 \\
    \end{bmatrix}
```

<details>
<br>
<summary></summary>

Replacement: $r_3 \rightarrow r_3 - 4r_1$

</details>
<br>

d.
```math
\begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & -2 & -11 & -6 \\
    0 & -7 & -7 & -14 \\
    \end{bmatrix}
    \sim
    \begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & -2 & -11 & -6 \\
    0 & 1 & 1 & 2 \\
    \end{bmatrix}
```

<details>
<br>
<summary></summary>

Scaling: $r_3 \rightarrow -\frac{1}{7}r_3$

</details>
<br>

e.
```math
\begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & -2 & -11 & -6 \\
    0 & 1 & 1 & 2 \\
    \end{bmatrix}
    \sim
    \begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & 1 & 1 & 2 \\
    0 & -2 & -11 & -6 \\
    \end{bmatrix}
```

<details>
<br>
<summary></summary>

Swap: $r_2 \leftrightarrow r_3$

</details>
<br>

f.
```math
\begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & 1 & 1 & 2 \\
    0 & -2 & -11 & -6 \\
    \end{bmatrix}
    \sim
    \begin{bmatrix}
    1 & 1 & 2 & 4 \\
    0 & 1 & 1 & 2 \\
    0 & 0 & -9 & -2 \\
    \end{bmatrix}
```

<details>
<br>
<summary></summary>

Replacement: $r_3 \rightarrow r_3 + 2r_2$

</details>
<br>

g. The reduced matrix from (f)  is the augmented matrix for a system of linear equations. Does this system have no solution, a unique solution, or infinitely many solutions?

<details>
<br>
<summary></summary>

The system has a unique solution, since there is a pivot in each column of the coefficient part of the reduced matrix.

</details>
<br>

### Exercise 4: System of linear equations
Given the following system of linear equations:

$$
\begin{aligned}
2x_1 - 4x_2 + 6x_3 &= 2 \\
x_1 + x_3 &= 3 \\
-4x_1 + 2x_2 &= 2
\end{aligned}
$$

a. Write down the augmented matrix for the system.
<details>
<br>
<summary> </summary>

```math
\begin{bmatrix}
    2 & -4 & 6 & 2\\
    1 & 0  & 1 & 3\\
    -4& 2  & 0 & 2
\end{bmatrix}
```

</details>
<br>

b. Use row operations to get the reduced row echelon form of the matrix and write down the solution.

<details>
<br>
<summary></summary>

RREF:
```math	
\begin{bmatrix}  1 & 0 & 0 & 1\\
                        0 & 1 & 0 & 3\\
                        0 & 0 & 1 & 2
                        \end{bmatrix}
```
Solution:
```math
\begin{cases}
                x_1 = 1\\
                x_2 = 3\\
                x_3 = 2
\end{cases}
```

</details>
<br>

### Exercise 5: Row Reduction
Solve the systems whose augmented matrices are given below. Write down the general solution, i.e. write the basic variables in terms of the free variables. 

a.
```math	
\begin{bmatrix} 1 & 2 & 3 & 4\\
                    4 & 8 & 9 & 4\end{bmatrix}
```

<details>

<br>
<summary> </summary>

```math
\begin{cases}
x_1 = -8-2x_2\\
x_2 \text{ free}\\
x_3 = 4
\end{cases}
```

</details>

<br>

b.
```math	
\begin{bmatrix} 1 & -1 & -2 & 3\\
                    4 & -2 & -8 & 2\end{bmatrix}
```



<details>

<br>
<summary> </summary>

```math
\begin{cases}
x_1 = -2+2x_3\\
x_2 = -5\\
x_3 \text{ free}
\end{cases}
```

</details>

<br>

c.
```math	
\begin{bmatrix} -2 & 4 & -3 & 0\\
                    4 & -8 & 6& 0\\
                    -6& 12& -9 & 0\end{bmatrix}
```

<details>

<br>
<summary> </summary>

```math
\begin{cases}
x_1 = 2x_2 - \frac{3}{2}x_3\\
x_2 \text{ free}\\
x_3 \text{ free}
\end{cases}
```


</details>

<br>


### Exercise 6: Consistency of the system
Which of the augmented matrices below represent an inconsistens system of equations?

a. 
```math
\begin{bmatrix}
    0 & 3 & -2 & 1\\
    0 & 0  & -1 & 4\\
    0 & 0  & 0 & 0
\end{bmatrix}
```

b.
```math
\begin{bmatrix}
    -1 & 3 & 1 \\
    0 & 5  & 3 \\
    0 & 0  & 6 
\end{bmatrix}
```

c.
```math
\begin{bmatrix}
    7 & 1 & 1 \\
    0 & 2  & 2 \\
    0 & 0  & 3 \\
    0 & 0  & 0
\end{bmatrix}
```

d. 
```math
\begin{bmatrix}
    1 & 0 \\
    0 & 1 
\end{bmatrix}
```

e.
```math
\begin{bmatrix}
    -3 & 0 & 0 & 9\\
    0 & 1  & 0 & 0\\
    0 & 0  & 4 & 0
\end{bmatrix}
```

f.
```math
\begin{bmatrix}
    0 & 0 & 6 & 3
\end{bmatrix}
```


<details>

<br>
<summary> </summary>

inconsistent: b, c, d

consistent: a, e, f


</details>

<br>

g. For the consistens systems find the general solution.

<details>

<br>
<summary> </summary>

a.
```math	
\begin{cases}
x_1  \text{ free}\\
x_2 = -\frac{7}{3}\\
x_3 = -4
\end{cases}
```

e.
```math
\begin{cases}
x_1 = -3\\
x_2 = 0\\
x_3 = 0
\end{cases}
```

f.
```math
\begin{cases}
x_1 \text{ free}\\
x_2 \text{ free}\\
x_3 = \frac{1}{2}
\end{cases}
```
</details>

<br>


### Exercise 7: Plan a diet
Use Python to solve this exercise. 

For a week you decide to eat only butter, apples, and oats.

|Nutritional values per 100 g|  Butter  |  Apple  |  Oats  | Rye bread|
|----------------------------|---------:|--------:|-------:|---------:|
|Protein       (g)           |    0.2   |   0.3   | 14.0   |    6.4   |
|Fat           (g)           |   82.5   |   0.2   |  6.9   |    4.7   |
|Carbohydrates (g)           |    0.0   |   12.1  | 57.0   |   32.0   |

a. How much butter, apple, and oats do you need to eat to get 50 g of protein, 70 g of fat, and 260 g of carbohydrates per day?

<details>

<br>
<summary> </summary>

```math
\begin{cases}  54.7 \text{ g butter}\\
                522.8\text{ g apple}\\
                345.2 \text{ g oats}\end{cases}
```

</details>

<br>

Next week, you decide to replace apples with rye bread.

b. Is it possible to plan a diet of butter, rye bread, and oats to still get 50 g of protein, 70 g of fat and 260 g of carbohydrate per day?

<details>

<br>
<summary> </summary>

The system of linear equations has a unique solution. However, the solution contains a negative amount of oats, which does not make sense.

</details>

<br>