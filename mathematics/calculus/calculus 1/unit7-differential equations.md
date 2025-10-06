# 📘 Calculus 1 – Unit 7: Differential Equations

*This file documents concepts and strategies I learned from Khan Academy's Unit 7 of Calculus 1: Differential Equations.*

🔗 Source: [Khan Academy – Differential Equations](https://www.khanacademy.org/math/calculus-1/cs1-differential-equations)

---

## 📌 Introduction to Differential Equations

A **differential equation** is an equation that relates a function to its derivatives.

- **Example:**

$$
\frac{dy}{dx} = 3y
$$

This means the rate of change of $y$ with respect to $x$ is 3 times $y$.

- **Solution:** A function $y(x)$ that satisfies the equation.

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

## 📌 Logistic Growth Model

Population growth with limiting factor:

$$
\frac{dP}{dt} = kP\left(1 - \frac{P}{M}\right)
$$

- $M$ = carrying capacity  
- Integrate using **partial fractions** for solution.

- **Example:** 

$$
\frac{dP}{dt}=0.5 P\left(1 - \frac{P}{1000}\right), \quad P(0)=50
$$

---

## ✅ Summary of Topics in Unit 7

* [x] Introduction to differential equations  
* [x] Writing differential equations from scenarios  
* [x] Verifying solutions  
* [x] Slope fields  
* [x] Reasoning with slope fields  
* [x] Separation of variables  
* [x] Particular solutions & initial conditions  
* [x] Exponential growth & decay  
* [x] Logistic growth model  

---

> This file is part of my AI/ML journey repo documenting foundational math skills before diving into machine learning and AI.
