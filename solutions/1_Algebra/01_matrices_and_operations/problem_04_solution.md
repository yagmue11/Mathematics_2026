
## Given

$$
A=\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix},
\qquad
B=\begin{pmatrix}
2 & 0\\
3 & 1
\end{pmatrix}
$$

Both matrices are 2 × 2, so AB and BA are defined.

## 1. Calculate AB

$$
AB=
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0\\
3 & 1
\end{pmatrix}
$$

Multiply each row of A by each column of B.

$$
AB=
\begin{pmatrix}
(1)(2)+(2)(3) & (1)(0)+(2)(1)\\
(0)(2)+(1)(3) & (0)(0)+(1)(1)
\end{pmatrix}
$$

Simplifying:

$$
AB=
\begin{pmatrix}
2+6 & 0+2\\
0+3 & 0+1
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
AB=\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
}
$$

## 2. Calculate BA

$$
BA=
\begin{pmatrix}
2 & 0\\
3 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
$$

Multiply each row of B by each column of A.

$$
BA=
\begin{pmatrix}
(2)(1)+(0)(0) & (2)(2)+(0)(1)\\
(3)(1)+(1)(0) & (3)(2)+(1)(1)
\end{pmatrix}
$$

Simplifying:

$$
BA=
\begin{pmatrix}
2+0 & 4+0\\
3+0 & 6+1
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
BA=\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
}
$$

## 3. Is AB = BA?

We obtained:

$$
AB=\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
$$

$$
BA=\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
$$

Since the corresponding elements are different:

$$
\boxed{AB\neq BA}
$$

Therefore, AB is not equal to BA.

## 4. Explain Noncommutativity

Matrix multiplication is generally noncommutative.

This means that changing the order of multiplication
can change the result.

In general:

$$
\boxed{AB\neq BA}
$$

In this example, multiplying A by B gives a different
matrix from multiplying B by A.

Therefore, this example demonstrates that matrix
multiplication is not commutative.

## Final Answers

$$
\boxed{
AB=\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
}
$$

$$
\boxed{
BA=\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
}
$$

$$
\boxed{AB\neq BA}
$$

**Conclusion:** Matrix multiplication is generally
noncommutative because changing the order of the
matrices can produce different results.
