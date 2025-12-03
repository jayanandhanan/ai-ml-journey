# 📘 Linear Algebra – Unit 2: Matrix Transformations

*This file documents all concepts, formulas, and strategies I learned from Khan Academy’s Linear Algebra unit on Matrix Transformations.*

🔗 **Source:** *Khan Academy – Matrix Transformations*

---

# 📌 1. Functions, Domain, Codomain, Range

A **function** maps each input to exactly one output:

```
f : A → B
```

* **Domain:** all allowed inputs
* **Codomain:** all possible outputs
* **Range:** all actual outputs produced

A **transformation** is a function whose inputs and outputs are vectors.

### Example

```
f(x) = x²
Domain = ℝ
Codomain = ℝ
Range = [0, ∞)
```

---

# 📌 2. Vector Transformations

A transformation between vector spaces:

```
T : ℝⁿ → ℝᵐ
```

### Example

```
T([x y]ᵀ) = [3x  
             x + y]
```

---

# 📌 3. Linear Transformations

A transformation is **linear** if:

```
1. T(u + v) = T(u) + T(v)
2. T(cu) = cT(u)
```

Automatically implies:

```
T(0) = 0
```

### Example

Check linearity:

```
T([x y]ᵀ) = [2x  
             5y]
```

This is linear — no constants added, only scaling.

---

# 📌 4. Visualizing Linear Transformations

* Lines through origin remain lines
* Grids become stretched grids
* Shapes scale, rotate, shear, reflect

### Example (shear)

```
A = [1 1
     0 1]
```

This pushes points sideways depending on their y-value.

---

# 📌 5. Matrix from a Linear Transformation

For a linear transformation `T(x) = Ax`, the matrix `A` is built by transforming standard basis vectors.

### Example

```
T(e₁) = [3  
         1]

T(e₂) = [2  
         4]
```

Matrix:

```
A = [3 2
     1 4]
```

---

# 📌 6. Matrix–Vector Product as Linear Combination

```
Ax = x₁A₁ + x₂A₂ + ... + xₙAₙ
```

Where `A₁, A₂, ..., Aₙ` are the **columns** of `A`.

### Example

```
A = [1 2
     3 4]

x = [5
     6]
```

Compute:

```
Ax = 5[1 3]ᵀ + 6[2 4]ᵀ
   = [17  
      39]
```

---

# 📌 7. Image of a Vector and Image of a Set

**Image of vector**: `T(x)`
**Image of set**:

```
T(S) = {T(x) | x ∈ S}
```

### Example

Transform the unit square by matrix

```
A = [2 0
     0 3]
```

Image: rectangle stretched 2× horizontally, 3× vertically.

---

# 📌 8. Pre-Image and Kernel (Null Space)

**Pre-image** of `y` is set of all `x` such that:

```
T(x) = y
```

**Kernel** (null space):

```
ker(T) = { x | T(x) = 0 } = N(A)
```

### Example

If

```
A = [1 2
     2 4]
```

Solve `Ax = 0`:

```
x = t[-2  
      1]
```

This whole line is the kernel.

---

# 📌 9. Kernel Properties

The kernel is always a **subspace**:

* Contains 0
* Closed under addition
* Closed under scalar multiplication

If:

```
ker(A) = {0}
```

Then transformation is **one-to-one**.

---

# 📌 10. Sums and Scalar Multiples of Transformations

```
(T₁ + T₂)(x) = T₁(x) + T₂(x)
(cT₁)(x) = cT₁(x)
```

For matrices:

```
(A + B)x = Ax + Bx
(cA)x = c(Ax)
```

### Example

```
A = [1 0]   B = [3 2]
    [0 1]        [1 4]
```

Then
`A + B = [4 2; 1 5]`

---

# 📌 11. Examples of Linear Transformations

### Scaling

```
T(x) = 3x
```

### Reflection (across x-axis)

```
[1  0
 0 -1]
```

### Rotation in ℝ²

```
Rθ = [cosθ  -sinθ
      sinθ   cosθ]
```

---

# 📌 12. Projections

Projection of vector `v` onto `u`:

```
projᵤ(v) = (u·v)/(u·u) * u
```

Projection matrix:

```
P = (u uᵀ) / (uᵀu)
```

### Example

Project `[3 4]ᵀ` onto `[1 0]ᵀ`:

