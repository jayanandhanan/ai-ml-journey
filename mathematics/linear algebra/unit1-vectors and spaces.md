# 📘 Linear Algebra – Unit 1: Vectors and Spaces

*This file documents all concepts, formulas, and strategies I learned from Khan Academy’s Linear Algebra unit on Vectors and Spaces.*

🔗 **Source:** [Khan Academy – Vectors and Spaces](https://www.khanacademy.org/math/linear-algebra/vectors-and-spaces)

---

## 📌 1. Vectors and Real Coordinate Spaces

A **vector** is an ordered list of numbers representing both **magnitude** and **direction**.

Example:

$$
v =
\begin{bmatrix}
2 \\
-3 \\
5
\end{bmatrix}
\in \mathbb{R}^3
$$

Here, $\mathbb{R}^3$ means all 3D vectors with real-number components.

---

## 📌 2. Adding Vectors Algebraically and Graphically

For two vectors:

$$
u =
\begin{bmatrix}
u_1 \\
u_2
\end{bmatrix},
\quad
v =
\begin{bmatrix}
v_1 \\
v_2
\end{bmatrix}
$$

Their sum is:

$$
u + v =
\begin{bmatrix}
u_1 + v_1 \\
u_2 + v_2
\end{bmatrix}
$$

**Graphically:** Place the tail of $v$ at the head of $u$;  
the diagonal of the parallelogram represents $u + v$.

---

## 📌 3. Multiplying a Vector by a Scalar

For scalar $c$:

$$
c v =
\begin{bmatrix}
c v_1 \\
c v_2
\end{bmatrix}
$$

- $c > 1$: stretches the vector  
- $0 < c < 1$: shrinks the vector  
- $c < 0$: reverses direction

---

## 📌 4. Unit Vectors and Their Formula

The **magnitude (length)** of a vector is:

$$
\|v\| = \sqrt{v_1^2 + v_2^2 + \dots + v_n^2}
$$

A **unit vector** in the direction of $v$:

$$
\hat{v} = \frac{v}{\|v\|}
$$

---

## 📌 5. Vector Addition Using Components and Unit Representation

If:

$$
a = a_x i + a_y j,
\quad
b = b_x i + b_y j
$$

Then:

$$
a + b = (a_x + b_x)i + (a_y + b_y)j
$$

---

## 📌 6. Parallelogram Method and Angle–Magnitude Form

If two vectors $a$ and $b$ make an angle $\theta$,  
the magnitude of their resultant is:

$$
|a + b| = \sqrt{a^2 + b^2 + 2ab\cos(\theta)}
$$

The direction is given by:

$$
\tan(\phi) = \frac{b\sin(\theta)}{a + b\cos(\theta)}
$$

---

## 📌 7. Magnitude, Length, and Direction with the x-axis

For vector $v = [x, y]^T$:

$$
\|v\| = \sqrt{x^2 + y^2}
$$

If $\theta$ is the angle with the x-axis:

$$
x = r\cos(\theta), \quad y = r\sin(\theta)
$$

where $r = \|v\|$.

---

## 📌 8. Parametric Representation of Lines

A line through point $p_0$ in direction $d$:

$$
r(t) = p_0 + t d, \quad t \in \mathbb{R}
$$

**Example:**

$$
r(t) =
\begin{bmatrix}
2 \\
-1 \\
0
\end{bmatrix}
+
t
\begin{bmatrix}
3 \\
2 \\
-4
\end{bmatrix}
$$

---

## 📌 9. Vector Connecting Two Points

If $P(x_1, y_1, z_1)$ and $Q(x_2, y_2, z_2)$:

$$
\overrightarrow{PQ} =
\begin{bmatrix}
x_2 - x_1 \\
y_2 - y_1 \\
z_2 - z_1
\end{bmatrix}
$$

---

## 📌 10. Linear Combinations and Span

A **linear combination** of vectors $v_1, v_2, \dots, v_k$:

$$
c_1 v_1 + c_2 v_2 + \dots + c_k v_k
$$

The **span** is the set of all possible combinations.

**Example:**

$$
\text{Span}(
\{
\begin{bmatrix}
1 \\
0
\end{bmatrix},
\begin{bmatrix}
0 \\
1
\end{bmatrix}
\}
)
= \mathbb{R}^2
$$

---

## 📌 11. Linear Dependence and Independence

Vectors are **linearly independent** if:

$$
c_1 v_1 + c_2 v_2 + \dots + c_k v_k = 0
$$

implies $c_1 = c_2 = \dots = c_k = 0$.  
Otherwise, they are **dependent**.

---

## 📌 12. Linear Subspaces and Basis

A **subspace** of $\mathbb{R}^n$ is a set of vectors closed under addition and scalar multiplication.

A **basis** is a set of linearly independent vectors that span a subspace.

The number of basis vectors = **dimension** of that subspace.

---

## 📌 13. Dot Product and Vector Length

For $u, v \in \mathbb{R}^n$:

$$
u \cdot v = u_1v_1 + u_2v_2 + \dots + u_nv_n
$$

and

$$
\|v\| = \sqrt{v \cdot v}
$$

---

## 📌 14. Dot Product Properties

1. $u \cdot v = v \cdot u$  
2. $u \cdot (v + w) = u \cdot v + u \cdot w$  
3. $(c u) \cdot v = c(u \cdot v)$

---

## 📌 15. Cauchy–Schwarz and Triangle Inequalities

**Cauchy–Schwarz:**

$$
|u \cdot v| \le \|u\| \, \|v\|
$$

**Triangle Inequality:**

$$
\|u + v\| \le \|u\| + \|v\|
$$

---

## 📌 16. Angle Between Vectors and Orthogonality

$$
\cos(\theta) = \frac{u \cdot v}{\|u\| \, \|v\|}
$$

If $u \cdot v = 0$, the vectors are **orthogonal** (perpendicular).

---

## 📌 17. Planes in $\mathbb{R}^3$ and Normal Vectors

Equation of a plane:

$$
a(x - x_0) + b(y - y_0) + c(z - z_0) = 0
$$

where $[a, b, c]$ is the **normal vector**.

---

## 📌 18. Cross Product and Relation to Angle

For $u, v \in \mathbb{R}^3$:

$$
u \times v =
\begin{bmatrix}
u_2v_3 - u_3v_2 \\
u_3v_1 - u_1v_3 \\
u_1v_2 - u_2v_1
\end{bmatrix}
$$

and

$$
\|u \times v\| = \|u\| \, \|v\| \sin(\theta)
$$

---

## 📌 19. Dot and Cross Product Comparison

| Property | Dot Product | Cross Product |
|-----------|--------------|----------------|
| Type | Scalar | Vector |
| Depends on | $\cos(\theta)$ | $\sin(\theta)$ |
| Measures | Parallel similarity | Perpendicular direction |

---

## 📌 20. Vector Triple Product

$$
a \times (b \times c) = b(a \cdot c) - c(a \cdot b)
$$

---

## 📌 21. Distance from Point to Plane

If plane: $ax + by + cz + d = 0$ and point $P(x_1, y_1, z_1)$:

$$
D = \frac{|ax_1 + by_1 + cz_1 + d|}{\sqrt{a^2 + b^2 + c^2}}
$$

---

## 📌 22. Distance Between Two Parallel Planes

For $ax + by + cz + d_1 = 0$ and $ax + by + cz + d_2 = 0$:

$$
\text{Distance} = \frac{|d_1 - d_2|}{\sqrt{a^2 + b^2 + c^2}}
$$

---

## 📌 23. Matrices and Solving Systems by Elimination

Matrix form:

$$
A x = b
$$

Solve by **Gaussian elimination** to reach **Row-Reduced Echelon Form (RREF)**.

---

## 📌 24. Matrix–Vector Products

For:

$$
A =
\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix},
\quad
x =
\begin{bmatrix}
x_1 \\
x_2
\end{bmatrix}
$$

