
# Exercise 11: Commutativity of Matrix Multiplication

## Given

$$
A=\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix},
\qquad
B=\begin{pmatrix}
a & b\\
c & d
\end{pmatrix}
$$

We need to find the conditions on a, b, c, and d
such that:

$$
AB=BA
$$

## 1. Calculate AB

$$
AB=
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
a & b\\
c & d
\end{pmatrix}
$$

Multiplying rows by columns:

$$
AB=
\begin{pmatrix}
1(a)+1(c) & 1(b)+1(d)\\
0(a)+1(c) & 0(b)+1(d)
\end{pmatrix}
$$

Simplifying:

$$
\boxed{
AB=\begin{pmatrix}
a+c & b+d\\
c & d
\end{pmatrix}
}
$$

## 2. Calculate BA

$$
BA=
\begin{pmatrix}
a & b\\
c & d
\end{pmatrix}
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

Multiplying rows by columns:

$$
BA=
\begin{pmatrix}
a(1)+b(0) & a(1)+b(1)\\
c(1)+d(0) & c(1)+d(1)
\end{pmatrix}
$$

Simplifying:

$$
\boxed{
BA=\begin{pmatrix}
a & a+b\\
c & c+d
\end{pmatrix}
}
$$

## 3. Apply the Condition AB = BA

For the matrices to commute, we require:

$$
AB=BA
$$

Therefore:

$$
\begin{pmatrix}
a+c & b+d\\
c & d
\end{pmatrix}
=
\begin{pmatrix}
a & a+b\\
c & c+d
\end{pmatrix}
$$

Equating corresponding elements gives:

$$
a+c=a
$$

$$
b+d=a+b
$$

$$
c=c
$$

$$
d=c+d
$$

## 4. Solve the Equations

From the first equation:

$$
a+c=a
$$

Subtracting a from both sides:

$$
\boxed{c=0}
$$

From the second equation:

$$
b+d=a+b
$$

Subtracting b from both sides:

$$
\boxed{d=a}
$$

The third equation:

$$
c=c
$$

is always true.

The fourth equation:

$$
d=c+d
$$

also gives:

$$
c=0
$$

Therefore, the required conditions are:

$$
\boxed{c=0,\qquad d=a}
$$

There are no restrictions on a and b.

## 5. General Form of B

We started with:

$$
B=\begin{pmatrix}
a & b\\
c & d
\end{pmatrix}
$$

Substituting the conditions:

$$
c=0,\qquad d=a
$$

We obtain:

$$
\boxed{
B=\begin{pmatrix}
a & b\\
0 & a
\end{pmatrix}
}
$$

where a and b can be any real numbers.

## 6. Verification

Let:

$$
B=\begin{pmatrix}
a & b\\
0 & a
\end{pmatrix}
$$

Calculate AB:

$$
AB=
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
a & b\\
0 & a
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
a & a+b\\
0 & a
\end{pmatrix}
$$

Now calculate BA:

$$
BA=
\begin{pmatrix}
a & b\\
0 & a
\end{pmatrix}
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

$$
BA=
\begin{pmatrix}
a & a+b\\
0 & a
\end{pmatrix}
$$

Since both products are equal:

$$
\boxed{AB=BA}
$$

Thus, the conditions are verified.

## Final Answers

**Conditions:**

$$
\boxed{c=0,\qquad d=a}
$$

**General form of B:**

$$
\boxed{
B=\begin{pmatrix}
a & b\\
0 & a
\end{pmatrix},
\qquad a,b\in\mathbb{R}
}
$$

## Conclusion

The matrices A and B commute if and only if
c = 0 and d = a.

Therefore, all matrices B that commute with A
are upper triangular matrices with equal
diagonal entries.

The values of a and b can be any real numbers.
