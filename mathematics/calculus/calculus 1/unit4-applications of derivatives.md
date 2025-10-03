# 📘 Calculus 1 – Unit 4: Applications of Derivatives

*This file documents concepts and strategies I learned from Khan Academy's Unit on Applications of Derivatives.*

🔗 Source: [Khan Academy – Applications of Derivatives](https://www.khanacademy.org/math/calculus-1/cs1-applications-of-derivatives)

---

## 📌 Meaning of the Derivative in Context

* The derivative represents the **instantaneous rate of change** of a function with respect to its variable.
* Example: If $B(t)$ represents bear population over time:

$$
B(t) = 2190 e^{-0.3 t} \implies B'(t) = -657 e^{-0.3 t}
$$

* Interpretation: $B'(2) \approx -361$ bears/year → population decreasing at 361 bears/year at $t=2$ years.

---

## 🚗 Straight-Line Motion

* **Position function:** $s(t)$
* **Velocity:** $v(t) = s'(t)$
* **Acceleration:** $a(t) = v'(t) = s''(t)$

**Example:**

A particle moves along the x-axis with

$$
v(t) = t^3 - 3t^2 - 8t + 3
$$

Find $v(4)$ and $a(4)$:

$$
v(4) = 64 - 48 - 32 + 3 = -13
$$

$$
a(t) = 3t^2 - 6t - 8 \implies a(4) = 48 - 24 - 8 = 16
$$

*Speeding up or slowing down?* Check signs of $v$ and $a$.

---

## 🔢 Non-Motion Applications of Derivatives

* Related to **growth, decay, or changing quantities**.
* Example: Area of triangle with base $b$ and height $h$:

$$
A = \frac{1}{2} b h \implies \frac{dA}{dt} = \frac{1}{2} \left( b \frac{dh}{dt} + h \frac{db}{dt} \right)
$$

*Example:* Base decreasing at 13 mm/min, height increasing at 6 mm/min, base 5 mm, height 1 mm:

$$
\frac{dA}{dt} = \frac{1}{2}(5 \cdot 6 + 1 \cdot (-13)) = 8.5\, \text{mm²/min}
$$

---

## 🔄 Introduction to Related Rates

* Start with **formula relating quantities**
* Differentiate both sides w\.r.t time $t$
* Substitute known values to solve for unknown rate

**Example:** Ladder problem

$$
20^2 = x^2 + y^2
$$

Given $rac{dy}{dt} = -8$, $y = 12$, find $rac{dx}{dt}$:

$$
2x \frac{dx}{dt} + 2y \frac{dy}{dt} = 0 \implies \frac{dx}{dt} = -\frac{y}{x} \frac{dy}{dt} = 6\, \text{m/min}
$$

---

## 📈 Solving Related Rates Problems

* **Step 1:** Write equation linking variables
* **Step 2:** Differentiate implicitly w\.r.t time
* **Step 3:** Substitute known values
* **Step 4:** Solve for unknown rate

**Example:** Cylinder volume changing

$$
V = \pi r^2 h,\quad h \text{ constant}, \frac{dV}{dt} = 10\pi, h=5
$$

$$
\frac{dr}{dt} = \frac{dV/dt}{2\pi r h} = \frac{10\pi}{2 \pi \cdot 4 \cdot 5} = \frac{1}{4}
$$

Surface area rate:

$$
S = 2\pi r^2 + 2\pi r h \implies \frac{dS}{dt} = (4\pi r + 2\pi h) \frac{dr}{dt} = \frac{13\pi}{2}\,\text{m²/h}
$$

---

## 🔢 Approximation with Local Linearity

* **Linear approximation:**

$$
L(x) = f(a) + f'(a)(x-a)
$$

*Example:* $h(-6)=2, h'(-6)=-1$

$$
L(-6.2) = 2 + (-1)(-0.2) = 1.8\quad \text{(check carefully with sign)}
$$

*Interpretation:* Approximates value of $h$ near $x=-6$

---

## 🔢 L’Hôpital’s Rule

* Used for **0/0** or **∞/∞** indeterminate forms

$$
\lim_{x \to a} \frac{f(x)}{g(x)} = \lim_{x \to a} \frac{f'(x)}{g'(x)} \text{ if limit exists}
$$

**Example:**

$$
\lim_{x \to 0} \frac{\sin x}{5x + 3\sin x} = \frac{\cos 0}{5 + 3\cos 0} = \frac{1}{8}
$$

---

## 🔢 L’Hôpital’s Rule: Composite Exponential Functions

**Example:**

$$
\lim_{x \to \infty} (1 + 5 e^x)^{1/x} = e^{\lim_{x \to \infty} \frac{\ln(1+5e^x)}{x}} = e^5
$$

**Steps:**

1. Take natural log: $\ln L = \lim \frac{\ln(f(x))}{g(x)}$
2. Apply L’Hôpital’s rule if 0/0 or ∞/∞
3. Exponentiate to recover original limit

---

## ✅ Summary of Topics in Unit 4

* Meaning of derivatives in context
* Straight-line motion (position, velocity, acceleration)
* Non-motion applications
* Related rates: introduction and solving problems
* Approximation with local linearity
* L’Hôpital’s rule (including composite exponential forms)
* Examples of derivatives of exponentials, logs, and chain rule applications

---

---

> This file is part of my AI/ML journey repo documenting foundational math skills before diving into machine learning and AI.

