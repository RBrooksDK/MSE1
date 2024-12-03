# 1. Introduction: Basic Arithmetic and Functions

### Session Preparation:

Brooks: [Chapter 1](https://drive.google.com/file/d/1P9eidJb5qtlZgvHCtqu4uuPa5FFU0Zpn/view?usp=sharing).

We will not be going through the arithmetic part, but we will be doing examples and exercises in arithmetic. So you need to prepare this on your own before classes.

### Session Material:

[Session notes](https://drive.google.com/file/d/1IXTVyUP_TeX4co_uwSSlf6AHYYrln1fL/view?usp=drive_link)

[Session Resources](https://viaucdk-my.sharepoint.com/:f:/g/personal/rib_viauc_dk/EtdW6vDKB6FHsPZdtO6XUhMB5n3uwC00IoyfXj5g1O6JlA?e=vAY78F)

--------------------------

### Topic Description
In this first session, we will lay the groundwork for our study of mathematics within the context of software engineering. The session will begin with an overview of the course structure, objectives, and expectations. Following this, we will review and practice essential calculation rules and the basic properties of functions. These fundamental concepts are critical as they form the basis for more advanced topics that will be covered later in the course.

The focus will be on understanding and applying the power rules, radicals, exponents, and logarithms. We will also explore the definition and types of functions, delving into their domains, codomains, and ranges. Finally, we'll introduce the concepts of inverse and composite functions, which will be important for later discussions.

#### Key Concepts
- Introduction to the course
- Review of basic calculation rules
- Power rules
- Radicals (roots)
- Exponents
- Logarithms
- Definition and types of functions
- Domain, codomain, and range
- Inverse function
- Composite functions
--------------------------

### Exercises for recitation

[Notes from recitation](https://drive.google.com/file/d/1wDoPLD34pPfCy0JqtNpFQ9sGq8FMTWM2/view?usp=sharing)

#### Exercise 1:

Solve the following equations 1

a. $\quad 2-\frac{4 x+3}{x+x^2}=\frac{2 x}{x+1}-\frac{5}{x}$ (1)
{ .annotate }

1. $$x=-\frac{2}{3}$$


b. $\quad -2+2 \ln 3 x=17$ (1)
{ .annotate }

1. $$x=\frac{e^{\frac{19}{2}}}{3}$$

c. $\quad \ln (x+1)^2=2$ (1)
{ .annotate }

1. $$x= \pm e-1$$

d. $\quad \ln \left(x^2+1\right)=8$ (1)
{ .annotate }

1. $x= \pm \sqrt{-1+e^8}$

e. $\quad 5^{3 x+2}=25^{x-1}$(1)
{ .annotate }

1. $x=-4$

#### Exercise 2:

According to Einstein's theory of relativity, the mass of a particle is given by

$$
m=\frac{m_0}{\sqrt{1-\left(\frac{v}{c}\right)^2}}
$$

where
$m_0$ is the mass of the particle at rest
$v$ is the speed of the particle, and
$c$ is the speed of light in a vacuum.

a. Make $v$ the subject of the formula given $v>0$ (1)
{ .annotate }

1. $v=c \cdot \sqrt{1-\left(\frac{m_0}{m}\right)^2}$

b. Find the speed necessary to increase the mass of a particle to three times its rest mass. Give the value for $v$ as a fraction of $c$ (or as a decimal).(1)
{ .annotate }

1. $v=0.943 c$

#### Exercise 3
Determine the domain and range of each of the real functions below. It is a good idea to plot the functions using some software (e.g. Geogebra, WolframAlpha, etc.):

a. $\quad f(x)=\frac{1}{x-7}$

??? answer "&nbsp;"

    Domain: $\mathbb{R} \backslash\{7\}$;

    Range: $\mathbb{R} \backslash\{0\}$


b. $\quad f(x)=\sqrt{x+3}$

??? answer "&nbsp;"

    Domain: $\mathbb{R}_ {\geq-3}$;

    Range: $\mathbb{R}_ {\geq 0}$

#### Exercise 4
Find each of the following composite functions:

a. $\quad g \circ f$ when $f(x)=3 x+1$ and $g(x)=x^2$.


??? answer "&nbsp;"

    $(g \circ f)(x)=9 x^2+1+6 x$


b. $f \circ g$ when $f(x)=x^2+1$ and $g(x)=\frac{1}{x}$.

??? answer "&nbsp;"

    $(f \circ g)(x)=\frac{1}{x^2}+1$

c. $\quad g \circ f$ when $f$ and $g$ are defined as in exercise (b).

??? answer "&nbsp;"

    $(g \circ f)(x)=\frac{1}{x^2+1}$

#### Exercise 5
Find the inverse

a. $\quad f(x)=\frac{6}{5-x}$

??? answer "&nbsp;"

    $f^{-1}(x)=5-\frac{6}{x}$

b. $\quad f(x)=-\ln (1-2 x)+1$

??? answer "&nbsp;"

    $f^{-1}(x)=\left(1-e^{1-x}\right) / 2$

c. $\quad f(x)=2 \cdot 10^{3 x}-1$

??? answer "&nbsp;"

    $f^{-1}(x)=\frac{\log \left(\frac{x+1}{2}\right)}{3}$

#### Exercise 6

A bacteria culture starts with 1000 bacteria at time $t=0$ and the number doubles every 40 minutes.

a. Find a functional expression for the number of bacteria at time $t$ (measured in minutes).

??? answer "&nbsp;"
    $f(t)=1000 \cdot 2^{t / 40}$

b. Find the number of bacteria after one hour.

??? answer "&nbsp;"

    $f(60) \approx 2828$

c. After how many minutes will there be 50000 bacteria?

??? answer "&nbsp;"

    approx. 225.75 minutes