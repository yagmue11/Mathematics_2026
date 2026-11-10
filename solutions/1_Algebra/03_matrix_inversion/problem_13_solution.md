### Exercise 13. Undoing a Composite Transformation

The matrices

$$S= \begin{pmatrix} 2 & 0 \\ 0 & 1 \\ \end{pmatrix},\qquad H= \begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix}$$

describe nonuniform scaling and shear. For $T=HS$, find $T^{-1}$ in two ways:

1. first compute $T$, then its inverse,
2. use $(HS)^{-1}=S^{-1}H^{-1}$.

Compare the results. Additionally compute $H^{-1}S^{-1}$ and verify that the incorrect order gives a different matrix. Explain the rule: “when undoing a composition of operations, we undo them from the end.”

### Solution

**1. Method 1: Compute $T$ first, then its inverse**

Calculate the composite matrix $T = HS$:

$$\begin{aligned} T &= \begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} 2 & 0 \\ 0 & 1 \\ \end{pmatrix} \\ &= \begin{pmatrix} 1(2) + 1(0) & 1(0) + 1(1) \\ 0(2) + 1(0) & 0(0) + 1(1) \\ \end{pmatrix} \\ &= \begin{pmatrix} 2 & 1 \\ 0 & 1 \\ \end{pmatrix} \end{aligned}$$

Next, compute the inverse $T^{-1}$. The determinant is $\det T = 2(1) - 1(0) = 2$. Using the explicit formula for a $2 \times 2$ inverse:

$$\begin{aligned} T^{-1} &= \frac{1}{2} \begin{pmatrix} 1 & -1 \\ 0 & 2 \\ \end{pmatrix} \\ &= \begin{pmatrix} \frac{1}{2} & -\frac{1}{2} \\ 0 & 1 \\ \end{pmatrix} \end{aligned}$$

**2. Method 2: Use $(HS)^{-1} = S^{-1}H^{-1}$**

Compute the individual inverses $S^{-1}$ and $H^{-1}$. The determinant of $S$ is $2$, and the determinant of $H$ is $1$.

$$S^{-1}= \begin{pmatrix} \frac{1}{2} & 0 \\ 0 & 1 \\ \end{pmatrix},\qquad H^{-1}= \begin{pmatrix} 1 & -1 \\ 0 & 1 \\ \end{pmatrix}$$

Multiply $S^{-1}$ and $H^{-1}$ in that specific order:

$$\begin{aligned} S^{-1}H^{-1} &= \begin{pmatrix} \frac{1}{2} & 0 \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & -1 \\ 0 & 1 \\ \end{pmatrix} \\ &= \begin{pmatrix} \frac{1}{2}(1) + 0(0) & \frac{1}{2}(-1) + 0(1) \\ 0(1) + 1(0) & 0(-1) + 1(1) \\ \end{pmatrix} \\ &= \begin{pmatrix} \frac{1}{2} & -\frac{1}{2} \\ 0 & 1 \\ \end{pmatrix} \end{aligned}$$

**3. Compare the results**

Both methods yield the exact same matrix:

$$T^{-1} = S^{-1}H^{-1} = \begin{pmatrix} \frac{1}{2} & -\frac{1}{2} \\ 0 & 1 \\ \end{pmatrix}$$

**4. Compute $H^{-1}S^{-1}$ and verify the incorrect order**

Multiply the inverses in the unreversed order:

$$\begin{aligned} H^{-1}S^{-1} &= \begin{pmatrix} 1 & -1 \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} \frac{1}{2} & 0 \\ 0 & 1 \\ \end{pmatrix} \\ &= \begin{pmatrix} 1\left(\frac{1}{2}\right) + (-1)(0) & 1(0) + (-1)(1) \\ 0\left(\frac{1}{2}\right) + 1(0) & 0(0) + 1(1) \\ \end{pmatrix} \\ &= \begin{pmatrix} \frac{1}{2} & -1 \\ 0 & 1 \\ \end{pmatrix} \end{aligned}$$

Comparing the matrices confirms that $H^{-1}S^{-1} \neq S^{-1}H^{-1}$. The incorrect order yields a completely different matrix.

**5. Explanation of the rule**

When a composite transformation $T = HS$ is applied to a vector $v$, the operations are evaluated from right to left as $H(Sv)$. Geometrically, the scaling $S$ happens first, followed by the shear $H$.

To successfully undo a sequence of transformations and return to the original state, one must reverse the operations in a last-in, first-out manner. The shear $H$ was applied last, so the reverse shear $H^{-1}$ must be applied first. The scaling $S$ was applied first, so the reverse scaling $S^{-1}$ must be applied last. Algebraically, applying $H^{-1}$ first and $S^{-1}$ second means left-multiplying the vector by $S^{-1}H^{-1}$. Attempting to undo the operations in their original forward order fails because it applies the reverse scaling to a geometry that is still skewed by the shear.