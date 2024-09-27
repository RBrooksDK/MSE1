## Exercises: Boolean Algebra

### Exercise 1: Numeral Systems Recap

RGBA is an extension to the (R)ed (G)reen (B)lue color model, which includes an (A)lpha channel representing the level of opacity from $0.0$ to $1.0$, where $0.0$ is fully transparent (i.e. invisible) and $1.0$ is fully opaque.
The four channels are represented by 1 byte (8 bits) each, often expressed in hexadecimal, where for instance # $A01009FF$ corresponds to RGBA($160, 16, 9, 1.0$), a fully opaque medium dark red.

a. What is the maximum decimal value for any of the RGB channels?
<details>
<br>
<summary> </summary>
$255$
</details>
<br>

b. What is the cardinality (or the order) of the set of all possible RGB colors?
<details>
<br>
<summary> </summary>
$16^{6} = 16 777 216$
</details>
<br>

c. What is the cardinality (or the order) of the set of all possible RGBA colors, if all colors with an alpha of $0$ are considered the same?
<details>
<br>
<summary> </summary>
$16^{6} \cdot (16^2-1) + 1 = 16 777 216 \cdot 255 + 1 = 4 278 190 081$
</details>
<br>

d. Express an opacity level of $0.8$ in binary.
<details>
<br>
<summary> </summary>
$255 \cdot 0.8 = 204_{10} = 11001100_2$
</details>
<br>

e. What is the hexadecimal value for an opacity of $0.5$?
<details>
<br>
<summary> </summary>
$\approx 7F$ or $80$
</details>
<br>

### Exercise 2: Boolean Calculation

Calculate

a. $1 \cdot \overline{1}$  
<details>
<br>
<summary> </summary>
$0$
</details>
<br>

b. $\overline{1} + \overline{0}$  
<details>
<br>
<summary> </summary>
$1$
</details>
<br>

