### Exercise 8. Inverse of a Transformation

The matrix

$$S= \begin{pmatrix} 2 & 0 \\ 0 & \frac{1}{2} \\ \end{pmatrix}$$

describes a scaling of the plane. Find $S^{-1}$ and explain geometrically what the inverse transformation does. Check the action of the pair $S,S^{-1}$ on one simple vector.

### Solution

**1. Find the inverse matrix $S^{-1}$**

The determinant of the diagonal matrix $S$ is $\det S = 2 \cdot \frac{1}{2} = 1$. The inverse of an invertible diagonal matrix is obtained by taking the reciprocal of each main diagonal entry:

$$S^{-1}= \begin{pmatrix} \frac{1}{2} & 0 \\ 0 & 2 \\ \end{pmatrix}$$

**2. Explain the geometric effect of the inverse**

The original matrix $S$ scales the plane by a factor of $2$ in the horizontal direction ($x$-axis) and by a factor of $\frac{1}{2}$ in the vertical direction ($y$-axis). The inverse matrix $S^{-1}$ precisely reverses this action by scaling the plane by a factor of $\frac{1}{2}$ in the horizontal direction and by a factor of $2$ in the vertical direction, returning any transformed geometry to its original state.

**3. Check the action on a simple vector**

Choose the vector $v = \begin{pmatrix} 1 \\ 2 \end{pmatrix}$. First, apply the transformation $S$ to $v$:

$$\begin{aligned} Sv &= \begin{pmatrix} 2 & 0 \\ 0 & \frac{1}{2} \\ \end{pmatrix} \begin{pmatrix} 1 \\ 2 \\ \end{pmatrix} \\ &= \begin{pmatrix} 2(1) + 0(2) \\ 0(1) + \frac{1}{2}(2) \\ \end{pmatrix} \\ &= \begin{pmatrix} 2 \\ 1 \\ \end{pmatrix} \end{aligned}$$

Next, apply the inverse transformation $S^{-1}$ to the resulting vector $Sv$:

$$\begin{aligned} S^{-1}(Sv) &= \begin{pmatrix} \frac{1}{2} & 0 \\ 0 & 2 \\ \end{pmatrix} \begin{pmatrix} 2 \\ 1 \\ \end{pmatrix} \\ &= \begin{pmatrix} \frac{1}{2}(2) + 0(1) \\ 0(2) + 2(1) \\ \end{pmatrix} \\ &= \begin{pmatrix} 1 \\ 2 \\ \end{pmatrix} \end{aligned}$$

Because $S^{-1}(Sv) = v$, the inverse transformation successfully reverses the scaling operation on the vector.