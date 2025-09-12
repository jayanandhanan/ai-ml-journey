# 📘 Calculus 1 – Unit 3: Chain Rule and Other Advanced Topics

*This file documents concepts and strategies I learned from Khan Academy's Unit 3 of Calculus 1: Chain Rule and Other Advanced Topics.*

---

## 📌 Chain Rule

The **chain rule** allows you to differentiate **composite functions**.

If $y = f(g(x))$, then:

$$
\frac{dy}{dx} = f'\bigl(g(x)\bigr) \cdot g'(x)
$$

* **f'(g(x))**: derivative of the outer function evaluated at the inner function
* **g'(x)**: derivative of the inner function

**Example:**
$y = \sin(3x^2)$

* Inner function: $g(x) = 3x^2$
* Outer function: $f(u) = \sin(u)$

$$
\frac{dy}{dx} = \cos(3x^2) \cdot 6x = 6x\cos(3x^2)
$$

---

## 🔍 Identifying Composite Functions

* **Composite function:** $f(g(x))$
* Example: $h(x) = \sqrt{5x + 3}$

  * Inner: $g(x) = 5x + 3$
  * Outer: $f(u) = \sqrt{u}$

---

## 📈 Derivatives of Exponential and Logarithmic Functions

* $\frac{d}{dx} e^{x} = e^x$
* $\frac{d}{dx} a^x = a^x \ln(a)$, $a > 0$
* $\frac{d}{dx} \ln(x) = 1/x$, $x>0$
* **Composite example:** $y = e^{3x^2}$

$$
\frac{dy}{dx} = e^{3x^2} \cdot 6x = 6x e^{3x^2}
$$

* **Composite ln example:** $y = \ln(2x^3 + 1)$

$$
\frac{dy}{dx} = \frac{6x^2}{2x^3 + 1}
$$

---

## 🔄 Implicit Differentiation

Used when $y$ is not isolated:

**Example:** $x^2 + y^2 = 25$

$$
2x + 2y \frac{dy}{dx} = 0 \implies \frac{dy}{dx} = -\frac{x}{y}
$$

---

## 🔑 Applications of Chain Rule

* **Slope of tangent line** at a point:

  * Find $\frac{dy}{dx}$ using chain rule or implicit differentiation
  * Use point-slope formula: $y - y_0 = m(x - x_0)$

---

## 🔢 Derivatives of Inverse Functions

* If $f$ and $g$ are inverses:

$$
f(g(x)) = x \implies f'(g(x)) \cdot g'(x) = 1
$$

$$
g'(x) = \frac{1}{f'(g(x))}
$$

* Another formula: If $y = f^{-1}(x)$ and $x = f(y)$

$$
\frac{dy}{dx} = \frac{1}{f'(y)}
$$

---

## 🔢 Derivatives of Inverse Trig Functions

* $\frac{d}{dx} \arcsin(x) = \frac{1}{\sqrt{1 - x^2}}$
* $\frac{d}{dx} \arccos(x) = -\frac{1}{\sqrt{1 - x^2}}$
* $\frac{d}{dx} \arctan(x) = \frac{1}{1 + x^2}$
* **Composite example:** $y = \arcsin(3x)$

$$
\frac{dy}{dx} = \frac{3}{\sqrt{1 - 9x^2}}
$$

---

## 🔢 Differentiating Using Multiple Rules

* **Product of >2 functions:**

$$
\frac{d}{dx}[u \cdot v \cdot w] = u'vw + uv'w + uvw'
$$

* **Quotient Rule for composite functions** applies similarly:

$$
\frac{d}{dx}\left[\frac{u(x)}{v(x)}\right] = \frac{u'v - uv'}{v^2}
$$

---

## 📐 Second Derivatives

* For $y = f(x)$, second derivative:

$$
\frac{d^2y}{dx^2} = \frac{d}{dx}\left(\frac{dy}{dx}\right)
$$

* **Implicit example:** $x^2 + y^2 = 1$
  $\frac{dy}{dx} = -\frac{x}{y}$

$$
\frac{d^2y}{dx^2} = -\frac{y - (-x)(dy/dx)}{y^2} = -\frac{y^2 + x^2}{y^3} = -\frac{1}{y^3}
$$

---

## 🔢 Composite Exponential Functions

* Example: $y = (3x^2)^{x^3}$
* Take natural log: $\ln y = x^3 \ln(3x^2)$
* Differentiate implicitly using chain and product rules

---

## ✅ Completed Topics from Khan Academy

* Chain Rule
* Identifying composite functions
* Derivatives of exponential and logarithmic functions
* Implicit differentiation
* Applications: slope of tangent line
* Derivatives of inverse functions
* Derivatives of inverse trig functions
* Differentiating using multiple rules
* Second derivatives (including implicit)
* Composite exponential function differentiation

---

## 📚 Reference

Khan Academy: [Unit 3 – Chain Rule and Other Advanced Topics](https://www.khanacademy.org/math/calculus-1/cs1-derivatives-chain-rule-and-other-advanced-topics)

---

> This file is part of my AI/ML journey repo documenting foundational math skills before diving into machine learning and AI model building.
