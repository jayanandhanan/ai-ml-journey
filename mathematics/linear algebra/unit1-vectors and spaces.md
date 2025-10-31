# 📘 Linear Algebra – Unit 1: Vectors and Spaces

*This file documents all concepts, formulas, and examples from Khan Academy’s Linear Algebra Unit 1: “Vectors and Spaces.”*

🔗 Source: [Khan Academy – Vectors and Spaces](https://www.khanacademy.org/math/linear-algebra/vectors-and-spaces)

---

## 📌 1. Vectors and Real Coordinate Spaces

A **vector** is an ordered list of numbers representing both **magnitude** and **direction**.

Example:

$$
\mathbf{v} =
\begin{bmatrix}
2 \\ -3 \\ 5
\end{bmatrix}
\in \mathbb{R}^3
$$

Here, \( \mathbb{R}^3 \) means all 3D vectors with real-number components.

---

## 📌 2. Adding Vectors Algebraically and Graphically

For two vectors:

$$
\mathbf{u} =
\begin{bmatrix} u_1 \\ u_2 \end{bmatrix},
\quad
\mathbf{v} =
\begin{bmatrix} v_1 \\ v_2 \end{bmatrix}
$$

Their sum is:

$$
\mathbf{u} + \mathbf{v} =
\begin{bmatrix}
u_1 + v_1 \\
u_2 + v_2
\end{bmatrix}
$$

**Graphically:** Place the tail of **v** at the head of **u**; the diagonal of the parallelogram represents **u + v**.

---

## 📌 3. Multiplying a Vector by a Scalar

For scalar \( c \):

$$
c\mathbf{v} =
\begin{bmatrix}
cv_1 \\
cv_2
\end{bmatrix}
$$

- \( c > 1 \): stretches the vector  
- \( 0 < c < 1 \): shrinks the vector  
- \( c < 0 \): reverses direction

---

## 📌 4. Unit Vectors and Their Formula

The **magnitude (length)** of a vector is:

$$
||\mathbf{v}|| = \sqrt{v_1^2 + v_2^2 + \dots + v_n^2}
$$

A **unit vector** in the direction of \( \mathbf{v} \):

$$
\hat{\mathbf{v}} = \frac{\mathbf{v}}{||\mathbf{v}||}
$$

---

## 📌 5. Vector Addition Using Components and Unit Representation

If:

$$
\mathbf{a} = a_x \hat{i} + a_y \hat{j}
\quad \text{and} \quad
\mathbf{b} = b_x \hat{i} + b_y \hat{j}
$$

Then:

$$
\mathbf{a} + \mathbf{b} = (a_x + b_x)\hat{i} + (a_y + b_y)\hat{j}
$$

---

## 📌 6. Parallelogram Method and Angle–Magnitude Form

The **resultant vector** of \( \mathbf{a} \) and \( \mathbf{b} \):

$$
R = \sqrt{a^2 + b^2 + 2ab\cos\theta}
$$

Direction (angle):

$$
\tan\phi = \frac{b\sin\theta}{a + b\cos\theta}
$$

---

## 📌 7. Magnitude, Length, and Direction with x-axis

For vector \( \mathbf{v} = (x, y) \):

$$
||\mathbf{v}|| = \sqrt{x^2 + y^2}
$$

If \( \theta \) is the angle with the x-axis:

$$
x = r\cos\theta, \quad y = r\sin\theta
$$

where \( r = ||\mathbf{v}|| \).

---

## 📌 8. Parametric Representation of Lines

A line through point \( \mathbf{p_0} \) in direction \( \mathbf{d} \):

$$
\mathbf{r}(t) = \mathbf{p_0} + t\mathbf{d}, \quad t \in \mathbb{R}
$$

Example:

$$
\mathbf{r}(t) =
\begin{bmatrix} 2 \\ -1 \\ 0 \end{bmatrix}
+ t
\begin{bmatrix} 3 \\ 2 \\ -4 \end{bmatrix}
$$

---

## 📌 9. Vector Connecting Two Points

If \( P(x_1, y_1, z_1) \) and \( Q(x_2, y_2, z_2) \):

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

A **linear combination** of vectors \( \mathbf{v_1}, \mathbf{v_2}, ..., \mathbf{v_k} \):

$$
c_1\mathbf{v_1} + c_2\mathbf{v_2} + ... + c_k\mathbf{v_k}
$$

The **span** is the set of all possible combinations.

Example:
\[
\text{Span}\{ [1, 0], [0, 1] \} = \mathbb{R}^2
\]

---

## 📌 11. Linear Dependence and Independence

Vectors are **linearly independent** if:

$$
c_1\mathbf{v_1} + c_2\mathbf{v_2} + ... + c_k\mathbf{v_k} = \mathbf{0}
$$

implies \( c_1 = c_2 = ... = c_k = 0 \).  
Otherwise, they’re **dependent**.

---

## 📌 12. Linear Subspaces and Basis

A **subspace** of \( \mathbb{R}^n \) is a set of vectors closed under addition and scalar multiplication.

A **basis** is a set of linearly independent vectors that span a subspace.

Number of basis vectors = **dimension** of that subspace.

---

## 📌 13. Dot Product and Vector Length

For \( \mathbf{u}, \mathbf{v} \in \mathbb{R}^n \):

$$
\mathbf{u} \cdot \mathbf{v} = u_1v_1 + u_2v_2 + \dots + u_nv_n
$$

and

$$
||\mathbf{v}|| = \sqrt{\mathbf{v} \cdot \mathbf{v}}
$$

---

## 📌 14. Dot Product Properties

1. \( \mathbf{u} \cdot \mathbf{v} = \mathbf{v} \cdot \mathbf{u} \)  
2. \( \mathbf{u} \cdot (\mathbf{v} + \mathbf{w}) = \mathbf{u} \cdot \mathbf{v} + \mathbf{u} \cdot \mathbf{w} \)  
3. \( (c\mathbf{u}) \cdot \mathbf{v} = c(\mathbf{u} \cdot \mathbf{v}) \)

---

## 📌 15. Cauchy–Schwarz and Triangle Inequalities

**Cauchy–Schwarz:**
$$
|\mathbf{u} \cdot \mathbf{v}| \le ||\mathbf{u}|| \, ||\mathbf{v}||
$$

**Triangle Inequality:**
$$
||\mathbf{u} + \mathbf{v}|| \le ||\mathbf{u}|| + ||\mathbf{v}||
$$

---

## 📌 16. Angle Between Vectors and Orthogonality

$$
\cos\theta = \frac{\mathbf{u} \cdot \mathbf{v}}{||\mathbf{u}|| \, ||\mathbf{v}||}
$$

If \( \mathbf{u} \cdot \mathbf{v} = 0 \), the vectors are **orthogonal** (perpendicular).

---

## 📌 17. Planes in \(\mathbb{R}^3\) and Normal Vectors

Equation of a plane:

$$
a(x - x_0) + b(y - y_0) + c(z - z_0) = 0
$$

where \( [a, b, c] \) is the **normal vector**.

---

## 📌 18. Cross Product and Relation to Angle

For \( \mathbf{u}, \mathbf{v} \in \mathbb{R}^3 \):

$$
\mathbf{u} \times \mathbf{v} =
\begin{bmatrix}
u_2v_3 - u_3v_2 \\
u_3v_1 - u_1v_3 \\
u_1v_2 - u_2v_1
\end{bmatrix}
$$

and

$$
||\mathbf{u} \times \mathbf{v}|| = ||\mathbf{u}|| \, ||\mathbf{v}|| \sin\theta
$$

---

## 📌 19. Dot and Cross Product Comparison

| Property | Dot Product | Cross Product |
|-----------|--------------|----------------|
| Type | Scalar | Vector |
| Depends on | cos(θ) | sin(θ) |
| Measures | Parallel similarity | Perpendicular direction |

---

## 📌 20. Vector Triple Product

$$
\mathbf{a} \times (\mathbf{b} \times \mathbf{c}) = \mathbf{b}(\mathbf{a} \cdot \mathbf{c}) - \mathbf{c}(\mathbf{a} \cdot \mathbf{b})
$$

---

## 📌 21. Distance from Point to Plane

If plane: \( ax + by + cz + d = 0 \) and point \( P(x_1, y_1, z_1) \):

$$
D = \frac{|ax_1 + by_1 + cz_1 + d|}{\sqrt{a^2 + b^2 + c^2}}
$$

---

## 📌 22. Distance Between Two Parallel Planes

For \( ax + by + cz + d_1 = 0 \) and \( ax + by + cz + d_2 = 0 \):

$$
\text{Distance} = \frac{|d_1 - d_2|}{\sqrt{a^2 + b^2 + c^2}}
$$

---

## 📌 23. Matrices and Solving Systems by Elimination

Matrix form:

$$
A\mathbf{x} = \mathbf{b}
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
\mathbf{x} =
\begin{bmatrix}
x_1 \\ x_2
\end{bmatrix}
$$

then:

$$
A\mathbf{x} =
\begin{bmatrix}
1x_1 + 2x_2 \\
3x_1 + 4x_2
\end{bmatrix}
$$

---

## 📌 25. Null Space of a Matrix

The **null space** \( N(A) \):

$$
N(A) = \{ \mathbf{x} \mid A\mathbf{x} = 0 \}
$$

Represents all solutions that map to zero.

---

## 📌 26. Column Space of a Matrix

The **column space** \( C(A) \):

$$
C(A) = \text{Span of the columns of } A
$$

Represents all possible output vectors of \( A\mathbf{x} \).

---

## 📌 27. Relation Between Null Space and Linear Independence

If the **null space** contains only the zero vector, the columns of \( A \) are **linearly independent**.

---

## 📌 28. Basis for Null and Column Spaces

- **Basis for \( N(A) \)**: independent solutions to \( A\mathbf{x} = 0 \)  
- **Basis for \( C(A) \)**: pivot columns of \( A \)

---

## 📌 29. Visualizing Column Space as Plane in \(\mathbb{R}^3\)

If matrix \( A \) has two independent columns in \( \mathbb{R}^3 \), its column space is a **plane through the origin**.

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

> This file is part of my AI/ML journey repo documenting foundational math skills necessary for understanding vector calculus and motion before diving into machine learning and AI.

