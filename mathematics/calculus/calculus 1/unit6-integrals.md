# 📘 Calculus 1 – Unit 6: Integrals

*This file documents core concepts, strategies, and examples from Khan Academy’s Unit on Integrals.*  
🔗 Source: [Khan Academy – Integrals](https://www.khanacademy.org/math/calculus-1/cs1-integrals)

---

## 📌 Accumulations of Change – Introduction: Integrals

- If a quantity’s **rate of change** is given by \(f(x)\), then the **accumulated amount** from \(a\) to \(b\) is
  \[
  \int_a^b f(x)\,dx.
  \]
- **Interpretation:** Area under the curve \(f(x)\), above the \(x\)-axis (subtract below-axis parts).

**Example:**  
If water fills a tank at rate \(r(t)=5\) liters/minute, then over 10 min, the amount is  
\[
\int_0^{10} 5\,dt = 5 \cdot 10 = 50 \text{ liters}.
\]

---

## 📌 Approximation with Riemann Sums: Integrals

We approximate the definite integral by sums of rectangles:

\[
\sum_{i=1}^n f(x_i^*) \, \Delta x
\]

- **Left Riemann Sum:** use left endpoints \(x_i = a + (i-1)\Delta x\)  
- **Right Riemann Sum:** use right endpoints \(x_i = a + i \Delta x\)  
- **Midpoint Rule:** use midpoints of subintervals  

**Example:**  
\(\displaystyle \int_0^2 x\,dx\) via right Riemann sum with \(n=2\):  
\(\Delta x =1\), right points \(x=1,2\):  
Sum = \(x_1 + x_2 = 1 + 2 = 3\). Approx ≈ 3 (true value = 2).

---

## 📌 Summation Notation Review: Integrals

- \(\sum_{i=1}^n i = \frac{n(n+1)}{2}\)  
- \(\sum_{i=1}^n i^2 = \frac{n(n+1)(2n+1)}{6}\)  
- \(\sum_{i=1}^n c = nc\) (constant sum)  

Use these to simplify Riemann sums when \(f(x)\) is polynomial.

---

## 📌 Riemann Sums in Summation Notation: Integrals

Given interval \([a,b]\), subdivided into \(n\) parts:

\[
\Delta x = \frac{b-a}{n}
\]

- Right sum: \(\sum_{i=1}^n f\left(a + i\Delta x\right) \Delta x\)  
- Left sum: \(\sum_{i=0}^{n-1} f\left(a + i\Delta x\right) \Delta x\)

**Example:**  
\(\int_0^1 x^2 dx\) approximated by right sum, \(n=2\):  
\(\Delta x = 0.5\), points: \(x=0.5,1\):  
Sum = \((0.5^2 + 1^2)\cdot 0.5 = (0.25 + 1)\cdot0.5 = 0.625\).

---

## 📌 Defining Integrals with Riemann Sums: Integrals

\[
\int_a^b f(x)\,dx = \lim_{n\to\infty} \sum_{i=1}^n f(x_i^*)\,\Delta x
\]

This gives the rigorous definition of the definite integral, provided the limit exists.

---

## 📌 Fundamental Theorem of Calculus & Accumulation Functions: Integrals

- Define \(F(x) = \int_a^x f(t)\,dt\).  
- Then \(F'(x) = f(x)\) (if \(f\) is continuous).  

This links integration (accumulation) with differentiation.

**Example:**  
\[
F(x) = \int_0^x \sin t\,dt \implies F'(x) = \sin x.
\]

---

## 📌 Interpreting the Behavior of Accumulation Functions: Integrals

- If \(f(x) > 0\), \(F(x)\) is **increasing**.  
- If \(f(x) < 0\), \(F(x)\) is **decreasing**.  
- When \(f\) crosses zero, \(F\) reaches local extrema.  

**Example:** If \(f(t) = \cos t\), then \(F(x) = \int_0^x \cos t\,dt = \sin x\). \(f\) positive → \(F\) rising; \(f\) negative → \(F\) falling.

---

## 📌 Properties of Definite Integrals: Integrals

For continuous \(f\),

1. \(\displaystyle \int_a^b f(x)\,dx = -\int_b^a f(x)\,dx\)  
2. \(\displaystyle \int_a^a f(x)\,dx = 0\)  
3. **Additivity:** \(\displaystyle \int_a^b f(x)\,dx + \int_b^c f(x)\,dx = \int_a^c f(x)\,dx\)  
4. **Constant multiple:** \(\displaystyle \int_a^b c\,f(x)\,dx = c\int_a^b f(x)\,dx\)  
5. **Sum rule:** \(\displaystyle \int_a^b (f(x)+g(x))\,dx = \int_a^b f(x)\,dx + \int_a^b g(x)\,dx\)

---

## 📌 Fundamental Theorem of Calculus & Definite Integrals: Integrals

If \(F\) is any antiderivative of \(f\), then

\[
\int_a^b f(x)\,dx = F(b) - F(a).
\]

This is what allows evaluation without Riemann sums.

---

## 📌 Reverse Power Rule: Integrals

\[
\int x^n \, dx = \frac{x^{n+1}}{n+1} + C \quad (n\neq -1)
\]

**Example:** \(\int x^3 dx = \frac{x^4}{4} + C\).

---

## 📌 Indefinite Integrals of Common Functions: Integrals

| \(f(x)\) | \(\int f(x)\,dx\) |
|---|---|
| \(e^x\) | \(e^x + C\) |
| \(\sin x\) | \(-\cos x + C\) |
| \(\cos x\) | \(\sin x + C\) |
| \(\sec^2 x\) | \(\tan x + C\) |
| \(\csc^2 x\) | \(-\cot x + C\) |
| \(\sec x \tan x\) | \(\sec x + C\) |
| \(\csc x \cot x\) | \(-\csc x + C\) |
| \(1/x\) | \(\ln |x| + C\) |

---

## 📌 Definite Integrals of Common Functions: Integrals

Evaluate definite integrals using antiderivatives:

\[
\int_a^b e^x\,dx = e^b - e^a
\]

\[
\int_0^{\pi} \sin x\,dx = 2
\]

\[
\int_{1}^{e} \frac{1}{x} \,dx = 1
\]

---

## 📌 Integrating with \(u\)-Substitution: Integrals

- Choose \(u = g(x)\) so \(du = g'(x)dx\).  
- Replace integrand & \(dx\) in terms of \(u\).  
- Integrate in \(u\), then resubstitute.

**Example:**  
\(\int 2x e^{x^2}\,dx\). Let \(u = x^2\), \(du = 2x dx\). → \(\int e^u\,du = e^u + C = e^{x^2} + C.\)

---

## 📌 Integrating Using Long Division & Completing the Square: Integrals

- **Long division** helps when rational integrand has numerator degree ≥ denominator’s.  
- **Completing the square** is essential when denominator is quadratic and we want forms like \(\int \frac{1}{(x - h)^2 + a^2} dx\).  

**Examples:**

- \(\int \frac{x^2 + 3x + 2}{x+1} dx\) → divide, then integrate the quotient + remainder part.  
- \(\int \frac{1}{x^2 + 4x + 8} dx\) → write denominator as \((x+2)^2 + 4\), then use arctan formula.

---

## 📌 Integrating Using Trigonometric Identities: Integrals

Use trig identities to simplify integrals:

- **Power-reducing:** \(\sin^2 x = \frac{1-\cos(2x)}{2}\)  
- **Pythagorean identities:** \(\sec^2 x = 1 + \tan^2 x\)  
- **Double-angle / half-angle** for integrals like \(\int \sin^3 x dx\) etc.

**Example:**  
\(\int \sin^2 x\, dx = \int \frac{1 - \cos 2x}{2} dx = \frac{x}{2} - \frac{1}{4}\sin 2x + C.\)

---

If you like, I can send you this Markdown file (.md) as a downloadable file or in a code block you can copy to your notes. Would you like me to package it for you?
::contentReference[oaicite:0]{index=0}
