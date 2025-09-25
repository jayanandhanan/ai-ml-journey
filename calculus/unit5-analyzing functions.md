# 📘 Calculus 1 – Unit 5: Analyzing Functions

*This file documents concepts, strategies, and examples from Khan Academy's Unit on Analyzing Functions.*

🔗 Source: [Khan Academy – Analyzing Functions](https://www.khanacademy.org/math/calculus-1/cs1-analyzing-functions)

---

## 📌 Mean Value Theorem (MVT)

* If a function $f$ is **continuous** on $[a,b]$ and **differentiable** on $(a,b)$, then there exists $c \in (a,b)$ such that:

$$
f'(c) = \frac{f(b)-f(a)}{b-a}
$$

*Example:*

$$
f(x)=x^2,\ [1,3] \implies f'(c) = \frac{f(3)-f(1)}{3-1} = \frac{9-1}{2} = 4 \implies c=2
$$

---

## 📌 Extreme Value Theorem and Critical Points

* **Extreme Value Theorem:** If $f$ is **continuous** on a closed interval $[a,b]$, it has both a **maximum** and **minimum**.
* **Critical points:** Points where $f'(x)=0$ or $f'(x)$ is undefined.

**Example:** $f(x) = x^3 - 3x^2 + 2$

* $f'(x) = 3x^2 - 6x = 3x(x-2)$ → critical points at $x=0,2$.
* Evaluate $f(0), f(2), f(a), f(b)$ to find absolute extrema.

---

## 📌 Intervals of Increase and Decrease

* **Increasing:** $f'(x) > 0$
* **Decreasing:** $f'(x) < 0$

**Example:** $f(x) = x^3 - 3x^2$

* $f'(x) = 3x^2 - 6x = 3x(x-2)$
* Increasing: $(-\infty,0)\cup(2,\infty)$
* Decreasing: $(0,2)$

---

## 📌 Relative (Local) Extrema

* **Local Maximum:** $f'(x)=0$ and $f'$ changes from $+ \to -$
* **Local Minimum:** $f'(x)=0$ and $f'$ changes from $- \to +$

**Example Table:**

| Interval      | $f'(x)$ | Graph Behavior |
| ------------- | ------- | -------------- |
| $(-\infty,0)$ | $+$     | Increasing     |
| $(0,2)$       | $-$     | Decreasing     |
| $(2,\infty)$  | $+$     | Increasing     |

* Local min at $x=2$, local max at $x=0$.

---

## 📌 Absolute (Global) Extrema

* Evaluate $f$ at **critical points** and **endpoints** of a closed interval.
* Maximum and minimum values are the **absolute extrema**.

**Example:** $f(x)=x^3-3x^2$ on $[0,3]$

* Critical points: $x=0,2$
* Evaluate $f(0)=0, f(2)=-4, f(3)=0$ → Absolute min $-4$, Absolute max $0$

---

## 📌 Concavity and Inflection Points

* **Concave Up:** $f''(x) > 0$ → graph curves upward, slope $f'(x)$ increasing.
* **Concave Down:** $f''(x) < 0$ → graph curves downward, slope $f'(x)$ decreasing.
* **Inflection Points:** Points where $f''(x)=0$ and concavity changes.

**Example Table:**

| Interval      | $f'(x)$    | $f''(x)$ | Graph Concavity |
| ------------- | ---------- | -------- | --------------- |
| $(-\infty,1)$ | Increasing | $+$      | Concave up      |
| $(1,3)$       | Decreasing | $-$      | Concave down    |

**Graphical Representation:**

* Concave up: cup-shaped
* Concave down: upside-down cup
* Inflection: where concavity changes

---

## 📌 Second Derivative Test

* If $f'(c)=0$:

  * $f''(c)>0$ → local minimum
  * $f''(c)<0$ → local maximum
  * $f''(c)=0$ → test inconclusive, check higher derivatives or sign changes

**Example:** $f(x)=x^3-3x^2$

* $f'(x)=3x(x-2)$ → $f'(0)=0$, $f'(2)=0$
* $f''(x)=6x-6$, $f''(0)=-6<0$ → local max at $x=0$
* $f''(2)=6>0$ → local min at $x=2$

---

## 📌 Sketching Curves

Steps:

1. Find **domain**
2. Find **intercepts**
3. Find **critical points**
4. Determine **intervals of increase/decrease**
5. Find **inflection points** and **concavity**
6. Evaluate **endpoints** (if closed interval)
7. Sketch with concavity and extrema in mind

**Example Sketch Table:**

| x  | f(x) | f'(x) | f''(x) | Behavior                 |
| -- | ---- | ----- | ------ | ------------------------ |
| -1 | ...  | +     | +      | Increasing, concave up   |
| 0  | ...  | 0     | -      | Max, concave down        |
| 1  | ...  | -     | -      | Decreasing, concave down |
| 2  | ...  | 0     | +      | Min, concave up          |

---

## 📌 Connecting $f$, $f'$, and $f''$

* **f'** indicates slope of $f$ → increasing/decreasing
* **f''** indicates slope of $f'$ → concavity
* **Summary:**

  * $f'>0$ → $f$ increasing
  * $f'<0$ → $f$ decreasing
  * $f''>0$ → $f$ concave up
  * $f''<0$ → $f$ concave down

**Example Graphs:**

* $f(x)=x^3-3x^2$
* $f'(x)=3x^2-6x$
* $f''(x)=6x-6$

---

## 📌 Solving Optimization Problems

1. Identify **objective function**
2. Determine **constraints**
3. Find **derivative**, set $f'(x)=0$
4. Determine **max/min** via first or second derivative test

**Example:** Max area of rectangle under parabola $y=9-x^2$

* $R(x)=2x \cdot y = 2x(9-x^2) = 18x-2x^3$
* $R'(x)=18-6x^2=0 \implies x=\sqrt{3}$
* Maximum area occurs at $x=\sqrt{3}$

---

## 📌 Analyzing Implicit Relations

* For equations not solved for $y$, use **implicit differentiation**:

$$
F(x,y)=0 \implies \frac{dy}{dx}=-\frac{F_x}{F_y}
$$

**Example:**

$x^2+4y^2=7+3xy$
$\frac{dy}{dx} = \frac{3y-2x}{8y-3x}$

---

## ✅ Summary of Topics in Unit 5

* Mean Value Theorem
* Extreme Value Theorem & Critical Points
* Intervals of Increase/Decrease
* Relative (Local) Extrema
* Absolute (Global) Extrema
* Concavity & Inflection Points
* Second Derivative Test
* Sketching Curves
* Connecting $f$, $f'$, $f''$
* Optimization Problems
* Analyzing Implicit Relations

> This file is part of my AI/ML learning journey repo documenting foundational Calculus 1 skills, including pictorial representations and tables linking $f$, $f'$, and $f''$.
