# 📘 Calculus 2 – Unit 5: Parametric Equations, Polar Coordinates, and Vector-Valued Functions

*This file documents concepts and strategies I learned from Khan Academy's Calculus 2 unit on Parametric Equations, Polar Coordinates, and Vector-Valued Functions.*

🔗 Source: [Khan Academy – Parametric Equations, Polar Coordinates, and Vector-Valued Functions](https://www.khanacademy.org/math/calculus-2/cs2-parametric-equations-polar-coordinates-and-vector-valued-functions)

---

## 📌 Parametric Equations: Introduction

A **parametric equation** defines $x$ and $y$ in terms of a third variable, $t$ (the parameter):

$$
x = f(t), \quad y = g(t)
$$

**Example:**

$$
x = t^2, \quad y = t^3
$$

To eliminate $t$:

$$
t = \sqrt{x} \implies y = (\sqrt{x})^3 = x^{3/2}
$$

---

## 📌 Second Derivatives of Parametric Equations

The first derivative:

$$
\frac{dy}{dx} = \frac{\frac{dy}{dt}}{\frac{dx}{dt}}
$$

The second derivative:

$$
\frac{d^2y}{dx^2} = \frac{d}{dx} \left( \frac{dy}{dx} \right) = \frac{ \frac{d}{dt} \left( \frac{dy}{dx} \right) }{ \frac{dx}{dt} }
$$

**Example:**

$$
x = t^2, \quad y = t^3
$$

$$
\frac{dy}{dx} = \frac{3t^2}{2t} = \frac{3t}{2}, \quad \frac{d^2y}{dx^2} = \frac{d/dt (3t/2)}{dx/dt} = \frac{3/2}{2t} = \frac{3}{4t}
$$

---

## 📌 Arc Length: Parametric Curves

Arc length of a parametric curve:

$$
L = \int_a^b \sqrt{\left(\frac{dx}{dt}\right)^2 + \left(\frac{dy}{dt}\right)^2} dt
$$

**Example:**

$$
x = t, \quad y = t^2, \quad t \in [0,1]
$$

$$
L = \int_0^1 \sqrt{(dx/dt)^2 + (dy/dt)^2} dt = \int_0^1 \sqrt{1 + (2t)^2} dt = \int_0^1 \sqrt{1 + 4t^2} dt
$$

---

## 📌 Vector-Valued Functions

A vector-valued function can be expressed in **component form** using **unit vectors** $\mathbf{i}$ and $\mathbf{j}$:

$$
\vec{r}(t) = x(t)\mathbf{i} + y(t)\mathbf{j}
$$

Velocity:

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = x'(t)\mathbf{i} + y'(t)\mathbf{j}
$$

Speed:

$$
|\vec{v}(t)| = \sqrt{ (x'(t))^2 + (y'(t))^2 }
$$

---

### 🔹 Directional (unit vector) form

The **unit vector along velocity**:

$$
\hat{v}(t) = \frac{\vec{v}(t)}{|\vec{v}(t)|}
$$

Then the velocity can be expressed as:

$$
\vec{v}(t) = |\vec{v}(t)| \hat{v}(t)
$$

---

### Example

Let:

$$
x(t) = t^2, \quad y(t) = t^3
$$

**Component form:**

$$
\vec{r}(t) = t^2 \mathbf{i} + t^3 \mathbf{j}, \quad 
\vec{v}(t) = 2t \mathbf{i} + 3t^2 \mathbf{j}
$$

**Speed:**

$$
|\vec{v}(t)| = \sqrt{(2t)^2 + (3t^2)^2} = \sqrt{4t^2 + 9t^4}
$$

**Unit vector along velocity:**

$$
\hat{v}(t) = \frac{\vec{v}(t)}{|\vec{v}(t)|} = \left\langle \frac{2t}{\sqrt{4t^2 + 9t^4}}, \frac{3t^2}{\sqrt{4t^2 + 9t^4}} \right\rangle
$$

**Magnitude-direction form:**

$$
\vec{v}(t) = |\vec{v}(t)| \hat{v}(t) = \sqrt{4t^2 + 9t^4} \, \hat{v}(t)
$$

---

## 📌 Planar Motion

For an object moving in the plane with $\vec{r}(t) = \langle x(t), y(t) \rangle$:

- Position: $\vec{r}(t)$  
- Velocity: $\vec{v}(t) = \frac{d\vec{r}}{dt}$  
- Acceleration: $\vec{a}(t) = \frac{d\vec{v}}{dt}$  

**Example:**

$$
x(t) = t^2, \quad y(t) = t^3
$$

$$
\vec{v}(t) = \langle 2t, 3t^2 \rangle, \quad \vec{a}(t) = \langle 2, 6t \rangle
$$

---

## 📌 Polar Functions

Polar coordinates:

$$
x = r \cos\theta, \quad y = r \sin\theta
$$

$$
r = \sqrt{x^2 + y^2}, \quad \theta = \arctan\frac{y}{x}
$$

---

## 📌 Area: Polar Regions (Single Curve)

Area enclosed by a polar curve $r(\theta)$:

$$
A = \frac{1}{2} \int_{\alpha}^{\beta} r^2 d\theta
$$

**Example:**

$$
r = 2\cos\theta, \quad \theta \in [0, \pi/2]
$$

$$
A = \frac{1}{2} \int_0^{\pi/2} (2\cos\theta)^2 d\theta = 2 \int_0^{\pi/2} \cos^2\theta d\theta
$$

---

## 📌 Area: Polar Regions (Two Curves)

For $r = r_1(\theta)$ outside and $r = r_2(\theta)$ inside:

$$
A = \frac{1}{2} \int_{\alpha}^{\beta} \left( r_1^2 - r_2^2 \right) d\theta
$$

**Example:**

$$
r_1 = 3, \quad r_2 = 3 - 3\sin\theta, \quad \theta \in [0, \pi]
$$

$$
A = \frac{1}{2} \int_0^\pi \left( 3^2 - (3-3\sin\theta)^2 \right) d\theta
$$

---

## 📌 Arc Length: Polar Curves

Arc length for a polar curve $r(\theta)$:

$$
L = \int_{\alpha}^{\beta} \sqrt{ r^2 + \left(\frac{dr}{d\theta}\right)^2 } d\theta
$$

**Example:**

$$
r = 2\theta, \quad \theta \in [0, \pi]
$$

$$
L = \int_0^\pi \sqrt{ (2\theta)^2 + (2)^2 } d\theta = \int_0^\pi \sqrt{4\theta^2 + 4} d\theta
$$

---

## ✅ Topics Covered in this Unit

* [x] Parametric equations: introduction  
* [x] Second derivatives of parametric equations  
* [x] Arc length: parametric curves  
* [x] Vector-valued functions  
* [x] Planar motion  
* [x] Polar functions  
* [x] Area: polar regions (single curve)  
* [x] Area: polar regions (two curves)  
* [x] Arc length: polar curves  

---

> This file is part of my AI/ML journey repo documenting foundational math skills necessary for understanding vector calculus and motion before diving into machine learning and AI.

