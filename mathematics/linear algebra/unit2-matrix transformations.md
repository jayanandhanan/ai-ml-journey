# 📘 Linear Algebra – Unit 2: Matrix Transformations

*This file documents all concepts, formulas, and strategies from Khan Academy’s Linear Algebra unit on Matrix Transformations.*

🔗 **Source:** [Khan Academy – Matrix Transformations](https://www.khanacademy.org/math/linear-algebra/matrix-transformations)

---

## 📌 1. Functions, Domain, Codomain, & Range

A **function** maps each input to exactly one output:

$$
f : A \to B
$$

- **Domain:** all allowed inputs  
- **Codomain:** all possible outputs  
- **Range:** set of actual outputs produced  

A **transformation** is a function where inputs and outputs are vectors.

---

## 📌 2. Vector Transformations

A transformation between vector spaces:

$$
T : \mathbb{R}^n \to \mathbb{R}^m
$$

---

## 📌 3. Linear Transformations

A transformation \(T\) is **linear** if:

$$
T(u + v) = T(u) + T(v)
$$

$$
T(cu) = c \ T(u)
$$

This implies automatically:

$$
T(0) = 0
$$

---

## 📌 4. Matrix from a Linear Transformation

Matrix \(A\) representing \(T\) is obtained by transforming standard basis vectors:

$$
e_1 =
\begin{bmatrix}
1 \\
0
\end{bmatrix}, \quad
e_2 =
\begin{bmatrix}
0 \\
1
\end{bmatrix}
$$

$$
A = 
\begin{bmatrix}
T(e_1) & T(e_2)
\end{bmatrix}
$$

---

## 📌 5. Matrix–Vector Product as Linear Combination

Columns of \(A\): $$(A_1, A_2, \..., A_n)$$

$$
Ax = x_1 A_1 + x_2 A_2 + \dots + x_n A_n
$$

---

## 📌 6. Image and Pre-image

- **Image of a vector:** $$\(T(x)\)$$
- **Image of a set:** $$\(T(S) = \{T(x) \mid x \in S\}\)$$
- **Pre-image of y:** $$all \(x\) such that \(T(x) = y\)$$

---

## 📌 7. Kernel (Null Space)

$$
\ker(T) = \{x \mid T(x) = 0\}
$$

---

## 📌 8. Sums and Scalar Multiples of Linear Transformations

$$
(T_1 + T_2)(x) = T_1(x) + T_2(x)
$$

$$
(c \ T_1)(x) = c \ T_1(x)
$$

---

## 📌 9. Linear Transformation Types

- **Scaling:** 

$$
A =
\begin{bmatrix}
k & 0 \\
0 & k
\end{bmatrix}
$$

- **Reflection across x-axis:** 

$$
A =
\begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix}
$$

- **Rotation in $$\(\mathbb{R}^2\):$$**

$$
A =
\begin{bmatrix}
\cos \theta & -\sin \theta \\
\sin \theta & \cos \theta
\end{bmatrix}
$$

---

## 📌 10. Unit Vectors and Projections

Projection of \(v\) onto \(u\):

$$
\text{proj}_u(v) = \frac{u \cdot v}{u \cdot u} \, u
$$

Matrix form:

$$
P = \frac{u u^T}{u^T u}
$$

---

## 📌 11. Composition of Transformations

$$
T_2(T_1(x)) = B A x
$$

---

## 📌 12. Properties of Matrix Multiplication

- Associative: $$\((AB)C = A(BC)\)$$ 
- Distributive: $$\(A(B + C) = AB + AC\)$$ 
- Not commutative: $$\(AB \neq BA\)$$

---

## 📌 13. Inverse Transformations

$$
T^{-1}(T(x)) = x
$$

**Matrix Condition:**

$$
A \text{ invertible } \iff \det(A) \neq 0
$$

---

## 📌 14. Conditions for Invertibility

A square matrix is invertible iff:

1. $$\(\det(A) \neq 0\)$$
2. Columns independent  
3. Rank = n  
4. Nullity = 0  
5. Transformation is one-to-one and onto

---

## 📌 15. Surjective (Onto) and Injective (One-to-One)

- **Onto:** $$Every \(y\)$$ has some \(x\) s.t. \(Ax = y\)$$
- **One-to-One:** $$\(Ax = 0 \implies x = 0\)$$

---

## 📌 16. Solving \(Ax = b\)

General solution:

$$
x = x_p + x_n
$$

Where $$\(x_p\) = particular solution, \(x_n\) = null-space vector.$$

---

## 📌 17. Determinants

**2×2:**

$$
\det
\begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
= ad - bc
$$

**3×3 (Sarrus rule):**

$$
\det
\begin{bmatrix}
a & b & c \\
d & e & f \\
g & h & i
\end{bmatrix}
= aei + bfg + cdh - ceg - bdi - afh
$$

---

## 📌 18. Determinants and Geometry

- Area scaling in $$\(\mathbb{R}^2\), volume in \(\mathbb{R}^3\): \(|\det(A)|\)$$ 
- $$0 → collapse to lower dimension$$

---

## 📌 19. Transpose of a Matrix

$$
(A^T)_{ij} = A_{ji}
$$

Properties:

- $$\((A^T)^T = A\)$$ 
- $$\((AB)^T = B^T A^T\)$$
- $$\(\det(A^T) = \det(A)\)$$

---

## 📌 20. Row Space, Column Space & Null Spaces

- Row space = span of rows  
- Column space = span of columns  
- Null space = $$\(\{x \mid Ax = 0\}\)$$  
- Left null space = $$\(\{y \mid A^T y = 0\}\)$$  

**Orthogonality:**

- Row space ⟂ Null space  
- Column space ⟂ Left null space

---

## 📌 21. Rank and Invertibility

- $$\(\text{rank}(A) = \text{rank}(A^T)\)$$  
- $$\(A^T A\) invertible ⇔ columns independent$$

---

## ✅ Topics Covered

- Functions → transformations  
- Vector transformations  
- Linear transformations: scaling, reflection, & rotation  
- Matrix representation, composition, sum, & scalar multiple  
- Image, pre-image, & kernel  
- Projections & unit vectors  
- Solving $$\(Ax = b\)$$, invertibility, one-to-one, & onto  
- Determinants & transpose  
- Row space, column space, left null space, & rank  

---

> This file is part of my AI/ML learning journey — documenting linear algebra concepts before advancing to vector calculus and machine learning.

