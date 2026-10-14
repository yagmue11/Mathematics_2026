
# Exercise 15: Associativity of Matrix Multiplication

## Given

$$
A=\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix},
\quad
B=\begin{pmatrix}
1 & 0\\
2 & 1\\
-1 & 3
\end{pmatrix},
\quad
C=\begin{pmatrix}
2 & 1\\
0 & -1
\end{pmatrix}
$$

The matrix dimensions are:

$$
A_{2\times3},\quad B_{3\times2},\quad C_{2\times2}
$$

We need to calculate (AB)C and A(BC),
compare the results and the number of
intermediate operations, and explain associativity.

## 1. Calculate (AB)C

First, calculate AB.

$$
AB=
\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 0\\
2 & 1\\
-1 & 3
\end{pmatrix}
$$

Multiplying rows by columns:

$$
AB=
\begin{pmatrix}
1(1)+2(2)+0(-1) & 1(0)+2(1)+0(3)\\
0(1)+1(2)+1(-1) & 0(0)+1(1)+1(3)
\end{pmatrix}
$$

Simplifying:

$$
AB=
\begin{pmatrix}
5 & 2\\
1 & 4
\end{pmatrix}
$$

Now multiply AB by C.

$$
(AB)C=
\begin{pmatrix}
5 & 2\\
1 & 4
\end{pmatrix}
\begin{pmatrix}
2 & 1\\
0 & -1
\end{pmatrix}
$$

Multiplying:

$$
(AB)C=
\begin{pmatrix}
5(2)+2(0) & 5(1)+2(-1)\\
1(2)+4(0) & 1(1)+4(-1)
\end{pmatrix}
$$

Simplifying:

$$
(AB)C=
\begin{pmatrix}
10 & 3\\
2 & -3
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
(AB)C=
\begin{pmatrix}
10 & 3\\
2 & -3
\end{pmatrix}
}
$$

## 2. Calculate A(BC)

First, calculate BC.

$$
BC=
\begin{pmatrix}
1 & 0\\
2 & 1\\
-1 & 3
\end{pmatrix}
\begin{pmatrix}
2 & 1\\
0 & -1
\end{pmatrix}
$$

Multiplying rows by columns:

$$
BC=
\begin{pmatrix}
1(2)+0(0) & 1(1)+0(-1)\\
2(2)+1(0) & 2(1)+1(-1)\\
-1(2)+3(0) & -1(1)+3(-1)
\end{pmatrix}
$$

Simplifying:

$$
BC=
\begin{pmatrix}
2 & 1\\
4 & 1\\
-2 & -4
\end{pmatrix}
$$

Now multiply A by BC.

$$
A(BC)=
\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 1\\
4 & 1\\
-2 & -4
\end{pmatrix}
$$

Multiplying:

$$
A(BC)=
\begin{pmatrix}
1(2)+2(4)+0(-2) & 1(1)+2(1)+0(-4)\\
0(2)+1(4)+1(-2) & 0(1)+1(1)+1(-4)
\end{pmatrix}
$$

Simplifying:

$$
A(BC)=
\begin{pmatrix}
10 & 3\\
2 & -3
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
A(BC)=
\begin{pmatrix}
10 & 3\\
2 & -3
\end{pmatrix}
}
$$

## 3. Compare the Results

From Part 1:

$$
(AB)C=
\begin{pmatrix}
10 & 3\\
2 & -3
\end{pmatrix}
$$

From Part 2:

$$
A(BC)=
\begin{pmatrix}
10 & 3\\
2 & -3
\end{pmatrix}
$$

Since both matrices are equal:

$$
\boxed{(AB)C=A(BC)}
$$

Therefore, associativity is verified.

## 4. Compare the Number of Operations

We count the scalar multiplications
required for each matrix product.

For multiplying an m × n matrix by
an n × p matrix, the number of scalar
multiplications is:

$$
mnp
$$

### Method 1: (AB)C

First, calculate AB:

$$
(2\times3)(3\times2)
$$

Number of scalar multiplications:

$$
2\times3\times2=12
$$

Then calculate (AB)C:

$$
(2\times2)(2\times2)
$$

Number of scalar multiplications:

$$
2\times2\times2=8
$$

Total:

$$
\boxed{12+8=20}
$$

### Method 2: A(BC)

First, calculate BC:

$$
(3\times2)(2\times2)
$$

Number of scalar multiplications:

$$
3\times2\times2=12
$$

Then calculate A(BC):

$$
(2\times3)(3\times2)
$$

Number of scalar multiplications:

$$
2\times3\times2=12
$$

Total:

$$
\boxed{12+12=24}
$$

### Comparison

| Method | Scalar Multiplications |
|--------|------------------------|
| (AB)C | 20 |
| A(BC) | 24 |

Therefore, calculating (AB)C requires
4 fewer scalar multiplications than A(BC).

If scalar additions are also counted,
(AB)C requires 12 additions, while
A(BC) requires 14 additions.

Thus, (AB)C is computationally more
efficient for these matrices.

## 5. Explain Associativity

Associativity of matrix multiplication
means that the grouping of matrices
does not affect the final result,
provided the products are defined.

In general:

$$
\boxed{(AB)C=A(BC)}
$$

This means we can multiply A and B first,
then multiply the result by C.

Alternatively, we can multiply B and C
first, then multiply A by the result.

Both methods produce the same matrix.

However, the number of intermediate
arithmetic operations can be different.

Therefore, choosing a suitable grouping
can make matrix multiplication more efficient.

## Final Answers

**Part 1:**

$$
\boxed{
(AB)C=
\begin{pmatrix}
10 & 3\\
2 & -3
\end{pmatrix}
}
$$

**Part 2:**

$$
\boxed{
A(BC)=
\begin{pmatrix}
10 & 3\\
2 & -3
\end{pmatrix}
}
$$

**Part 3:**

$$
\boxed{(AB)C=A(BC)}
$$

**Number of scalar multiplications:**

$$
\boxed{
(AB)C:20,\qquad A(BC):24
}
$$

## Conclusion

Matrix multiplication is associative,
meaning that changing the grouping
of matrices does not change the result.

In this example, both (AB)C and A(BC)
produce the same 2 × 2 matrix.

However, (AB)C requires fewer scalar
multiplications, showing that the
grouping can affect computational efficiency
even though the final result is unchanged.