then:

$$
A x =
\begin{bmatrix}
1x_1 + 2x_2 \\
3x_1 + 4x_2
\end{bmatrix}
$$

---

## 📌 25. Null Space of a Matrix

The **null space** $N(A)$:

$$
N(A) = \{ x \mid A x = 0 \}
$$

Represents all solutions that map to zero.

---

## 📌 26. Column Space of a Matrix

The **column space** $C(A)$:

$$
C(A) = \text{Span of the columns of } A
$$

Represents all possible output vectors of $A x$.

---

## 📌 27. Relation Between Null Space and Linear Independence

If the **null space** contains only the zero vector,  
the columns of $A$ are **linearly independent**.

---

## 📌 28. Basis for Null and Column Spaces

- **Basis for $N(A)$:** independent solutions to $A x = 0$  
- **Basis for $C(A)$:** pivot columns of $A$

---

## 📌 29. Visualizing Column Space as a Plane in $\mathbb{R}^3$

If matrix $A$ has two independent columns in $\mathbb{R}^3$,  
its column space is a **plane through the origin**.

---

## 📌 30. Dimension, Rank, and Nullity

- **Rank(A)** = dimension of column space  
- **Nullity(A)** = dimension of null space  

**Rank–Nullity Theorem:**

$$
\text{rank}(A) + \text{nullity}(A) = \text{number of columns of } A
$$

---

## ✅ Topics Covered

- [x] Vectors and coordinate spaces  
- [x] Vector addition and scalar multiplication  
- [x] Unit vectors and direction cosines  
- [x] Linear combinations and spans  
- [x] Dependence and independence  
- [x] Subspaces and basis  
- [x] Dot, cross, and triple products  
- [x] Planes, normals, and distances  
- [x] Matrices, RREF, and elimination  
- [x] Null and column spaces, basis, rank, nullity  

---

> This file is part of my AI/ML learning journey — documenting foundational linear algebra concepts before advancing to calculus, vector calculus, and machine learning.