Result = `[3 0]ᵀ`.

---

# 📌 13. Composition of Transformations

```
T₂(T₁(x)) = (A₂A₁)x
```

Matrix multiplication **is** composing transformations.

### Example

Rotate then scale:

```
A = scale(2)
B = rotation(90°)
```

Composite = `A B`.

---

# 📌 14. Properties of Matrix Multiplication

* Associative
* Distributive
* **Not commutative**

### Example

```
AB ≠ BA
```

for most matrices.

---

# 📌 15. Inverse Transformations

A function or matrix is invertible if:

```
T⁻¹(T(x)) = x
```

For matrices:

```
AA⁻¹ = A⁻¹A = I
```

---

# 📌 16. When Is a Matrix Invertible?

A square matrix is invertible iff:

* det(A) ≠ 0
* Rank = n
* Nullity = 0
* Columns are independent
* Transformation is 1-1 and onto

### Example

```
A = [1 2
     3 4] → det = -2 ≠ 0 → invertible
```

---

# 📌 17. Surjective (Onto) and Injective (One-to-One)

### Onto

Every `y` has some `x` such that `Ax = y`.

Condition:

```
Column space = ℝⁿ
```

### One-to-One

```
Ax = 0 ⇒ x = 0
```

Condition:

```
ker(A) = {0}
```

---

# 📌 18. Solving Ax = b: Structure of Solutions

General solution:

```
x = xₚ + xₙ
```

Where:

* `xₚ` = a particular solution
* `xₙ` = general null-space vector

### Example

Solve:

```
x + y = 2
2x + 2y = 4  (same equation)
```

Particular: `xₚ = [2 0]ᵀ`
Null space: `t[-1 1]`.

Solution:

```
x = [2 0]ᵀ + t[-1 1]ᵀ
```

---

# 📌 19. Matrix Condition for One-to-One

Equivalent conditions:

* Null space = `{0}`
* Pivot in every column
* Columns linearly independent
* Rank = number of columns

---

# 📌 20. Determinants

### Uses

* Invertibility
* Orientation
* Area/volume scaling
* Change of variables
* Geometric meaning of matrix

### Example

Rotation matrix:

```
det = 1
```

→ preserves area.

Reflection:

```
det = -1
```

→ area same but orientation flips.

---

# 📌 21. Computing Determinants

### 2×2

```
|a b|
|c d| = ad − bc
```

### 3×3 (Sarrus)

```
|a b c|
|d e f|
|g h i|

= aei + bfg + cdh − ceg − bdi − afh
```

---

# 📌 22. Determinants and Geometry

If `A` maps a square → parallelogram:

```
Area(new) = |det(A)| * Area(original)
```

### Example

```
A = [2 0
     0 3]
```

→ Area scaled by `2×3 = 6`.

---

# 📌 23. Transpose of a Matrix

Definition:

```
(Aᵀ)ᵢⱼ = Aⱼᵢ
```

Properties:

```
(Aᵀ)ᵀ = A
(AB)ᵀ = BᵀAᵀ
det(Aᵀ) = det(A)
```

---

# 📌 24. Row Space and Left Null Space

* **Row space** = span of rows
* **Null space** = solutions to `Ax = 0`
* **Left null space** = solutions to `Aᵀy = 0`

---

# 📌 25. Orthogonality Relationships

```
Row space ⟂ Null space
Column space ⟂ Left null space
```

### Example

If `Ax = 0`, then `rowᵢ · x = 0` → row vectors are orthogonal to null-space vectors.

---

# 📌 26. Rank of A and Aᵀ

```
rank(A) = rank(Aᵀ)
```

Both count number of pivots.

---

# 📌 27. When Is AᵀA Invertible?

```
AᵀA invertible ⇔ columns of A independent
```

Used heavily in machine learning (normal equations):

```
(AᵀA)x = Aᵀb
```

---

## ✅ Topics Covered

- [x] Function → transformation
- [x] Linear transformations
- [x] Matrix representation
- [x] Composition
- [x] Inverse matrices
- [x] Determinants
- [x] Kernels
- [x] Row/column space
- [x] Rank/Nullity
- [x] Orthogonality
- [x] AᵀA and ML usage

---

> This file is part of my AI/ML learning journey — documenting foundational linear algebra concepts before advancing to calculus, vector calculus, and machine learning.