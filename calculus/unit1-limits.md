# 📘 Calculus 1 – Unit 1: Limits and Continuity

*This file documents concepts and strategies I learned from Khan Academy's Unit 1 of Calculus 1: Limits and Continuity.*

🔗 Source: [Khan Academy – Limits and Continuity](https://www.khanacademy.org/math/calculus-1/cs1-limits-and-continuity)

---

## 📌 What is a Limit?

A **limit** is the value that a function $f(x)$ approaches as $x$ approaches some value $c$:

$$
\lim_{x \to c} f(x) = L
$$

**Example:**  
$f(x) = \frac{x - 1}{x - 1}$  
- At $x = 1$, this becomes $0/0$, which is undefined.  
- But using the **limit** $\lim_{x \to 1} f(x)$, we analyze values of $x$ approaching 1 from both sides.

---

## 🔍 Left-Hand and Right-Hand Limits

A limit exists **only if** both one-sided limits exist and are equal:  

$$
\lim_{x \to a^-} f(x) = \lim_{x \to a^+} f(x) \implies \lim_{x \to a} f(x) \text{ exists}
$$

---

## 🧮 Limit Properties

If $\lim_{x \to a} f(x) = L$ and $\lim_{x \to a} g(x) = M$, then:  
- $\lim_{x \to a} [f + g](x) = L + M$  
- $\lim_{x \to a} [f \cdot g](x) = L \cdot M$  
- $\lim_{x \to a} \frac{f(x)}{g(x)} = \frac{L}{M}$, if $M \neq 0$

---

## 🔁 Limits of Composite Functions

$$
\lim_{x \to a} f(g(x)) = f\Big(\lim_{x \to a} g(x)\Big)
$$
> When $f$ is continuous at $\lim g(x)$

---

## 🧠 Strategies to Find Limits

1. **Try direct substitution**:  
   - If $f(a) = b/0$, suspect a vertical asymptote.  
   - If $f(a) = b$, you're done!  

2. **Indeterminate form $0/0$**: Try:  
   - Factoring  
   - Rationalizing (conjugates)  
   - Trig identities  
   - Algebraic simplification  

---

## ✂️ Squeeze Theorem

Used when a function is trapped between two others:  

If $f(x) \le g(x) \le h(x)$, and both outer limits equal $L$, then:  
$$
\lim_{x \to a} g(x) = L
$$

---

## 📈 Piecewise Functions

A piecewise function may have a limit $L$ at $x = c$, but the **function value** $f(c) \ne L$.  
This causes a **removable discontinuity**.

---

## 🧩 Discontinuities

Types of discontinuity at $x = c$:  
- **Removable**: limit exists, but $f(c)$ is undefined or different  
- **Jump**: left and right-hand limits are not equal  
- **Infinite**: function approaches $\infty$ or $-\infty$  

---

## 🔄 Continuity

### Continuity at a point $c$:  
A function $f(x)$ is continuous at $c$ if:  
1. $f(c)$ is defined  
2. $\lim_{x \to c} f(x)$ exists  
3. $\lim_{x \to c} f(x) = f(c)$  

### Continuity over an interval:  
If a function is continuous at **every point** in the interval.

---

## 🔧 Removing Discontinuity (Example)

Given:  
$$
f(x) = \frac{x^2 - 9}{x - 3} = \frac{(x - 3)(x + 3)}{x - 3} = x + 3, \quad x \ne 3
$$

- The function has a **removable discontinuity** at $x = 3$  
- Define $f(3) = 6$ to make it continuous

---

## 🔭 Infinite Limits & Limits at Infinity

### Infinite Limit:  
$$
\lim_{x \to a} f(x) = \infty
$$
⇒ Vertical asymptote at $x = a$

### Limit at Infinity:  
$$
\lim_{x \to \infty} \frac{1}{x} = 0
$$
⇒ Horizontal asymptote at $y = 0$

---

## 📏 Delta-Epsilon Definition

For a formal proof:  
$$
\lim_{x \to c} f(x) = L \iff \forall \epsilon > 0, \exists \delta > 0 \text{ such that } 0 < |x - c| < \delta \implies |f(x) - L| < \epsilon
$$

---

## 📍 Intermediate Value Theorem

If $f$ is continuous on $[a, b]$ and $N$ is between $f(a)$ and $f(b)$,  
then there exists $c \in [a, b]$ such that:  
$$
f(c) = N
$$

---

## ✅ Completed Topics from Khan Academy

* [x] Estimating limits  
* [x] One-sided limits  
* [x] Infinite limits  
* [x] Limits at infinity  
* [x] Formal definition with epsilon-delta  
* [x] Continuity  
* [x] Intermediate value theorem  
* [x] Discontinuities and fixing them

---

## 📚 Reference

Khan Academy: [Unit 1 – Limits and Continuity](https://www.khanacademy.org/math/calculus-1/cs1-limits-and-continuity)

---

> This file is part of my AI/ML journey repo documenting foundational math skills before diving into machine learning and AI model building.
