

## Given

$$
A=\begin{pmatrix}
1 & 2 & 3\\
4 & 5 & 6
\end{pmatrix},
\qquad
B=\begin{pmatrix}
1 & 0\\
2 & 1\\
-1 & 3
\end{pmatrix}
$$

## 1. Calculate A Transpose

The transpose of a matrix is obtained by
interchanging its rows and columns.

$$
A^T=
\begin{pmatrix}
1 & 4\\
2 & 5\\
3 & 6
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
A^T=
\begin{pmatrix}
1 & 4\\
2 & 5\\
3 & 6
\end{pmatrix}
}
$$

## 2. Calculate B Transpose

Interchange the rows and columns of B.

$$
B^T=
\begin{pmatrix}
1 & 2 & -1\\
0 & 1 & 3
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
B^T=
\begin{pmatrix}
1 & 2 & -1\\
0 & 1 & 3
\end{pmatrix}
}
$$

## 3. Calculate AB

$$
AB=
\begin{pmatrix}
1 & 2 & 3\\
4 & 5 & 6
\end{pmatrix}
\begin{pmatrix}
1 & 0\\
2 & 1\\
-1 & 3
\end{pmatrix}
$$

Multiply each row of A by each column of B.

$$
AB=
\begin{pmatrix}
1(1)+2(2)+3(-1) & 1(0)+2(1)+3(3)\\
4(1)+5(2)+6(-1) & 4(0)+5(1)+6(3)
\end{pmatrix}
$$

Simplifying:

$$
AB=
\begin{pmatrix}
1+4-3 & 0+2+9\\
4+10-6 & 0+5+18
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
AB=\begin{pmatrix}
2 & 11\\
8 & 23
\end{pmatrix}
}
$$

## 4. Calculate (AB) Transpose

We already know:

$$
AB=\begin{pmatrix}
2 & 11\\
8 & 23
\end{pmatrix}
$$

Interchange the rows and columns.

$$
\boxed{
(AB)^T=
\begin{pmatrix}
2 & 8\\
11 & 23
\end{pmatrix}
}
$$

## 5. Calculate B Transpose Times A Transpose

We have:

$$
B^T=
\begin{pmatrix}
1 & 2 & -1\\
0 & 1 & 3
\end{pmatrix}
$$

$$
A^T=
\begin{pmatrix}
1 & 4\\
2 & 5\\
3 & 6
\end{pmatrix}
$$

Now multiply:

$$
B^TA^T=
\begin{pmatrix}
1 & 2 & -1\\
0 & 1 & 3
\end{pmatrix}
\begin{pmatrix}
1 & 4\\
2 & 5\\
3 & 6
\end{pmatrix}
$$

$$
B^TA^T=
\begin{pmatrix}
1(1)+2(2)+(-1)(3) & 1(4)+2(5)+(-1)(6)\\
0(1)+1(2)+3(3) & 0(4)+1(5)+3(6)
\end{pmatrix}
$$

Simplifying:

$$
B^TA^T=
\begin{pmatrix}
1+4-3 & 4+10-6\\
0+2+9 & 0+5+18
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
B^TA^T=
\begin{pmatrix}
2 & 8\\
11 & 23
\end{pmatrix}
}
$$

## 6. Verify (AB)^T = B^TA^T

From our calculations:

$$
(AB)^T=
\begin{pmatrix}
2 & 8\\
11 & 23
\end{pmatrix}
$$

And:

$$
B^TA^T=
\begin{pmatrix}
2 & 8\\
11 & 23
\end{pmatrix}
$$

Since both matrices are equal:

$$
\boxed{(AB)^T=B^TA^T}
$$

Therefore, the property is verified.

## Final Answers

**Transpose of A:**

$$
\boxed{
A^T=\begin{pmatrix}
1 & 4\\
2 & 5\\
3 & 6
\end{pmatrix}
}
$$

**Transpose of B:**

$$
\boxed{
B^T=\begin{pmatrix}
1 & 2 & -1\\
0 & 1 & 3
\end{pmatrix}
}
$$

**Matrix multiplication AB:**

$$
\boxed{
AB=\begin{pmatrix}
2 & 11\\
8 & 23
\end{pmatrix}
}
$$

**Verification:**

$$
\boxed{
(AB)^T=B^TA^T=
\begin{pmatrix}
2 & 8\\
11 & 23
\end{pmatrix}
}
$$

## Conclusion

The transpose of a product of two matrices
is equal to the product of their transposes
in reverse order.

$$
\boxed{(AB)^T=B^TA^T}
$$

This property has been verified using the
given matrices A and B.
