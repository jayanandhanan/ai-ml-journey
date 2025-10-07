# 📘 Calculus 1 – Unit 8: Applications of Integrals

*This file documents concepts and strategies I learned from Khan Academy's Unit 8 of Calculus 1: Applications of Integrals.*

🔗 Source: [Khan Academy – Applications of Integrals](https://www.khanacademy.org/math/calculus-1/cs1-applications-of-integrals)

---

## 📌 Average Value of a Function

The **average value** of a continuous function $f(x)$ on $[a,b]$ is:

$$
f_{\text{avg}} = \frac{1}{b-a} \int_a^b f(x)\,dx
$$

- **Example:** Find the average value of $f(x)=x^2$ on $[0,2]$:

$$
f_{\text{avg}} = \frac{1}{2-0} \int_0^2 x^2 \, dx = \frac{1}{2} \cdot \frac{8}{3} = \frac{4}{3}
$$

---

## 📌 Straight-Line Motion

Position $s(t)$, velocity $v(t)$, and acceleration $a(t)$ are related:

$$
v(t) = \frac{ds}{dt}, \quad a(t) = \frac{dv}{dt}
$$

**Displacement:**

$$
\Delta s = \int_{t_0}^{t_1} v(t) \, dt
$$

**Distance traveled:**

$$
\text{Distance} = \int_{t_0}^{t_1} |v(t)| \, dt
$$

---

## 📌 Non-Motion Applications of Integrals

Integrals can represent accumulated quantities such as:

- Area under a curve  
- Total charge, mass, or energy  

- **Example:** Total charge if current $I(t)$:

$$
Q = \int_{t_0}^{t_1} I(t) \, dt
$$

---

## 📌 Area: Vertical Area Between Curves

For functions $f(x)$ and $g(x)$ with $f(x) \ge g(x)$:

$$
\text{Area} = \int_a^b \big(f(x) - g(x)\big) \, dx
$$

- **Example:** Area between $f(x)=x^2$ and $g(x)=x$ on $[0,1]$:

$$
\int_0^1 (x - x^2) \, dx = \frac{1}{6}
$$

---

## 📌 Area: Horizontal Area Between Curves

If functions are given as $x=f(y)$ and $x=g(y)$:

$$
\text{Area} = \int_c^d \big(f(y) - g(y)\big) \, dy
$$

- Useful when curves are better expressed as functions of $y$.

---

## 📌 Area: Curves that Intersect at More Than Two Points

- Break the interval at **intersection points**.  
- Sum absolute differences:

$$
\text{Total Area} = \sum_i \int_{x_i}^{x_{i+1}} |f(x) - g(x)| \, dx
$$

---

## 📌 Volume: Cross Sections – Squares and Rectangles

- For a solid with known cross-sectional area $A(x)$:

$$
\text{Volume} = \int_a^b A(x) \, dx
$$

- **Square cross-section:** $A(x) = s^2$  
- **Rectangular cross-section:** $A(x) = \text{width} \cdot \text{height}$

---

## 📌 Volume: Cross Sections – Triangles and Semicircles

- **Triangular cross-section (base $b$, height $h$):**

$$
A = \frac{1}{2} b h
$$

- **Semicircular cross-section (radius $r$):**

$$
A = \frac{1}{2} \pi r^2
$$

- Volume formula still:

$$
V = \int_a^b A(x) \, dx
$$

---

## 📌 Volume: Disc Method (Revolving Around x- or y-Axes)

- **Revolve around x-axis:**

$$
V = \pi \int_a^b [f(x)]^2 \, dx
$$

- **Revolve around y-axis:**

$$
V = \pi \int_c^d [f(y)]^2 \, dy
$$

---

## 📌 Volume: Disc Method (Revolving Around Other Axes)

- Shift functions by axis $y=k$ or $x=h$:

$$
V = \pi \int_a^b [f(x)-k]^2 \, dx
$$

---

## 📌 Volume: Washer Method (Revolving Around x- or y-Axes)

- Hollow disc (washer) with outer $R(x)$ and inner $r(x)$:

$$
V = \pi \int_a^b \big(R(x)^2 - r(x)^2\big) \, dx
$$

---

## 📌 Volume: Washer Method (Revolving Around Other Axes)

- For axis $y=k$ or $x=h$:

$$
V = \pi \int_a^b \big([R(x)-k]^2 - [r(x)-k]^2\big) \, dx
$$

---

## ✅ Summary of Topics in Unit 8

* [x] Average value of a function  
* [x] Straight-line motion  
* [x] Non-motion applications of integrals  
* [x] Area: vertical area between curves  
* [x] Area: horizontal area between curves  
* [x] Area: curves that intersect at more than two points  
* [x] Volume: squares and rectangles cross sections  
* [x] Volume: triangles and semicircles cross sections  
* [x] Volume: disc method (x- and y-axes)  
* [x] Volume: disc method (other axes)  
* [x] Volume: washer method (x- and y-axes)  
* [x] Volume: washer method (other axes)  

---


> This file is part of my AI/ML journey repo documenting foundational math skills before diving into machine learning and AI.

