# 📘 Calculus 1 – Unit 6: Integrals & Accumulation

*This file documents concepts, strategies, and examples from Khan Academy's Unit on Integrals.*

🔗 Source: [Khan Academy – Integrals](https://www.khanacademy.org/math/calculus-1/cs1-integrals)

---

## 📌 Accumulations of Change – Introduction: Integrals

* If a quantity changes at rate $f(x)$, then the accumulated change from $a$ to $b$ is:

$$
\int_a^b f(x)\,dx
$$

* Geometric meaning: the **signed area** under the curve.

**Example:**

Water flows at rate $r(t)=5$ liters/min. Over 10 minutes:

$$
\int_0^{10} 5\,dt = 50 \ \text{liters}
$$

---

## 📌 Approximation with Riemann Sums

Approximate area with rectangles:

$$
\sum_{i=1}^n f(x_i^*) \,\Delta x
$$

* **Left Riemann Sum:** use left endpoints  
* **Right Riemann Sum:** use right endpoints  
* **Midpoint Rule:** use midpoints

---

## 📌 Riemann Sums in Summation Notation

For interval $[a,b]$, subdivide into $n$ parts:

$$
\Delta x = \frac{b-a}{n}
$$

Right sum:

$$
\sum_{i=1}^n f\\big(X_i)\Delta x\,\Delta x
$$

---

## 📌 Defining Integrals with Riemann Sums

The definite integral is defined as the limit:

$$
\int_a^b f(x)\,dx = \lim_{n\to\infty}\sum_{i=1}^n f(x_i^*)\Delta x
$$

---

## 📌 Fundamental Theorem of Calculus & Accumulation Functions

* Define $F(x)=\int_a^x f(t)\,dt$  
* Then $F'(x)=f(x)$ if $f$ is continuous

**Example:**

$$
F(x)=\int_0^x \sin t\,dt \quad\implies\quad F'(x)=\sin x
$$

---

## 📌 Interpreting the Behavior of Accumulation Functions

* If $f(x)>0$, $F(x)$ is increasing  
* If $f(x)<0$, $F(x)$ is decreasing  
* Zeros of $f(x)$ correspond to extrema of $F(x)$

---

## 📌 Properties of Definite Integrals

1. $\int_a^b f(x)\,dx = -\int_b^a f(x)\,dx$  
2. $\int_a^a f(x)\,dx = 0$  
3. $\int_a^b f(x)\,dx+\int_b^c f(x)\,dx=\int_a^c f(x)\,dx$  
4. $\int_a^b c f(x)\,dx = c\int_a^b f(x)\,dx$  
5. $\int_a^b (f+g)=\int_a^b f + \int_a^b g$

---

## 📌 Fundamental Theorem of Calculus & Definite Integrals

If $F$ is an antiderivative of $f$:

$$
\int_a^b f(x)\,dx = F(b)-F(a)
$$

---

## 📌 Reverse Power Rule

$$
\int x^n dx = \frac{x^{n+1}}{n+1}+C \quad (n\neq -1)
$$

**Example:**

$$
\int x^3 dx = \frac{x^4}{4}+C
$$

---

## 📌 Indefinite Integrals of Common Functions

| $f(x)$          | $\int f(x)\,dx$ |
|-----------------|-----------------|
| $e^x$           | $e^x+C$ |
| $\sin x$        | $-\cos x+C$ |
| $\cos x$        | $\sin x+C$ |
| $\sec^2 x$      | $\tan x+C$ |
| $\csc^2 x$      | $-\cot x+C$ |
| $\sec x \tan x$ | $\sec x+C$ |
| $\csc x \cot x$ | $-\csc x+C$ |
| $1/x$           | $\ln|x|+C$ |

---

## 📌 Definite Integrals of Common Functions

* $\int_a^b e^x dx = e^b-e^a$  
* $\int_0^\pi \sin x dx = 2$  
* $\int_1^e \tfrac{1}{x} dx = 1$

---

## 📌 Integrating with $u$-Substitution

If $u=g(x)$, then:

$$
\int f(g(x))g'(x)\,dx = \int f(u)\,du
$$

**Example:**

$$
\int 2x(x^2+1)^5 dx \quad u=x^2+1 \quad\implies\quad \int u^5 du = \frac{u^6}{6}+C
$$

---

## 📌 Integrating Using Long Division & Completing the Square

* If degree of numerator $\geq$ denominator, use polynomial long division.  
* Completing the square can simplify quadratics under radicals or denominators.

**Example:**

$$
\int \frac{x^2+1}{x+1}\,dx = \int \Big(x-1+\frac{2}{x+1}\Big)dx = \frac{x^2}{2}-x+2\ln|x+1|+C
$$

---

## 📌 Integrating Using Trigonometric Identities

Use trig identities to simplify:

* $\sin^2x = \frac{1-\cos 2x}{2}$  
* $\cos^2x = \frac{1+\cos 2x}{2}$  
* $\sin x \cos x = \tfrac{1}{2}\sin 2x$

**Example:**

$$
\int \sin^2x\,dx = \int \frac{1-\cos 2x}{2}\,dx = \frac{x}{2}-\frac{\sin 2x}{4}+C
$$

---

## 📌 Proof Videos

(Khan Academy provides detailed proofs for:  
* Fundamental Theorem of Calculus  
* Integration formulas  
* Properties of definite integrals)

---

## ✅ Summary of Topics in Unit 6

* Accumulations of change  
* Riemann sums & summation notation  
* Defining integrals via Riemann sums  
* Fundamental Theorem of Calculus  
* Accumulation functions & interpretation  
* Properties of integrals  
* Reverse power rule  
* Indefinite & definite integrals of common functions  
* $u$-substitution  
* Long division & completing the square  
* Trig identities in integration  
* Proofs of integration theorems

> This file is part of my AI/ML learning journey repo documenting foundational Calculus 1 skills, including step-by-step strategies, worked examples, and formula references.

