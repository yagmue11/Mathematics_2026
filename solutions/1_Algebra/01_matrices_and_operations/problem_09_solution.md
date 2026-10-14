

## Given

$$
S=\begin{pmatrix}
2 & 0\\
0 & 1
\end{pmatrix},
\qquad
R=\begin{pmatrix}
0 & -1\\
1 & 0
\end{pmatrix}
$$

And the vector:

$$
x=\begin{pmatrix}
1\\
2
\end{pmatrix}
$$

The matrix S represents nonuniform scaling, which
stretches the horizontal coordinate by a factor of 2
while leaving the vertical coordinate unchanged.

The matrix R represents a 90° counterclockwise rotation.

## 1. Calculate RSx

In matrix multiplication, transformations are
applied from right to left.

Therefore, RSx means first applying S to x,
then applying R to the result.

### Step 1: Calculate Sx

$$
Sx=
\begin{pmatrix}
2 & 0\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1\\
2
\end{pmatrix}
$$

Multiplying:

$$
Sx=
\begin{pmatrix}
2(1)+0(2)\\
0(1)+1(2)
\end{pmatrix}
$$

$$
Sx=\begin{pmatrix}
2\\
2
\end{pmatrix}
$$

### Step 2: Apply R to Sx

$$
RSx=
\begin{pmatrix}
0 & -1\\
1 & 0
\end{pmatrix}
\begin{pmatrix}
2\\
2
\end{pmatrix}
$$

Multiplying:

$$
RSx=
\begin{pmatrix}
0(2)+(-1)(2)\\
1(2)+0(2)
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
RSx=\begin{pmatrix}
-2\\
2
\end{pmatrix}
}
$$

## 2. Calculate SRx

SRx means first applying R to x,
then applying S to the result.

### Step 1: Calculate Rx

$$
Rx=
\begin{pmatrix}
0 & -1\\
1 & 0
\end{pmatrix}
\begin{pmatrix}
1\\
2
\end{pmatrix}
$$

Multiplying:

$$
Rx=
\begin{pmatrix}
0(1)+(-1)(2)\\
1(1)+0(2)
\end{pmatrix}
$$

$$
Rx=\begin{pmatrix}
-2\\
1
\end{pmatrix}
$$

### Step 2: Apply S to Rx

$$
SRx=
\begin{pmatrix}
2 & 0\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
-2\\
1
\end{pmatrix}
$$

Multiplying:

$$
SRx=
\begin{pmatrix}
2(-2)+0(1)\\
0(-2)+1(1)
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
SRx=\begin{pmatrix}
-4\\
1
\end{pmatrix}
}
$$

## 3. Compare the Results

From our calculations:

$$
RSx=\begin{pmatrix}
-2\\
2
\end{pmatrix}
$$

$$
SRx=\begin{pmatrix}
-4\\
1
\end{pmatrix}
$$

Since the resulting vectors are different:

$$
\boxed{RSx\neq SRx}
$$

Therefore, the order of transformations matters.

## 4. Geometric Explanation

### Applying RSx

First, S stretches the vector horizontally
by a factor of 2.

$$
(1,2)\xrightarrow{S}(2,2)
$$

Then, R rotates the resulting vector
90° counterclockwise.

$$
(2,2)\xrightarrow{R}(-2,2)
$$

Therefore:

$$
\boxed{RSx=(-2,2)}
$$

### Applying SRx

First, R rotates the original vector
90° counterclockwise.

$$
(1,2)\xrightarrow{R}(-2,1)
$$

Then, S stretches the rotated vector
horizontally by a factor of 2.

$$
(-2,1)\xrightarrow{S}(-4,1)
$$

Therefore:

$$
\boxed{SRx=(-4,1)}
$$

## 5. Why Does the Order Matter?

The scaling matrix S stretches vectors along
the horizontal axis.

When scaling is applied before rotation,
the stretched vector is rotated afterward.

When rotation is applied before scaling,
the vector changes direction first, and
then its new horizontal component is stretched.

Because scaling acts along a fixed coordinate
axis, changing the order produces different results.

This demonstrates that matrix transformations
are generally noncommutative.

$$
\boxed{RS\neq SR}
$$

## Final Answers

**Scaling first, then rotation:**

$$
\boxed{
RSx=\begin{pmatrix}
-2\\
2
\end{pmatrix}
}
$$

**Rotation first, then scaling:**

$$
\boxed{
SRx=\begin{pmatrix}
-4\\
1
\end{pmatrix}
}
$$

**Comparison:**

$$
\boxed{RSx\neq SRx}
$$

## Conclusion

The order of matrix transformations matters
because nonuniform scaling and rotation
generally do not commute.

Applying scaling before rotation produces
a different vector from applying rotation
before scaling.
