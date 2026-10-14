
# Exercise 10: Matrix Multiplication by Columns

## Given

$$
A=\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix},
\qquad
B=\begin{pmatrix}
1 & 2\\
-1 & 0\\
3 & 1
\end{pmatrix}
$$

The columns of B are:

$$
b_1=\begin{pmatrix}
1\\
-1\\
3
\end{pmatrix},
\qquad
b_2=\begin{pmatrix}
2\\
0\\
1
\end{pmatrix}
$$

## 1. Calculate Ab₁ and Ab₂

### Calculate Ab₁

$$
Ab_1=
\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1\\
-1\\
3
\end{pmatrix}
$$

Multiply each row of A by the vector b₁.

$$
Ab_1=
\begin{pmatrix}
1(1)+2(-1)+0(3)\\
0(1)+1(-1)+1(3)
\end{pmatrix}
$$

Simplifying:

$$
Ab_1=
\begin{pmatrix}
1-2+0\\
0-1+3
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
Ab_1=\begin{pmatrix}
-1\\
2
\end{pmatrix}
}
$$

### Calculate Ab₂

$$
Ab_2=
\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
2\\
0\\
1
\end{pmatrix}
$$

Multiply each row of A by the vector b₂.

$$
Ab_2=
\begin{pmatrix}
1(2)+2(0)+0(1)\\
0(2)+1(0)+1(1)
\end{pmatrix}
$$

Simplifying:

$$
Ab_2=
\begin{pmatrix}
2+0+0\\
0+0+1
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
Ab_2=\begin{pmatrix}
2\\
1
\end{pmatrix}
}
$$

## 2. Calculate AB

$$
AB=
\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 2\\
-1 & 0\\
3 & 1
\end{pmatrix}
$$

Since A is 2 × 3 and B is 3 × 2,
the resulting matrix will be 2 × 2.

Multiply rows of A by columns of B.

$$
AB=
\begin{pmatrix}
1(1)+2(-1)+0(3) & 1(2)+2(0)+0(1)\\
0(1)+1(-1)+1(3) & 0(2)+1(0)+1(1)
\end{pmatrix}
$$

Simplifying:

$$
AB=
\begin{pmatrix}
1-2+0 & 2+0+0\\
0-1+3 & 0+0+1
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
AB=\begin{pmatrix}
-1 & 2\\
2 & 1
\end{pmatrix}
}
$$

## 3. Compare the Results

From Part 1:

$$
Ab_1=\begin{pmatrix}
-1\\
2
\end{pmatrix}
$$

$$
Ab_2=\begin{pmatrix}
2\\
1
\end{pmatrix}
$$

From Part 2:

$$
AB=\begin{pmatrix}
-1 & 2\\
2 & 1
\end{pmatrix}
$$

We observe that the first column of AB is Ab₁,
and the second column of AB is Ab₂.

Therefore:

$$
\boxed{
AB=\begin{pmatrix}
Ab_1 & Ab_2
\end{pmatrix}
}
$$

## 4. Explanation

Matrix multiplication is performed by multiplying
each row of the first matrix by each column
of the second matrix.

When A multiplies B, each column of B is
multiplied separately by A.

Since B consists of the columns b₁ and b₂:

$$
B=\begin{pmatrix}
b_1 & b_2
\end{pmatrix}
$$

It follows that:

$$
AB=A\begin{pmatrix}
b_1 & b_2
\end{pmatrix}
$$

Therefore:

$$
\boxed{
AB=\begin{pmatrix}
Ab_1 & Ab_2
\end{pmatrix}
}
$$

This property holds for any matrices A and B
whose dimensions are compatible for multiplication.

## Final Answers

**Part 1:**

$$
\boxed{
Ab_1=\begin{pmatrix}
-1\\
2
\end{pmatrix},
\qquad
Ab_2=\begin{pmatrix}
2\\
1
\end{pmatrix}
}
$$

**Part 2:**

$$
\boxed{
AB=\begin{pmatrix}
-1 & 2\\
2 & 1
\end{pmatrix}
}
$$

**Part 3:**

$$
\boxed{
AB=\begin{pmatrix}
Ab_1 & Ab_2
\end{pmatrix}
}
$$

## Conclusion

The columns of AB are exactly the vectors
Ab₁ and Ab₂ because matrix multiplication
acts on each column of B separately.

Thus, multiplying A by B is equivalent to
multiplying A by each column of B and placing
the resulting vectors side by side.
