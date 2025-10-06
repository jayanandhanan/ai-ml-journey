# 📘 Calculus 1 – Unit 7: Differential Equations

*This file documents concepts and strategies I learned from Khan Academy's Unit 7 of Calculus 1: Differential Equations.*

🔗 Source: [Khan Academy – Differential Equations](https://www.khanacademy.org/math/calculus-1/cs1-differential-equations)

---

## 📌 Introduction to Differential Equations

A **differential equation** is an equation that relates a function to its derivatives.

- **Example:**  
  \[
  \frac{dy}{dx} = 3y
  \]  
  This says the rate of change of \(y\) with respect to \(x\) is 3 times \(y\).

- **Solution:** A function \(y(x)\) that satisfies the equation.  

---

## 📌 Verifying Solutions

To check if a function is a solution:

1. Compute the derivative \(y'(x)\).  
2. Substitute \(y(x)\) and \(y'(x)\) into the differential equation.  
3. If both sides are equal, the function is a solution.

- **Example:** Verify \(y=e^{2x}\) is a solution of \(\frac{dy}{dx}=2y\).

  \[
  y' = 2e^{2x}, \quad 2y = 2e^{2x} \implies y'=2y
  \]  
  ✅ True, so it is a solution.

---

## 📌 Slope Fields

A **slope field** is a graphical representation of a differential equation \(\frac{dy}{dx} = f(x,y)\).

- At each point \((x,y)\), draw a small line segment with slope \(f(x,y)\).  
- This helps visualize solution curves without solving the equation.

- **Example:** \(\frac{dy}{dx} = x - y\) → draw slope segments for various \((x,y)\) values.

---

## 📌 Reasoning with Slope Fields

- Observe the direction of slopes to predict behavior of solutions.  
- Solution curves follow the tangent lines indicated by the slope field.

- **Example:** For \(\frac{dy}{dx} = y\), slopes increase as \(y\) increases → solutions grow exponentially.

---

## 📌 Separation of Variables

Used for **separable differential equations**:

\[
\frac{dy}{dx} = g(x)h(y)
\]

**Steps:**

1. Rearrange to separate variables:
   \[
   \frac{dy}{h(y)} = g(x) dx
   \]
2. Integrate both sides:
   \[
   \int \frac{1}{h(y)} dy = \int g(x) dx
   \]
3. Solve for \(y\).

- **Example:** Solve \(\frac{dy}{dx} = 2y\), \(y(0)=3\)
  \[
  \frac{dy}{y} = 2 dx \implies \ln|y| = 2x + C \implies y = 3 e^{2x}
  \]

---

## 📌 Particular Solutions

- **Particular solution:** A solution satisfying an **initial condition**.  

- **Example:** Solve \(\frac{dy}{dx} = -3y\), \(y(1)=4\)
  \[
  \frac{dy}{y} = -3 dx \implies \ln|y| = -3x + C
  \]  
  Use initial condition:
  \[
  \ln 4 = -3(1) + C \implies C = \ln 4 + 3
  \]  
  Solution:
  \[
  y = e^{-3x + C} = 4 e^{3-3x}
  \]

---

## 📌 Exponential Growth and Decay

- If \(\frac{dy}{dt} = ky\), solution is:
  \[
  y(t) = y_0 e^{kt}
  \]
  - \(k>0\) → growth  
  - \(k<0\) → decay  

- **Example:** Radioactive decay: \(\frac{dy}{dt} = -0.1y\), \(y(0)=100\)
  \[
  y(t) = 100 e^{-0.1t}
  \]

- **Example:** Population growth: \(\frac{dP}{dt}=0.05P\), \(P(0)=1000\)
  \[
  P(t) = 1000 e^{0.05 t}
  \]

---

## 📌 Solving Linear First-Order Differential Equations

Equation:
\[
\frac{dy}{dx} + P(x)y = Q(x)
\]

**Steps:**

1. Find **integrating factor**:
   \[
   \mu(x) = e^{\int P(x) dx}
   \]
2. Multiply entire equation by \(\mu(x)\) to rewrite as:
   \[
   \frac{d}{dx} [\mu(x)y] = \mu(x)Q(x)
   \]
3. Integrate both sides and solve for \(y(x)\).

- **Example:** Solve \(\frac{dy}{dx}+2y = e^{3x}\)
  \[
  \mu(x) = e^{\int 2 dx} = e^{2x}
  \]
  \[
  \frac{d}{dx}[e^{2x}y] = e^{5x} \implies e^{2x}y = \frac{1}{5} e^{5x} + C
  \]
  \[
  y = \frac{1}{5} e^{3x} + C e^{-2x}
  \]

---

## 📌 Logistic Growth Model

Used to model **population with limiting factor**:

\[
\frac{dP}{dt} = kP\left(1-\frac{P}{M}\right)
\]

- \(M\) = carrying capacity  
- Solution involves integrating using partial fractions.

- **Example:** Solve \(\frac{dP}{dt}=0.5P(1-P/1000)\), \(P(0)=50\)

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
* [x] Linear first-order differential equations  
* [x] Logistic growth model  

---

> This file is part of my AI/ML journey repo documenting foundational math skills before diving into machine learning and AI.
