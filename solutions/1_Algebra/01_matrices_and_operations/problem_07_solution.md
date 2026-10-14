
## Given

$$
A=\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
$$

The identity matrix and zero matrix of size 2 × 2 are:

$$
I=\begin{pmatrix}
1 & 0\\
0 & 1
\end{pmatrix},
\qquad
0=\begin{pmatrix}
0 & 0\\
0 & 0
\end{pmatrix}
$$

## 1. Calculate AI

$$
AI=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
\begin{pmatrix}
1 & 0\\
0 & 1
\end{pmatrix}
$$

Multiplying:

$$
AI=
\begin{pmatrix}
2(1)+1(0) & 2(0)+1(1)\\
0(1)+2(0) & 0(0)+2(1)
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
AI=\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}=A
}
$$

## 2. Calculate IA

$$
IA=
\begin{pmatrix}
1 & 0\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
$$

Multiplying:

$$
IA=
\begin{pmatrix}
1(2)+0(0) & 1(1)+0(2)\\
0(2)+1(0) & 0(1)+1(2)
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
IA=\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}=A
}
$$

## 3. Calculate A + 0

$$
A+0=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
+
\begin{pmatrix}
0 & 0\\
0 & 0
\end{pmatrix}
$$

Adding corresponding elements:

$$
A+0=
\begin{pmatrix}
2+0 & 1+0\\
0+0 & 2+0
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
A+0=\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}=A
}
$$

## 4. Calculate A²

Matrix power A² means multiplying A by itself.

$$
A^2=A\cdot A
$$

$$
A^2=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
$$

Multiplying:

$$
A^2=
\begin{pmatrix}
2(2)+1(0) & 2(1)+1(2)\\
0(2)+2(0) & 0(1)+2(2)
\end{pmatrix}
$$

Simplifying:

$$
A^2=
\begin{pmatrix}
4 & 4\\
0 & 4
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
A^2=\begin{pmatrix}
4 & 4\\
0 & 4
\end{pmatrix}
}
$$

## 5. Calculate A³

Matrix power A³ means multiplying A² by A.

$$
A^3=A^2\cdot A
$$

$$
A^3=
\begin{pmatrix}
4 & 4\\
0 & 4
\end{pmatrix}
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
$$

Multiplying:

$$
A^3=
\begin{pmatrix}
4(2)+4(0) & 4(1)+4(2)\\
0(2)+4(0) & 0(1)+4(2)
\end{pmatrix}
$$

Simplifying:

$$
A^3=
\begin{pmatrix}
8 & 12\\
0 & 8
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
A^3=\begin{pmatrix}
8 & 12\\
0 & 8
\end{pmatrix}
}
$$

## 6. Explain the Roles of I and 0

### Identity Matrix (I)

The identity matrix acts as the multiplicative identity.

Multiplying any matrix by the identity matrix of
compatible size does not change the original matrix.

$$
\boxed{AI=IA=A}
$$

### Zero Matrix (0)

The zero matrix acts as the additive identity.

Adding a zero matrix of the same size to any matrix
does not change the original matrix.

$$
\boxed{A+0=A}
$$

## 7. Pattern in Successive Powers of A

From our calculations:

$$
A^1=\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
$$

$$
A^2=\begin{pmatrix}
4 & 4\\
0 & 4
\end{pmatrix}
$$

$$
A^3=\begin{pmatrix}
8 & 12\\
0 & 8
\end{pmatrix}
$$

We observe the following pattern:

1. The diagonal elements are powers of 2.

2. The bottom-left element always remains 0.

3. The top-right element follows the pattern:

$$
1,\quad 4,\quad 12,\quad 32,\ldots
$$

The general formula for the nth power is:

$$
\boxed{
A^n=
\begin{pmatrix}
2^n & n2^{n-1}\\
0 & 2^n
\end{pmatrix}
}
$$

For example, when n = 3:

$$
A^3=
\begin{pmatrix}
2^3 & 3(2^2)\\
0 & 2^3
\end{pmatrix}
=
\begin{pmatrix}
8 & 12\\
0 & 8
\end{pmatrix}
$$

This confirms the pattern.

## Final Answers

$$
\boxed{
AI=IA=A+0=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
}
$$

$$
\boxed{
A^2=
\begin{pmatrix}
4 & 4\\
0 & 4
\end{pmatrix}
}
$$

$$
\boxed{
A^3=
\begin{pmatrix}
8 & 12\\
0 & 8
\end{pmatrix}
}
$$

## Conclusion

The identity matrix I leaves a matrix unchanged
under multiplication, while the zero matrix
leaves a matrix unchanged under addition.

In successive powers of A, the diagonal elements
follow powers of 2, the bottom-left element
remains zero, and the top-right element follows
the formula n × 2^(n-1).
