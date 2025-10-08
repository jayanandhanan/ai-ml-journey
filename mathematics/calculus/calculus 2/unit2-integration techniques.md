# 📘 Calculus 2 – Unit: Integration Techniques

*This file documents concepts and strategies I learned from Khan Academy's Calculus 2 unit on Integration Techniques.*

🔗 Source: [Khan Academy – Integration Techniques](https://www.khanacademy.org/math/calculus-2/cs2-integration-techniques)

---

## 📌 Integrating with $u$-Substitution

Let $u = g(x)$, then $du = g'(x)\,dx$.

**Example:**

$$
\int 2x e^{x^2} dx,\quad u=x^2, \, du=2x dx
$$

$$
\int e^u du = e^u + C = e^{x^2}+C
$$

---

## 📌 Integrating Using Long Division and Completing the Square

**Long division:** use when $\deg(\text{numerator}) \ge \deg(\text{denominator})$.

**Completing the square:** transforms quadratic denominators for $\arctan$ or $\ln$ integrals.

**Example:**

$$
\int \frac{1}{x^2-14x+58} dx
$$

Complete the square: 

$$
x^2-14x+58=(x-7)^2+9
$$

$$
\int \frac{1}{(x-7)^2+3^2} dx = \frac{1}{3}\arctan\left(\frac{x-7}{3}\right) + C
$$

---

## 📌 Integrating Using Trigonometric Identities

- $\sin^2(x) = \frac{1-\cos(2x)}{2}$  
- $\cos^2(x) = \frac{1+\cos(2x)}{2}$  
- $\sin(x)\cos(x) = \frac{1}{2}\sin(2x)$  

**Example:**

$$
\int \sin^2(x) dx = \int \frac{1-\cos(2x)}{2} dx = \frac{x}{2} - \frac{\sin(2x)}{4} + C
$$

---

## 📌 Trigonometric Substitution

Use substitution for integrals of the form:

- $\sqrt{a^2 - x^2} \to x = a\sin\theta$  
- $\sqrt{a^2 + x^2} \to x = a\tan\theta$  
- $\sqrt{x^2 - a^2} \to x = a\sec\theta$  

**Example:**

$$
\int \frac{dx}{\sqrt{4-x^2}} \quad\text{let } x = 2\sin\theta, \, dx = 2\cos\theta d\theta
$$

$$
\int \frac{2\cos\theta d\theta}{\sqrt{4-4\sin^2\theta}} = \int d\theta = \theta + C = \arcsin\frac{x}{2}+C
$$

---

## 📌 Integration by Parts

Formula:

$$
\int u\, dv = uv - \int v\, du
$$

**Example:**

$$
\int x e^x dx
$$

Let $u = x$, $dv = e^x dx \implies du = dx, \, v = e^x$:

$$
\int x e^x dx = x e^x - \int e^x dx = x e^x - e^x + C
$$

---

## 📌 Integrating Using Linear Partial Fractions

If:

$$
\frac{P(x)}{(x-a)(x-b)} = \frac{A}{x-a} + \frac{B}{x-b}
$$

Solve for $A, B$ then integrate each term.

**Example:**

$$
\int \frac{3x+1}{x(x+1)} dx = \int \frac{1}{x} dx + \int \frac{2}{x+1} dx = \ln|x| + 2\ln|x+1| + C
$$

---

## 📌 Improper Integrals

For integrals with infinite limits or discontinuities:

- Infinite upper limit:

$$
\int_a^{\infty} f(x) dx = \lim_{b \to \infty} \int_a^b f(x) dx
$$

- Infinite lower limit:

$$
\int_{-\infty}^{b} f(x) dx = \lim_{a \to -\infty} \int_a^b f(x) dx
$$

- Discontinuity at $c \in [a,b]$:

$$
\int_a^b f(x) dx = \lim_{t \to c^-} \int_a^t f(x) dx + \lim_{t \to c^+} \int_t^b f(x) dx
$$

**Example:**

$$
\int_1^\infty \frac{1}{x^2} dx = \lim_{b \to \infty} \left[-\frac{1}{x}\right]_1^b = 1
$$

---

## ✅ Topics Covered in this Unit

* [x] Integrating with $u$-substitution  
* [x] Integrating using long division & completing the square  
* [x] Integrating using trigonometric identities  
* [x] Trigonometric substitution  
* [x] Integration by parts  
* [x] Integrating using linear partial fractions  
* [x] Improper integrals  

---

> This file is part of my AI/ML journey repo documenting foundational math skills before diving into machine learning and AI.
