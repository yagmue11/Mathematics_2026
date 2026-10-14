
# Exercise 5: Matrix-Vector Multiplication

## Given

$$
A=\begin{pmatrix}
2 & -1\\
1 & 3
\end{pmatrix},
\qquad
x=\begin{pmatrix}
4\\
2
\end{pmatrix}
$$

## 1. Calculate Ax

Multiply each row of matrix A by the column vector x.

$$
Ax=
\begin{pmatrix}
2 & -1\\
1 & 3
\end{pmatrix}
\begin{pmatrix}
4\\
2
\end{pmatrix}
$$

$$
Ax=
\begin{pmatrix}
(2)(4)+(-1)(2)\\
(1)(4)+(3)(2)
\end{pmatrix}
$$

Simplifying:

$$
Ax=
\begin{pmatrix}
8-2\\
4+6
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
Ax=\begin{pmatrix}
6\\
10
\end{pmatrix}
}
$$

## 2. Express Ax as a Linear Combination

The columns of matrix A are:

$$
a_1=\begin{pmatrix}
2\\
1
\end{pmatrix},
\qquad
a_2=\begin{pmatrix}
-1\\
3
\end{pmatrix}
$$

The coefficients come from vector x:

$$
x=\begin{pmatrix}
4\\
2
\end{pmatrix}
$$

Therefore, Ax can be written as:

$$
Ax=4a_1+2a_2
$$

Substituting the column vectors:

$$
Ax=
4\begin{pmatrix}
2\\
1
\end{pmatrix}
+
2\begin{pmatrix}
-1\\
3
\end{pmatrix}
$$

Multiply each vector by its coefficient:

$$
Ax=
\begin{pmatrix}
8\\
4
\end{pmatrix}
+
\begin{pmatrix}
-2\\
6
\end{pmatrix}
$$

Adding the vectors:

$$
\boxed{
Ax=\begin{pmatrix}
6\\
10
\end{pmatrix}
}
$$

## Final Answers

**Matrix-vector multiplication:**

$$
\boxed{
Ax=\begin{pmatrix}
6\\
10
\end{pmatrix}
}
$$

**Linear combination of the columns of A:**

$$
\boxed{
Ax=
4\begin{pmatrix}
2\\
1
\end{pmatrix}
+
2\begin{pmatrix}
-1\\
3
\end{pmatrix}
=
\begin{pmatrix}
6\\
10
\end{pmatrix}
}
$$

## Conclusion

Matrix-vector multiplication can be expressed as a
linear combination of the columns of the matrix.

The coefficients are the corresponding entries
of the vector x.

In this example, the coefficients are 4 and 2.
