# 📘 Calculus 1 – Unit 6: Integrals

*This file documents concepts, strategies, and worked examples from Khan Academy's Unit on Integrals.*

🔗 Source: [Khan Academy – Integrals](https://www.khanacademy.org/math/calculus-1/cs1-integrals)

---

## 📌 Accumulations of Change — Introduction to Integrals

If a function $f(x)$ represents a rate of change, then the accumulated change from $a$ to $b$ is:

$$
\int_a^b f(x) dx
$$

This represents the **signed area** under $f(x)$ between $x=a$ and $x=b$.

**Example:**

If $f(x)=3$, then

$$
\int_1^4 3 dx = 3 \cdot (4-1) = 9
$$

---

## 📌 Approximation with Riemann Sums

Divide $[a,b]$ into $n$ subintervals of equal width:

$$
\Delta x=\frac{b-a}{n}, \quad x_i=a+i\Delta x
$$

A general Riemann sum is:

$$
\sum_{i=1}^n f(x_i^*) \Delta x
$$

where $x_i^*$ is any point in $[x_{i-1},x_i]$.

* Special cases:  
  - Left sum: $x_i^*=x_{i-1}$  
  - Right sum: $x_i^*=x_i$  
  - Midpoint sum: $x_i^*=\dfrac{x_{i-1}+x_i}{2}$

---

## 📌 Numerical Integration — Midpoint and Trapezoidal Rules

**Midpoint rule:**

$$
M_n = \Delta x \sum_{i=1}^n f\left(\frac{x_{i-1}+x_i}{2}\right)
$$

**Trapezoidal rule:**

$$
T_n = \frac{\Delta x}{2}\left(f(x_0)+2\sum_{i=1}^{n-1}f(x_i)+f(x_n)\right)
$$

---

## 📌 Summation Notation Review

Common formulas:

$$
\sum_{i=1}^n i = \frac{n(n+1)}{2}, \quad
\sum_{i=1}^n i^2 = \frac{n(n+1)(2n+1)}{6}, \quad
\sum_{i=1}^n c = nc
$$

---

## 📌 Riemann Sums in Summation Notation

For $f(x)$ on $[a,b]$, a Riemann sum with $n$ rectangles is:

$$
\sum_{i=1}^n f(x_i) \Delta x, \quad \Delta x=\frac{b-a}{n}
$$

---

## 📌 Defining Integrals with Riemann Sums

The **definite integral** is defined as the limit of Riemann sums:

$$
\int_a^b f(x) dx = \lim_{n\to\infty}\sum_{i=1}^n f(x_i^*) \Delta x
$$

if the limit exists.

---

## 📌 Fundamental Theorem of Calculus and Accumulation Functions

**FTC Part 1:**  
If $F(x)=\int_a^x f(t) dt$, then

$$
F'(x)=f(x)
$$

**Example:**

$$
F(x)=\int_0^x \cos(t) dt \quad\implies\quad F'(x)=\cos(x)
$$

---

## 📌 Fundamental Theorem of Calculus and Definite Integrals

**FTC Part 2:**  
If $F'(x)=f(x)$, then

$$
\int_a^b f(x) dx=F(b)-F(a)
$$

**Example:**

$$
\int_0^2 3x^2 dx = \big[x^3\big]_0^2 = 8
$$

---

## 📌 Interpreting the Behavior of Accumulation Functions

If $F(x)=\int_a^x f(t) dt$:

- $F$ increases where $f(x)>0$
- $F$ decreases where $f(x)<0$
- Local maxima/minima of $F$ occur where $f(x)$ changes sign

---

## 📌 Properties of Definite Integrals

- $\int_a^a f(x) dx=0$  
- $\int_a^b f(x) dx = -\int_b^a f(x) dx$  
- $\int_a^c f(x) dx = \int_a^b f(x) dx + \int_b^c f(x) dx$  
- $\int_a^b \big(f(x)+g(x)\big) dx = \int_a^b f(x) dx + \int_a^b g(x) dx$  
- $\int_a^b k f(x) dx = k \int_a^b f(x) dx$  

---

## 📌 Reverse Power Rule

For $n\neq -1$:

$$
\int x^n dx=\frac{x^{n+1}}{n+1}+C
$$

---

## 📌 Indefinite Integrals of Common Functions

| Function $f(x)$ | Antiderivative $\int f(x) dx$ |
|-----------------|--------------------------------|
| $e^x$           | $e^x+C$                        |
| $\sin(x)$       | $-\cos(x)+C$                   |
| $\cos(x)$       | $\sin(x)+C$                    |
| $\sec^2(x)$     | $\tan(x)+C$                    |
| $\csc^2(x)$     | $-\cot(x)+C$                   |
| $\sec(x)\tan(x)$| $\sec(x)+C$                    |
| $\csc(x)\cot(x)$| $-\csc(x)+C$                   |
| $1/x$           | $\ln(x)+C$                    |

---

## 📌 Definite Integrals of Common Functions

- $\int_a^b e^x dx=e^b-e^a$  
- $\int_0^\pi \sin(x) dx=2$  
- $\int_1^e \frac{1}{x} dx=1$

---

## 📌 Integrating with $u$-Substitution

Let $u=g(x)$, then $du=g'(x) dx$.

**Example:**

$$
\int 2x e^{x^2} dx,\quad u=x^2, du=2x dx
$$

$$
\int e^u du=e^u+C=e^{x^2}+C
$$

---

## 📌 Integrating Using Long Division and Completing the Square

**Long division:** use when $\deg(\text{numerator}) \ge \deg(\text{denominator})$.  
**Completing the square:** transforms quadratic denominators for $\arctan$ or $\ln$ integrals.

**Example:**

$$
\int \frac{1}{x^2-14x+58} dx
$$

Complete the square: $x^2-14x+58=(x-7)^2+9$

$$
\int \frac{1}{(x-7)^2+3^2} dx=\frac{1}{3}\arctan\left(\frac{x-7}{3}\right)+C
$$

---

## 📌 Integrating Using Trigonometric Identities

- $\sin^2(x)=\frac{1-\cos(2x)}{2}$  
- $\cos^2(x)=\frac{1+\cos(2x)}{2}$  
- $\sin(x)\cos(x)=\frac{1}{2}\sin(2x)$  

**Example:**

$$
\int \sin^2(x) dx=\int \frac{1-\cos(2x)}{2} dx=\frac{x}{2}-\frac{\sin(2x)}{4}+C
$$

---

## ✅ Summary of Topics in Unit 6

* [x] Accumulations of change & integrals  
* [x] Approximation with Riemann sums  
* [x] Numerical methods (midpoint & trapezoidal)  
* [x] Summation notation & Riemann sums in notation  
* [x] Defining integrals with limits of sums  
* [x] Fundamental Theorem of Calculus — **Part 1**  & **Part 2**   
* [x] Interpreting accumulation functions  
* [x] Properties of definite integrals  
* [x] Reverse power rule  
* [x] Indefinite integrals of common functions  
* [x] Definite integrals of common functions  
* [x] $u$-substitution  
* [x] Long division & completing the square  
* [x] Integrating with trigonometric identities  

---

> This file is part of my AI/ML journey repo documenting foundational math skills before diving into machine learning and AI.



