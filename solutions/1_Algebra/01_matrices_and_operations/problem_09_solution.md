### Exercise. Transformation Order

Let

$$S= \begin{pmatrix} 2 & 0 \\ 0 & 1 \\ \end{pmatrix},\qquad R= \begin{pmatrix} 0 & -1 \\ 1 & 0 \\ \end{pmatrix}.$$

The matrix $S$ describes nonuniform scaling, while $R$ describes a $90^\circ$ counterclockwise rotation.
For

$$x= \begin{pmatrix} 1 \\ 2 \\ \end{pmatrix}$$

compute $RSx$ and $SRx$. Compare the results and explain geometrically why the order of these transformations matters.

### Solution

**1. Computation of $RSx$**

First, apply the scaling matrix $S$ to the vector $x$:

$$Sx = \begin{pmatrix} 2 & 0 \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 \\ 2 \\ \end{pmatrix} = \begin{pmatrix} 2 \\ 2 \\ \end{pmatrix}$$

Next, apply the rotation matrix $R$ to the result $Sx$:

$$RSx = \begin{pmatrix} 0 & -1 \\ 1 & 0 \\ \end{pmatrix} \begin{pmatrix} 2 \\ 2 \\ \end{pmatrix} = \begin{pmatrix} -2 \\ 2 \\ \end{pmatrix}$$

**2. Computation of $SRx$**

First, apply the rotation matrix $R$ to the vector $x$:

$$Rx = \begin{pmatrix} 0 & -1 \\ 1 & 0 \\ \end{pmatrix} \begin{pmatrix} 1 \\ 2 \\ \end{pmatrix} = \begin{pmatrix} -2 \\ 1 \\ \end{pmatrix}$$

Next, apply the scaling matrix $S$ to the result $Rx$:

$$SRx = \begin{pmatrix} 2 & 0 \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} -2 \\ 1 \\ \end{pmatrix} = \begin{pmatrix} -4 \\ 1 \\ \end{pmatrix}$$

**3. Comparison and Geometric Explanation**

Comparing the results, the final vectors are different:

$$\begin{pmatrix} -2 \\ 2 \\ \end{pmatrix} \neq \begin{pmatrix} -4 \\ 1 \\ \end{pmatrix}$$

Thus, $RSx \neq SRx$. The order of transformations matters because the scaling is nonuniform. The matrix $S$ stretches vectors by a factor of $2$ exclusively along the horizontal axis (the x-axis), leaving the vertical component unchanged.

* In the product $RSx$, the vector is scaled first. Its original x-component is stretched, and the resulting longer vector is then rotated by $90^\circ$.
* In the product $SRx$, the vector is rotated first. The original y-component becomes the new horizontal component. When the nonuniform scaling is applied afterward, it stretches this newly rotated horizontal component instead.

Because the axis along which the stretching occurs remains fixed in space, rotating the vector before or after the stretch changes which geometric features of the vector get deformed.