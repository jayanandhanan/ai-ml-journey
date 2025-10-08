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

## 📌 Verifying Solutions

To check if a function is a solution:

1. Compute the derivative $y'(x)$.  
2. Substitute $y(x)$ and $y'(x)$ into the differential equation.  
3. If both sides are equal, the function is a solution.

- **Example:** Verify $y=e^{2x}$ is a solution of $\frac{dy}{dx}=2y$.

$$
y' = 2e^{2x}, \quad 2y = 2e^{2x} \implies y' = 2y
$$

✅ True, so it is a solution.

---

## 📌 Slope Fields

A **slope field** is a graphical representation of a differential equation:

$$
\frac{dy}{dx} = f(x,y)
$$

- At each point $(x,y)$, draw a small line segment with slope $f(x,y)$.  
- Helps visualize solution curves without solving the equation.

- **Example:** For $\frac{dy}{dx} = x - y$, slopes decrease as $y$ increases.

---

## 📌 Reasoning Using Slope Fields

- Observe slopes to predict behavior of solutions.  
- Solution curves follow tangent lines in the slope field.

- **Example:** For $\frac{dy}{dx} = y$, slopes increase as $y$ increases → solutions grow exponentially.

---

## 📌 Separation of Variables

Used for **separable differential equations**:

$$
\frac{dy}{dx} = g(x)h(y)
$$

**Steps:**

1. Rearrange:

$$
\frac{dy}{h(y)} = g(x) dx
$$

2. Integrate both sides:

$$
\int \frac{1}{h(y)} dy = \int g(x) dx
$$

3. Solve for $y$.

- **Example:** Solve $\frac{dy}{dx} = 2y, \ y(0)=3$

$$
\frac{dy}{y} = 2 dx \implies \int \frac{dy}{y} = \int 2 dx
$$

$$
\ln|y| = 2x + C \implies y = 3 e^{2x}
$$

---

## 📌 Particular Solutions

A **particular solution** satisfies an **initial condition**.

- **Example:** Solve $\frac{dy}{dx} = -3y, \ y(1)=4$

$$
\frac{dy}{y} = -3 dx \implies \int \frac{dy}{y} = \int -3 dx
$$

$$
\ln|y| = -3x + C
$$

Using initial condition $y(1)=4$:

$$
\ln 4 = -3(1) + C \implies C = \ln 4 + 3
$$

Solution:

$$
y = e^{-3x + C} = 4 e^{3-3x}
$$

---

## 📌 Exponential Growth and Decay

If 

$$
\frac{dy}{dt} = ky
$$

then solution:

$$
y(t) = y_0 e^{kt}
$$

- $k>0$ → growth  
- $k<0$ → decay  

- **Example (decay):**

$$
\frac{dy}{dt} = -0.1y, \quad y(0)=100
$$

$$
y(t) = 100 e^{-0.1t}
$$

- **Example (growth):**

$$
\frac{dP}{dt} = 0.05P, \quad P(0)=1000
$$

$$
P(t) = 1000 e^{0.05 t}
$$

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






