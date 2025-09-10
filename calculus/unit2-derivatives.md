# 📘 Calculus 1 – Unit 2: Derivatives – Definition and Basic Rules

*This file documents concepts and strategies I learned from Khan Academy's Unit 2 of Calculus 1: Derivatives – Definition and Basic Rules.*

🔗 Source: [Khan Academy – Derivatives – Definition and Basic Rules](https://www.khanacademy.org/math/calculus-1/cs1-derivatives-definition-and-basic-rules)

---

## 📌 What is a Derivative?

A **derivative** represents the **instantaneous rate of change** of a function at a specific point. It provides the slope of the tangent line to the function's graph at that point.

**Mathematical Definition:**

The derivative of a function $f(x)$ at a point $x = a$ is defined as:

$$
f'(a) = \lim_{h \to 0} \frac{f(a+h) - f(a)}{h}
$$

This is known as the **difference quotient**.

---

## 🔍 Average vs. Instantaneous Rate of Change

* **Average Rate of Change**: Measures the change in the function's value over an interval $[a, b]$:

  $$
  \frac{f(b) - f(a)}{b - a}
  $$

* **Instantaneous Rate of Change**: Represents the rate at which the function's value changes at a specific point, equivalent to the slope of the tangent line at that point.

---

## 📏 Secant Line and Slope

* **Secant Line**: A line that intersects a curve at two points. Its slope represents the average rate of change between those two points.

* **Tangent Line**: A line that touches the curve at exactly one point. Its slope represents the instantaneous rate of change at that point.

---

## 🧮 Derivative Notations

Different notations are used to represent derivatives:

* **Lagrange Notation**: $f'(x)$
* **Leibniz Notation**: $\frac{dy}{dx}$
* **Newton Notation**: $\dot{y}$

---

## 📐 Tangent Line Equation

The equation of a tangent line at a point $(a, f(a))$ is given by:

$$
y - f(a) = f'(a)(x - a)
$$

This is the **point-slope form** of the line.

---

## 📈 Derivative as Slope of Curve

The derivative at a point gives the slope of the tangent line to the curve at that point, indicating how steep the curve is at that specific location.

---

## 🔄 Average Rate of Change Formula

The average rate of change of a function $f(x)$ over the interval $[a, b]$ is:

$$
\frac{f(b) - f(a)}{b - a}
$$

---

## 📘 Power Rule and Basic Derivative Rules

* **Power Rule**: For $f(x) = x^n$, the derivative is:

  $$
  $$

f'(x) = nx^{n-1}
]

* **Constant Rule**: The derivative of a constant is 0.
* **Constant Multiple Rule**: The derivative of $c \cdot f(x)$ is $c \cdot f'(x)$.
* **Sum/Difference Rule**: The derivative of $f(x) + g(x)$ is $f'(x) + g'(x)$, and similarly for subtraction.

---

## 📊 Differentiating Polynomials

To differentiate a polynomial:

1. Apply the power rule to each term.
2. Combine the results.

**Example**:

For $f(x) = 3x^3 + 2x^2 - x + 5$,

$$
f'(x) = 9x^2 + 4x - 1
$$

Slope of tangent line at any x-value is $f'(x)$.

---

## 🔢 Derivatives of Trigonometric Functions

* $\frac{d}{dx}(\sin x) = \cos x$
* $\frac{d}{dx}(\cos x) = -\sin x$
* $\frac{d}{dx}(\tan x) = \sec^2 x$
* $\frac{d}{dx}(\cot x) = -\csc^2 x$
* $\frac{d}{dx}(\sec x) = \sec x \tan x$
* $\frac{d}{dx}(\csc x) = -\csc x \cot x$

---

## 📈 Product and Quotient Rules

* **Product Rule**: For $f(x) = u(x) \cdot v(x)$,

  $$
  $$

f'(x) = u'(x)v(x) + u(x)v'(x)
]

* **Quotient Rule**: For $f(x) = \frac{u(x)}{v(x)}$,

  $$
  $$

f'(x) = \frac{v(x)u'(x) - u(x)v'(x)}{(v(x))^2}
]

---

## 📐 Slope of Normal Line

The slope of the **normal line** to a curve at a point is the negative reciprocal of the slope of the tangent line at that point:

$$
m_{\text{normal}} = -\frac{1}{m_{\text{tangent}}}
$$

---

## ✅ Completed Topics from Khan Academy

* [x] Average and instantaneous rate of change
* [x] Secant and tangent lines
* [x] Derivative notations
* [x] Tangent line equation
* [x] Derivative as slope of curve
* [x] Power and basic derivative rules
* [x] Differentiating polynomials
* [x] Derivatives of trigonometric functions
* [x] Product and quotient rules
* [x] Slope of normal line

---

## 📚 Reference

Khan Academy: [Unit 2 – Derivatives – Definition and Basic Rules](https://www.khanacademy.org/math/calculus-1/cs1-derivatives-definition-and-basic-rules)

---

> This file is part of my AI/ML journey repo documenting foundational math skills before diving into machine learning and AI model building.
