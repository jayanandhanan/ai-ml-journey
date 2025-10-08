# 📘 Calculus 2 – Unit 3: Differential Equations

*This file documents concepts and strategies I reviewed from Khan Academy's Unit 3 of Calculus 2: Differential Equations.*

🔗 Source: [Khan Academy – Differential Equations](https://www.khanacademy.org/math/calculus-2/cs2-differential-equations)

---

## 📌 Overview

This unit introduces **differential equations** and their applications. It revisits many concepts from **Calculus 1 – Unit 7: Differential Equations**, including slope fields, separation of variables, and particular solutions, and adds new topics like **logistic models** and **Euler’s method** for numerical approximations.

---

## ✅ Topics Reviewed

* [x] Introduction to differential equations  
* [x] Verifying solutions for differential equations  
* [x] Sketching slope fields  
* [x] Reasoning using slope fields  
* [x] Separation of variables  
* [x] Particular solutions to differential equations  
* [x] Exponential growth and decay models  

### 🔹 New Topics in Calculus 2 Unit 3

* [x] Logistic models  
* [x] Euler’s method for approximating solutions  

---

## 📌 Differential Equations — Key Concepts

A **differential equation** relates a function $y(x)$ to its derivative $y'(x)$:

$$
\frac{dy}{dx} = f(x,y)
$$

**Solution:** A function $y(x)$ satisfying the equation.

**Verifying a solution:** Substitute $y(x)$ and its derivative into the differential equation and check equality.

---

## 📌 Logistic Models

Accounts for **limited resources**. Differential equation:

$$
\frac{dP}{dt} = rP\left(1-\frac{P}{K}\right)
$$

- $P(t)$: population at time $t$  
- $r$: growth rate  
- $K$: carrying capacity  

**Solution:**

$$
P(t) = \frac{K}{1 + \left(\frac{K-P_0}{P_0}\right)e^{-rt}}
$$

**Example:**

Initial population $P_0 = 100$, $K = 500$, $r = 0.1$:

$$
P(t) = \frac{500}{1 + 4 e^{-0.1 t}}
$$

---

## 📌 Euler’s Method

Numerical approximation of solutions:

- Step size $h$  
- Recurrence:

$$
y_{n+1} = y_n + h f(x_n, y_n)
$$

**Example:**

$$
\frac{dy}{dx} = y, \quad y(0)=1 \, h=0.1
$$

- $y_1 = y_0 + 0.1 y_0 = 1 + 0.1 = 1.1$  
- $y_2 = 1.1 + 0.1(1.1) = 1.21$  
- Continue iteratively  

---

## 🔗 Reference

For detailed explanations, examples, and derivations, see:

👉 [Calculus 1 – Unit 7: Differential Equations](../calculus%201/unit7-differential%20equations.md)

---

> This file is part of my AI/ML journey repo documenting foundational math skills before diving into machine learning and AI.

