## Exercises: Combinatorics and Probability Theory

### Exercise 1: Boolean Algebra Recap

Consider the Boolean function $F(x, y, z)=x y+y(z+x)$. 

a. State the truth table for this function. If the table is constructed correctly, the last column will contain $F$ and will have 8 rows. Reading the rows from the bottom up will give you a binary value. Convert this value to decimal and state this as your result.
<details>
<br>
<summary> </summary>
200
</details>
<br>

b. Reduce the expression as much as possible and create the corresponding logic gate.
<details>
<br>
<summary> </summary>
<img src="/05_Combinatorics_and_Probability_Theory/logic1.png" width = "200">
</details>
<br>

c. Use Boolean algebra to simplify the following logic gate circuit and state the result as a boolean algebra expression.

<img src="/05_Combinatorics_and_Probability_Theory/logic2.png" width = "400">

<details>
<br>
<summary> </summary>

$AB+AC$

</details>
<br>

### Exercise 2: Combinatorics and Probability

a. An order for a personal digital assistant can specify any one of five memory sizes, any one of three types of displays, any one of four sizes of a hard disk, and can either include or not include a pen tablet. How many different systems can be ordered? State which Rule/Theorem from the book that you use.

<details>
<br>
<summary> </summary>

We multiply the number of possibilities for each of the choices: $5 \cdot 3 \cdot 4 \cdot 2=120$, which means we are using the Theorem 5.1 (Multiplication Rule)

</details>
<br>


b. A wireless garage door opener has a code determined by the up or down setting of 12 switches.

i. How many possible codes are there?

<details>
<br>
<summary> </summary>

$2^{12} = 4096$ 

</details>
<br>

ii. What is the probability that a burglar guesses the right code in the first try?


<details>
<br>
<summary> </summary>

$\frac{1}{4096} = 0.000244 = 0.0244\\%$

</details>
<br>

### Exercise 3: Combinatorics and Probability

A group of 3 kids is to be formed in a class of 15 kids.

a. In how many different ways can you make the group if the order of the kids doesn't matter?

<details>
<br>
<summary> </summary>

$\frac{15!}{(15-3)!\cdot 3!}=455$

</details>
<br>

b. In how many different ways can you make the group if the order of the kids does matter?

<details>
<br>
<summary> </summary>

$\frac{15!}{(15-3)!}=2730$

</details>
<br>

c.	What is the probability that the group will consist of the three kids Xavier, Ygritte and Zelda?

<details>
<br>
<summary> </summary>

$\frac{1}{455}=\frac{6}{2730}=0.00220 = 0.220\\%$

</details>
<br>

### Exercise 4: Poker Hands
In how many ways can you deal a poker hand of five cards from a standard deck of 52 cards? Also, how many ways are there to select 47 cards from a standard deck of 52 cards?

<details>
<br>
<summary> </summary>

$\frac{52!}{(52-5)!\cdot 5!}=2,598,960$

</details>
<br>

### Exercise 5: Garage Doors and Burglars Revisited

Recall the garage doors from Exercise 2b. What is the probability that a burglar guesses the right code in 3 tries, assuming that the guesses happen with replacement, i.e. that the probability for each try is the same?

<details>
<br>
<summary> </summary>

$P($ at least one correct $) = 1-\left(\frac{4095}{4096}\right)^3 \approx 0.00073$

</details>
<br>

### Exercise 6: Webpage Passwords
A webpage requires the user to create a password that contains exactly 4 characters. Let $A$ denote the set of passwords containing only letters (there are 26 lowercase letters, a-z, and 26 uppercase letters, A-Z), let $B$ denote the set of passwords containing only numbers (0-9), and let $C$ denote the set of passwords that can contain both letters and numbers.  A hacker tries to guess the password of a particular user. What is the probability that he guesses the correct password in the first attempt in each of the cases below?

a. The webpage only allows passwords from set $A$

<details>
<br>
<summary> </summary>

$\frac{1}{7,311,616}$

</details>
<br>

b.	 The webpage only allows passwords from set $B$.

<details>
<br>
<summary> </summary>

$\frac{1}{10,000}$

</details>
<br>

c. The webpage only allows passwords from set $A \cup B$.

<details>
<br>
<summary> </summary>

$\frac{1}{7,321,616}$

</details>
<br>

d. What is the probability that the hacker guesses the correct password in the first attempt if the webpage allows passwords from set $C$?

<details>
<br>
<summary> </summary>

$\frac{1}{14,776,336}$

</details>
<br>

### Exercise 7: Probability
The possible five outcomes of a random experiment are equally likely. The sample space is ${a,b,c,d,e}$. Let $A$ denote the event ${a,b}$, and $B$ denote the event ${c,d,e}$.

a. Draw a Venn diagram showing the sample space and each of the events A and B.

<details>
<br>
<summary> </summary>
<img src="/05_Combinatorics_and_Probability_Theory/venn1.png" width = "300">
</details>
<br>

b. Determine each of the following probabilities:

$P(A)$  
$P(B)$  
$P(\overline{A})$  
$P(A \cup B)$  
$P(A \cap B)$

<details>
<br>
<summary> </summary>

$P(A) = \frac{2}{5}$

$P(B) = \frac{3}{5}$  

$P(\overline{A}) = \frac{3}{5}$  

$P(A \cup B) = 1$  

$P(A \cap B) = 0$

</details>
<br>

### Exercise 8: Challenge Exercise
A computer password consists of 4 characters, each one of 26 lowercase letters or 26 uppercase letters or an integer between 0 and 9. If the password must contain at least one letter and at least one integer, how many different passwords are possible?

<details>
<br>
<summary> </summary>

The easiest way to calculate this, is to first calculate the number of 4-character passwords, and then subtract those that do not fulfill the rule, i.e. the passwords that do either only contain letters or only numbers: $62^4-52^4-10^4=7,454,720$

</details>
<br>