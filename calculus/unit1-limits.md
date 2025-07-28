
# 📘 Calculus 1 – Unit 1: Limits and Continuity

*This file documents concepts and strategies I learned from Khan Academy's Unit 1 of Calculus 1: Limits and Continuity.*

🔗 Source: [Khan Academy – Limits and Continuity](https://www.khanacademy.org/math/calculus-1/cs1-limits-and-continuity)

---

## 📌 What is a Limit?

A **limit** is the value that a function `f(x)` approaches as `x` approaches some value `c`:

`lim(x → c) f(x) = L`

**Example:**  
`f(x) = (x - 1)/(x - 1)`  
- At `x = 1`, this becomes `0/0`, which is undefined.  
- But using the **limit** `lim(x → 1) f(x)`, we analyze values of `x` approaching 1 from both sides.

---

## 🔍 Left-Hand and Right-Hand Limits

A limit exists **only if** both one-sided limits exist and are equal:  

`lim(x → a⁻) f(x) = lim(x → a⁺) f(x) ⇒ lim(x → a) f(x) exists`

---

## 🧮 Limit Properties

If `lim(x → a) f(x) = L` and `lim(x → a) g(x) = M`, then:  
- `lim(x → a) [f + g](x) = L + M`  
- `lim(x → a) [f ⋅ g](x) = L ⋅ M`  
- `lim(x → a) [f/g](x) = L/M`, if `M ≠ 0`

---

## 🔁 Limits of Composite Functions

`lim(x → a) f(g(x)) = f(lim(x → a) g(x))`  
> When `f` is continuous at `lim g(x)`

---

## 🧠 Strategies to Find Limits

1. **Try direct substitution**:  
   - If `f(a) = b/0`, suspect a vertical asymptote.  
   - If `f(a) = b`, you're done!  

2. **Indeterminate form `0/0`**: Try:  
   - Factoring  
   - Rationalizing (conjugates)  
   - Trig identities  
   - Algebraic simplification  

---

## ✂️ Squeeze Theorem

Used when a function is trapped between two others:  

If `f(x) ≤ g(x) ≤ h(x)`, and both outer limits equal `L`, then:  
`lim(x → a) g(x) = L`

---

## 📈 Piecewise Functions

A piecewise function may have a limit `L` at `x = c`, but the **function value** `f(c) ≠ L`.  
This causes a **removable discontinuity**.

---

## 🧩 Discontinuities

Types of discontinuity at `x = c`:  
- **Removable**: limit exists, but `f(c)` is undefined or different  
- **Jump**: left and right-hand limits are not equal  
- **Infinite**: function approaches `∞` or `-∞`  

---

## 🔄 Continuity

### Continuity at a point `c`:  
A function `f(x)` is continuous at `c` if:  
1. `f(c)` is defined  
2. `lim(x → c) f(x)` exists  
3. `lim(x → c) f(x) = f(c)`  

### Continuity over an interval:  
If a function is continuous at **every point** in the interval.

---

## 🔧 Removing Discontinuity (Example)

Given:  
`f(x) = (x^2 - 9)/(x - 3)`  
`= ((x - 3)(x + 3))/(x - 3)`  
`= x + 3` (when `x ≠ 3`)  

- The function has a **removable discontinuity** at `x = 3`  
- Define `f(3) = 6` to make it continuous

---

## 🔭 Infinite Limits & Limits at Infinity

### Infinite Limit:  
`lim(x → a) f(x) = ∞`  
⇒ Vertical asymptote at `x = a`

### Limit at Infinity:  
`lim(x → ∞) (1/x) = 0`  
⇒ Horizontal asymptote at `y = 0`

---

## 📏 Delta-Epsilon Definition

For a formal proof:  
`lim(x → c) f(x) = L`  
⇔ For every `ε > 0`, there exists `δ > 0` such that  
`0 < |x - c| < δ ⇒ |f(x) - L| < ε`

---

## 📍 Intermediate Value Theorem

If `f` is continuous on `[a, b]` and `N` is between `f(a)` and `f(b)`,  
then there exists `c ∈ [a, b]` such that:  
`f(c) = N`

---

## 🧠 Visual Summary

- **Limits from a graph**: Observe behavior as `x → a⁻` and `x → a⁺`  
- **Continuity**: No jumps, breaks, or holes  
- **Discontinuity types**: Visual cues help identify them quickly  
- **Asymptotes**: Look for division by 0 or end behavior

---

## ✅ Completed Topics from Khan Academy

- [x] Estimating limits  
- [x] One-sided limits  
- [x] Infinite limits  
- [x] Limits at infinity  
- [x] Formal definition with epsilon-delta  
- [x] Continuity  
- [x] Intermediate value theorem  
- [x] Discontinuities and fixing them

---

## 📚 Reference

Khan Academy: [Unit 1 – Limits and Continuity](https://www.khanacademy.org/math/calculus-1/cs1-limits-and-continuity)

---

> This file is part of my AI/ML journey repo documenting foundational math skills before diving into machine learning and AI model building.
