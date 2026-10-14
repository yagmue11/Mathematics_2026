
# Exercise 14: Rotation Matrices and Angle Addition

## Given

The rotation matrix through an angle θ is:

$$
R(\theta)=
\begin{pmatrix}
\cos\theta & -\sin\theta\\
\sin\theta & \cos\theta
\end{pmatrix}
$$

We need to compute R(α)R(β) and prove that:

$$
R(\alpha)R(\beta)=R(\alpha+\beta)
$$

## 1. Write the Rotation Matrices

For angle α:

$$
R(\alpha)=
\begin{pmatrix}
\cos\alpha & -\sin\alpha\\
\sin\alpha & \cos\alpha
\end{pmatrix}
$$

For angle β:

$$
R(\beta)=
\begin{pmatrix}
\cos\beta & -\sin\beta\\
\sin\beta & \cos\beta
\end{pmatrix}
$$

## 2. Calculate R(α)R(β)

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha & -\sin\alpha\\
\sin\alpha & \cos\alpha
\end{pmatrix}
\begin{pmatrix}
\cos\beta & -\sin\beta\\
\sin\beta & \cos\beta
\end{pmatrix}
$$

Multiply each row of the first matrix
by each column of the second matrix.

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta &
-\cos\alpha\sin\beta-\sin\alpha\cos\beta\\
\sin\alpha\cos\beta+\cos\alpha\sin\beta &
-\sin\alpha\sin\beta+\cos\alpha\cos\beta
\end{pmatrix}
$$

## 3. Apply the Angle-Sum Formulas

Recall the trigonometric identities:

**Cosine angle-sum formula:**

$$
\cos(\alpha+\beta)
=
\cos\alpha\cos\beta-\sin\alpha\sin\beta
$$

**Sine angle-sum formula:**

$$
\sin(\alpha+\beta)
=
\sin\alpha\cos\beta+\cos\alpha\sin\beta
$$

Using these identities, we simplify
each entry of the matrix.

Top-left entry:

$$
\cos\alpha\cos\beta-\sin\alpha\sin\beta
=
\cos(\alpha+\beta)
$$

Top-right entry:

$$
-\cos\alpha\sin\beta-\sin\alpha\cos\beta
=
-\sin(\alpha+\beta)
$$

Bottom-left entry:

$$
\sin\alpha\cos\beta+\cos\alpha\sin\beta
=
\sin(\alpha+\beta)
$$

Bottom-right entry:

$$
-\sin\alpha\sin\beta+\cos\alpha\cos\beta
=
\cos(\alpha+\beta)
$$

Therefore:

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta)\\
\sin(\alpha+\beta) & \cos(\alpha+\beta)
\end{pmatrix}
$$

## 4. Verify the Identity

By definition:

$$
R(\alpha+\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta)\\
\sin(\alpha+\beta) & \cos(\alpha+\beta)
\end{pmatrix}
$$

Comparing both matrices, we see that
all corresponding entries are equal.

Hence:

$$
\boxed{
R(\alpha)R(\beta)=R(\alpha+\beta)
}
$$

Therefore, the identity is proved.

## 5. Geometric Explanation

A rotation matrix rotates a vector
counterclockwise by the given angle
around the origin when the angle is positive.

When two rotation matrices are multiplied,
the rotations are applied successively.

In the product:

$$
R(\alpha)R(\beta)
$$

The rotation by β is applied first,
followed by the rotation by α.

The total rotation angle is:

$$
\alpha+\beta
$$

For example, rotating a vector by 30°
and then by 60° produces the same result
as rotating it once by 90°.

$$
30^\circ+60^\circ=90^\circ
$$

Thus:

$$
R(30^\circ)R(60^\circ)=R(90^\circ)
$$

This shows that successive rotations
around the same origin are equivalent
to a single rotation by the sum of
their angles.

## 6. Additional Observation

Since angle addition is commutative:

$$
\alpha+\beta=\beta+\alpha
$$

We also have:

$$
R(\alpha)R(\beta)
=
R(\beta)R(\alpha)
$$

Therefore, two-dimensional rotation
matrices commute with each other.

However, general matrix multiplication
is not necessarily commutative.

## Final Answer

$$
\boxed{
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta)\\
\sin(\alpha+\beta) & \cos(\alpha+\beta)
\end{pmatrix}
}
$$

Therefore:

$$
\boxed{
R(\alpha)R(\beta)=R(\alpha+\beta)
}
$$

## Conclusion

The product of two rotation matrices
represents a single rotation through
the sum of their angles.

Geometrically, rotating a vector by
angle β and then by angle α is
equivalent to rotating it once by
angle α + β.

This proves the rotation composition
property.