c. ![$\overline{0 \cdot (1 + 0)}$](https://github.com/jakobmwang/MSE1/blob/main/src/equation%20(5).svg)
<details>
<br>
<summary> </summary>
$1$
</details>
<br>

d. $\overline{1} + (0 \cdot 1)$  
<details>
<br>
<summary> </summary>
$0$
</details>
<br>

### Exercise 3: Boolean Functions
Construct the truth table for

a. $F(x) = x + (x \cdot \overline{x})$

| $x$ | $\overline{x}$ | $(x \cdot \overline{x})$ | $F(x) = x + (x \cdot \overline{x})$ |
|:-:|:------------------:|:--------------------------:|:---------------------------------------:|
|  |         &nbsp;          |                         |                                     |
|  |         &nbsp;          |                          |                                     |

<details>
<br>
<summary> </summary>

| $x$ | $\overline{x}$ | $(x \cdot \overline{x})$ | $F(x) = x + (x \cdot \overline{x})$ |
|:-:|:------------------:|:--------------------------:|:---------------------------------------:|
| 0 |         1          |             0              |                   0                    |
| 1 |         0          |             0              |                   1                    |

</details>
<br>

b. $G(x,y) = \overline{x} \cdot (\overline{x} + \overline{y})$

<details>
<br>
<summary> </summary>

| $x$ | $y$ | $\overline{x}$ | $\overline{y}$ | $(\overline{x} + \overline{y})$ | $G(x,y)=\overline{x} \cdot (\overline{x} + \overline{y})$ |
|:-:|:-:|:------------------:|:------------------:|:--------------------------------:|:------------------------------------------------------------:|
| 0 | 0 |         1          |         1          |               1                |                              1                               |
| 0 | 1 |         1          |         0          |               1                |                              1                               |
| 1 | 0 |         0          |         1          |               1                |                              0                               |
| 1 | 1 |         0          |         0          |               0                |                              0                               |

</details>
<br>

c. $H(x, y, z) = (x \cdot \overline{y}) + \overline{z}$

<details>
<br>
<summary> </summary>

| $x$ | $y$ | $z$ | $\overline{y}$ | $\overline{z}$ | $(x \cdot \overline{y})$ | $H(x,y,z)=(x \cdot \overline{y}) + \overline{z}$ |
|:-:|:-:|:-:|:------------------:|:------------------:|:--------------------------:|:--------------------------------------------------------:|
| 0 | 0 | 0 |         1          |         1          |             0              |                            1                             |
| 0 | 0 | 1 |         1          |         0          |             0              |                            0                             |
| 0 | 1 | 0 |         0          |         1          |             0              |                            1                             |
| 0 | 1 | 1 |         0          |         0          |             0              |                            0                             |
| 1 | 0 | 0 |         1          |         1          |             1              |                            1                             |
| 1 | 0 | 1 |         1          |         0          |             1              |                            1                             |
| 1 | 1 | 0 |         0          |         1          |             0              |                            1                             |
| 1 | 1 | 1 |         0          |         0          |             0              |                            0                             |

</details>
<br>

### Exercise 4: Boolean Expressions

Simplify

a. $(x + \overline{x}) \cdot y$  
<details>
<br>
<summary> </summary>
$y$
</details>
<br>

b. <img src="https://github.com/jakobmwang/MSE1/blob/main/src/equation%20(10).svg">
<details>
<br>
<summary> </summary>
<img src="https://github.com/jakobmwang/MSE1/blob/main/src/equation_0.svg">
</details>
<br>

c. $x \cdot (y + \overline{x})$  
<details>
<br>
<summary> </summary>
$x \cdot y$
</details>
<br>

d. <img src="https://github.com/jakobmwang/MSE1/blob/main/src/equation%20(9).svg">
<details>
<br>
<summary> </summary>
$x + \overline{y} + z$
</details>
<br>

e. $x \cdot y + \overline{x} \cdot y$  
<details>
<br>
<summary> </summary>
$y$
</details>
<br>

f. $x + y \cdot (\overline{x} + \overline{y})$
<details>
<br>
<summary> </summary>
$x + y$
</details>
<br>

g. $(x \cdot \overline{y}) + (\overline{x} \cdot y)$  
<details>
<br>
<summary> </summary>
$(x \cdot \overline{y}) + (\overline{x} \cdot y)$
</details>
<br>

h. <img src="https://github.com/jakobmwang/MSE1/blob/main/src/equation%20(8).svg">
<details>
<br>
<summary> </summary>
$1$
</details>
<br>

### Exercise 5: Problem

Let $A$ be 1 if you exceed the speed limit, 0 if not.

Let $B$ be 1 if the police sees you, 0 if not.

Let $C$ be 1 if your car is faster than the police car, 0 if not.

a. Create a function $F$ that returns 1 if you get a speeding ticket, 0 if you do not.
<details>
<br>
<summary> </summary>
$F(A,B,C) = A \cdot B \cdot \overline{C}$

$F(A,B,C) = A \cdot B \cdot 1$ if you are not into car chases.
</details>
<br>

### Exercise 6: Interpreting Circuits

Write the boolean expression for

a. <img src="https://github.com/jakobmwang/MSE1/blob/main/src/circuit3.png">
<details>
<br>
<summary> </summary>
$\overline{xy}+(\overline{z}+x)$
</details>
<br>

b. <img src="https://github.com/jakobmwang/MSE1/blob/main/src/circuit4.png">
<details>
<br>
<summary> </summary>
<img src="https://github.com/jakobmwang/MSE1/blob/main/src/equation%20(7).svg">
</details>
<br>

### Exercise 7: Constructing Circuits

Draw the circuits for

a. $x + y \cdot (\overline{x} + \overline{y})$
<details>
<br>
<summary> </summary>
<img src="https://github.com/jakobmwang/MSE1/blob/main/src/circuit5.png" width = "500">
</details>
<br>

b. $xy + \overline{x}y$
<details>
<br>
<summary> </summary>
<img src="https://github.com/jakobmwang/MSE1/blob/main/src/circuit6.png" width = "400">
</details>
<br>

c. ![$xyz + \overline{xyz}$](https://github.com/jakobmwang/MSE1/blob/main/src/equation%20(6).svg)
<details>
<br>
<summary> </summary>
<img src="https://github.com/jakobmwang/MSE1/blob/main/src/circuit7.png" width = "400">
</details>
<br>

### Exercise 8: Challenge

The VIA building has implemented a new area access system:

Everyone can access the lobby. <br>
To access the cafeteria, it has to be before 14:00. <br>
To access the classrooms, you have to be a student or a teacher. <br>
Everyone can access the elevators. <br>
To access the study rooms, you have to be a student. <br>
To access the offices, it has to be before 14:00, and you have to be a teacher. <br>
To access the luxurious lounge, it has to be after 14:00, and you have to be a teacher. <br>
To access the secret room, it has to be after 14:00, and you have to be both a student and a teacher. <br>

a. Define the boolean variables necessary to represent all of the above criteria for access.
<details>
<br>
<summary> </summary>
$A$: lobby <br>
$B$: cafeteria <br>
$C$: classrooms <br>
$D$: elevators <br>
$E$: study rooms <br>
$F$: offices <br>
$G$: luxurious lounge <br>
$H$: secret room <br>
$I$: student <br>
$J$: teacher <br>
$K$: before 14:00,
$\overline{K}$: after 14:00 <br>
</details>
<br>
b. Create a single boolean function that accepts the above variables to precisely evaluate whether access is granted or not, covering all cases.
<details>
<br>
<summary> </summary>
$f(A,B,C,D,E,F,G,H,I,J,K)=A+BK+C(I+J)+D+EI+FJK+GJ\overline{K}+HIJ\overline{K}$
</details>
<br>
c. Reduce the footprint of the access system by simplifying into a minimum of variables and terms.
<details>
<br>
<summary> </summary>
$f(A,B,C,D,E,F)=ABD+\overline{A}\overline{B}+C\overline{A}\overline{F}+AEF\overline{C}+DEF\overline{B}+BE\overline{C}\overline{F}$

(Note: This function is equivalent to the function in (b) but the variables do not correspond to the variables in (a).)
</details>
<br>