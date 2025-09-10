# 📘 Calculus 1 – Unit 2: Derivatives – Definition and Basic Rules

*This file documents concepts and strategies I learned from Khan Academy's Unit 2 of Calculus 1: Derivatives.*

🔗 Source: [Khan Academy – Derivatives](https://www.khanacademy.org/math/calculus-1/cs1-derivatives-intro)

---

## 📌 What is a Derivative?

A **derivative** represents the **instantaneous rate of change** of a function at a specific point. It tells how fast a function's output changes relative to its input.

### 🔹 Instantaneous Slope vs Average Slope

* **Instantaneous slope:** slope of the **tangent line** at a single point.
* **Average slope:** slope of a **secant line** over an interval `[a, b]`.

### 🔹 Secant Line and Slope Formula

The slope of a secant line through points `(x1, f(x1))` and `(x2, f(x2))` is:

```
m = (f(x2) - f(x1)) / (x2 - x1)
```

This slope gives the **average rate of change** over `[x1, x2]`. As `x2 → x1`, it approaches the derivative.

---

## 📐 Tangent Line and Point-Slope Form

The tangent line at `(a, f(a))` has slope `f'(a)` and equation:

```
y - f(a) = f'(a)(x - a)
```

* **Tangent line:** touches curve at one point, slope equals derivative.
* **Secant line:** intersects curve at two points, slope equals average rate of change.

---

## 🔢 Derivative Notations

* **Lagrange:** `f'(x)`
* **Leibniz:** `dy/dx`
* **Newton:** `ȳ` (used in physics)

---

## 🔁 Formal Definition of Derivative

```
f'(a) = lim(h → 0) [(f(a + h) - f(a)) / h]
```

This limit gives the **instantaneous rate of change** at `x = a`.

---

## 🧮 Basic Derivative Rules

* **Constant Rule:** `d/dx[c] = 0`
* **Power Rule:** `d/dx[x^n] = n*x^(n-1)`
* **Constant Multiple Rule:** `d/dx[c*f(x)] = c*f'(x)`
* **Sum/Difference Rule:** `d/dx[f(x) ± g(x)] = f'(x) ± g'(x)`

---

## 🧩 Derivatives of Common Functions

| Function | Derivative      |
| -------- | --------------- |
| sin(x)   | cos(x)          |
| cos(x)   | -sin(x)         |
| tan(x)   | sec^2(x)        |
| cot(x)   | -csc^2(x)       |
| sec(x)   | sec(x)\*tan(x)  |
| csc(x)   | -csc(x)\*cot(x) |
| ln(x)    | 1/x             |

---

## ✖️ Product Rule

```
d/dx[u*v] = u'*v + u*v'
```

## ➗ Quotient Rule

```
d/dx[u/v] = (v*u' - u*v') / v^2
```

## 🔁 Chain Rule

```
d/dx[f(g(x))] = f'(g(x)) * g'(x)
```

---

## 📐 Normal Line

Perpendicular to tangent. If tangent slope is `m`, normal slope is `-1/m`.

---

## ✅ Differentiability and Continuity

* Differentiable ⇒ Continuous
* Continuous ⇏ Differentiable (may have corners/cusps)

---

## 🧪 Example: Polynomial Derivative

```
f(x) = 3x^3 - 5x^2 + 2x - 7
f'(x) = 9x^2 - 10x + 2
```

Slope of tangent line at any x-value is `f'(x)`.

---

## 📈 Visual Summary

* **Secant Line:** average rate of change.
* **Tangent Line:** instantaneous rate of change.
* **Derivative:** slope of tangent line.

---

## ✅ Completed Topics from Khan Academy

* [x] Secant and tangent lines
* [x] Average vs instantaneous rate of change
* [x] Slope formulas
* [x] Derivative definitions and notations
* [x] Formal limit definition
* [x] Basic derivative rules
* [x] Product, quotient, chain rules
* [x] Differentiability and continuity
* [x] Polynomial derivatives
* [x] Trig and logarithmic derivatives
* [x] Tangent and normal lines

---

## 📚 Reference

Khan Academy: [Unit 2 – Derivatives](https://www.khanacademy.org/math/calculus-1/cs1-derivatives-intro)

---

> This file is part of my AI/ML journey repo documenting foundational math skills before diving into machine learning and AI model building.
