<!-- enable inline eqn and add new macro definitions -->
<script>
  MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']],
      macros: {
        indep: "{\\perp \\!\\!\\! \\perp}",
      }
    },
    svg: {
    fontCache: 'global'
  }
  };
</script>

<!-- load MathJax -->
<script type="text/javascript" id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>

## Exercises: Basic Arithmetic and Functions

### Exercise 1:

Solve the following equations

a. $\quad 2-\frac{4 x+3}{x+x^2}=\frac{2 x}{x+1}-\frac{5}{x}$

<details>

<br>
<summary> </summary>

$x=-\frac{2}{3}$

</details>

<br>

b. $\quad -2+2 \ln 3 x=17$

<details>

<br>
  <summary> </summary>

$x=\frac{e^{\frac{19}{2}}}{3}$

</details>

<br>

c. $\quad \ln (x+1)^2=2$

<details> <br>
  <summary> </summary>

$x= \pm e-1$

</details>

<br>

d. $\quad \ln \left(x^2+1\right)=8$

<details> <br>
  <summary> </summary>

$x= \pm \sqrt{-1+e^8}$

</details>

<br>

e. $\quad 5^{3 x+2}=25^{x-1}$

<details> <br>
  <summary> </summary>

$x=-4$

</details>

<br>

### Exercise 2:

According to Einstein's theory of relativity, the mass of a particle is given by

$$
m=\frac{m_0}{\sqrt{1-\left(\frac{v}{c}\right)^2}}
$$

where
$m_0$ is the mass of the particle at rest
$v$ is the speed of the particle, and
$c$ is the speed of light in a vacuum.

a. Make $v$ the subject of the formula given $v>0$

<details> <br>
  <summary> </summary>

$v=c \cdot \sqrt{1-\left(\frac{m_0}{m}\right)^2}$

</details>

<br>

b. Find the speed necessary to increase the mass of a particle to three times its rest mass. Give the value for $v$ as a fraction of $c$ (or as a decimal).

<details> <br>
  <summary> </summary>

$v=0.943 c$

</details>

<br>

### Exercise 3
Determine the domain and range of each of the real functions below. It is a good idea to plot the functions using some software (e.g. Geogebra, WolframAlpha, etc.):

a. $\quad f(x)=\frac{1}{x-7}$

<details> <br>
  <summary> </summary>

Domain: $\mathbb{R} \backslash\{7\}$;
Range: $\mathbb{R} \backslash\{0\}$

</details>

<br>

b. $\quad f(x)=\sqrt{x+3}$

<details> <br>
  <summary> </summary>

Domain: $\mathbb{R}_ {\geq-3}$;
Range: $\mathbb{R}_ {\geq 0}$

</details>

<br>

### Exercise 4
Find each of the following composite functions:

a. $\quad g \circ f$ when $f(x)=3 x+1$ and $g(x)=x^2$.

<details> <br>
  <summary> </summary>

$(g \circ f)(x)=9 x^2+1+6 x$

</details>

<br>

b. $f \circ g$ when $f(x)=x^2+1$ and $g(x)=\frac{1}{x}$.

<details> <br>
  <summary> </summary>

$(f \circ g)(x)=\frac{1}{x^2}+1$

</details>

<br>


c. $\quad g \circ f$ when $f$ and $g$ are defined as in exercise (b).

<details> <br>
  <summary> </summary>

$(g \circ f)(x)=\frac{1}{x^2+1}$

</details>

<br>

### Exercise 5
Find the inverse

a. $\quad f(x)=\frac{6}{5-x}$

<details> <br>
  <summary> </summary>

$f^{-1}(x)=5-\frac{6}{x}$

</details>

<br>

b. $\quad f(x)=-\ln (1-2 x)+1$

<details> <br>
  <summary> </summary>

$f^{-1}(x)=\left(1-e^{1-x}\right) / 2$


</details>

<br>

c. $\quad f(x)=2 \cdot 10^{3 x}-1$

<details> <br>
  <summary> </summary>

$f^{-1}(x)=\frac{\log \left(\frac{x+1}{2}\right)}{3}$

</details>

<br>

### Exercise 6

A bacteria culture starts with 1000 bacteria at time $t=0$ and the number doubles every 40 minutes.

a. Find a functional expression for the number of bacteria at time $t$ (measured in minutes).

<details> <br>
  <summary> </summary>

$f(t)=1000 \cdot 2^{t / 40}$

</details>

<br>

b. Find the number of bacteria after one hour.

<details> <br>
  <summary> </summary>

$f(60) \approx 2828$

</details>

<br>

c. After how many minutes will there be 50000 bacteria?

<details> <br>
  <summary> </summary>

approx. 225.75 minutes

</details>

<br>