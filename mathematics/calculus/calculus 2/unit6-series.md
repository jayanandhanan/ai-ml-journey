# 📘 Calculus 2 – Unit 6: Series

*This file documents concepts, formulas, and strategies I learned from Khan Academy's Calculus 2 unit on Series.*

🔗 Source: [Khan Academy – Series](https://www.khanacademy.org/math/calculus-2/cs2-series)

---

## 📌 Sequences: Convergent and Divergent

A **sequence** is **convergent** if

$$
\lim_{n \to \infty} a_n = L
$$

exists; otherwise, it is **divergent**.

**Example:**

$$
a_n = \frac{1}{n} \to 0 \quad \text{(convergent)}
$$

$$
b_n = (-1)^n \quad \text{(diverges)}
$$

---

## 📌 Partial Sums and Series

The **n-th partial sum** is

$$
S_n = \sum_{k=1}^{n} a_k
$$

A series **converges** if

$$
\lim_{n \to \infty} S_n \text{ exists}
$$

**Example:**

$$
\sum_{n=1}^{\infty} \frac{1}{2^n} = 1
$$

---

## 📌 Geometric Series

A geometric series is of the form:

$$
\sum_{n=0}^{\infty} ar^n
$$

* Converges if $|r|<1$ with sum

$$
S = \frac{a}{1-r}
$$

* Diverges if $|r| \ge 1$

**Example:**

$$
1 + \frac{1}{2} + \frac{1}{4} + \dots = 2
$$

---

## 📌 n-th Term Test for Divergence

If

$$
\lim_{n \to \infty} a_n \neq 0
$$

then the series **diverges**.

**Example:**

$$
\sum_{n=1}^{\infty} \frac{n}{n+1} \text{ diverges}
$$

---

## 📌 Integral Test

For positive, decreasing $f(n) = a_n$:

$$
\sum a_n \text{ converges } \iff \int_1^{\infty} f(x) dx \text{ converges}
$$

**p-Series:**

$$
\sum_{n=1}^{\infty} \frac{1}{n^p} \text{ converges if } p>1
$$

**Harmonic Series:**

$$
\sum_{n=1}^{\infty} \frac{1}{n} \text{ diverges}
$$

---

## 📌 Comparison Tests

**Direct Comparison Test:**

If $0 \le a_n \le b_n$:

* $\sum b_n$ converges $\Rightarrow \sum a_n$ converges
* $\sum a_n$ diverges $\Rightarrow \sum b_n$ diverges

**Limit Comparison Test:**

$$
\lim_{n\to\infty} \frac{a_n}{b_n} = c > 0 \Rightarrow \sum a_n \text{ and } \sum b_n \text{ converge/diverge together}
$$

---

## 📌 Alternating Series Test and Error Bound

Series of the form $\sum (-1)^n b_n$ converges if:

1. $b_n > 0$
2. $b_n$ decreasing
3. $\lim_{n\to\infty} b_n = 0$

**Error Bound:**

$$
|R_n| = |S - S_n| \le b_{n+1}
$$

---

## 📌 Ratio Test

For $\sum a_n$:

$$
L = \lim_{n \to \infty} \left| \frac{a_{n+1}}{a_n} \right|
$$

* $L < 1 \Rightarrow$ converges absolutely
* $L > 1 \Rightarrow$ diverges
* $L = 1 \Rightarrow$ inconclusive

---

## 📌 Absolute and Conditional Convergence

* **Absolute:** $\sum |a_n|$ converges $\Rightarrow \sum a_n$ converges
* **Conditional:** $\sum a_n$ converges but $\sum |a_n|$ diverges

---

## 📌 Taylor and Maclaurin Series

**Maclaurin Series:**

$$
f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(0)}{n!} x^n
$$

**Taylor Series about $a$:**

$$
f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!} (x-a)^n
$$

**Examples:**

$$
e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!}
$$

$$
\sin x = \sum_{n=0}^{\infty} (-1)^n \frac{x^{2n+1}}{(2n+1)!}
$$

$$
\cos x = \sum_{n=0}^{\infty} (-1)^n \frac{x^{2n}}{(2n)!}
$$

$$
\ln(1+x) = \sum_{n=1}^{\infty} (-1)^{n+1} \frac{x^n}{n}
$$

**Euler's Formula:**

$$
e^{ix} = \cos x + i \sin x
$$

**Euler's Identity:**

$$
e^{i\pi} + 1 = 0
$$

---

## 📌 Lagrange Error Bound

If approximating with $n$ terms:

$$
|R_n(x)| \le \frac{M |x-a|^{n+1}}{(n+1)!}
$$

where $M$ is the maximum of $|f^{(n+1)}(x)|$ on the interval.

---

## 📌 Power Series and Function Representations

* **Geometric Representation:**

$$
\frac{1}{1-x} = \sum_{n=0}^{\infty} x^n, \quad |x| < 1
$$

* **Substitutions:** e.g., $\arctan(2x)$
* **Differentiating/Integrating Series:**

$$
\frac{d}{dx} \sum_{n=0}^{\infty} c_n x^n = \sum_{n=1}^{\infty} n c_n x^{n-1}, \quad \int \sum_{n=0}^{\infty} c_n x^n dx = \sum_{n=0}^{\infty} \frac{c_n x^{n+1}}{n+1}
$$

* **Interval of Convergence:** Check endpoints separately after differentiation/integration

---

## 📌 Telescoping Series

Series of the form:

$$
\sum_{n=1}^{\infty} (a_n - a_{n+1}) = a_1 - \lim_{n\to\infty} a_{n+1}
$$

**Example:**

$$
\sum_{n=1}^{\infty} \frac{1}{n(n+1)} = 1
$$

---

## ✅ Topics Covered

* [x] Convergent/divergent sequences
* [x] Partial sums
* [x] Series as limit of partial sums
* [x] Geometric series
* [x] n-th term test
* [x] Integral test
* [x] Harmonic and p-series
* [x] Comparison and limit comparison tests
* [x] Alternating series test
* [x] Alternating series error bound
* [x] Ratio test
* [x] Absolute and conditional convergence
* [x] Taylor and Maclaurin series
* [x] Lagrange error bound
* [x] Power series and substitutions
* [x] Euler's formula and identity
* [x] Differentiating/integrating power series
* [x] Interval of convergence
* [x] Telescoping series

---


> This file is formatted exactly like Unit 5 and is part of an AI/ML journey repository documenting all foundational Calculus 2 series topics.

