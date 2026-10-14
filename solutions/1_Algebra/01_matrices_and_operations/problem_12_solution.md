
# Exercise 12: Matrix Powers and Mathematical Induction

## Given

$$
A=\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

We need to calculate A², A³, and A⁴, find a
general formula for Aⁿ, and prove it using
mathematical induction.

## 1. Calculate A²

$$
A^2=A\cdot A
$$

$$
A^2=
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

Multiplying:

$$
A^2=
\begin{pmatrix}
1(1)+1(0) & 1(1)+1(1)\\
0(1)+1(0) & 0(1)+1(1)
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
A^2=\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
}
$$

## 2. Calculate A³

$$
A^3=A^2\cdot A
$$

$$
A^3=
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

Multiplying:

$$
A^3=
\begin{pmatrix}
1(1)+2(0) & 1(1)+2(1)\\
0(1)+1(0) & 0(1)+1(1)
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
A^3=\begin{pmatrix}
1 & 3\\
0 & 1
\end{pmatrix}
}
$$

## 3. Calculate A⁴

$$
A^4=A^3\cdot A
$$

$$
A^4=
\begin{pmatrix}
1 & 3\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

Multiplying:

$$
A^4=
\begin{pmatrix}
1(1)+3(0) & 1(1)+3(1)\\
0(1)+1(0) & 0(1)+1(1)
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
A^4=\begin{pmatrix}
1 & 4\\
0 & 1
\end{pmatrix}
}
$$

## 4. Observe the Pattern

From our calculations:

$$
A^1=\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

$$
A^2=\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
$$

$$
A^3=\begin{pmatrix}
1 & 3\\
0 & 1
\end{pmatrix}
$$

$$
A^4=\begin{pmatrix}
1 & 4\\
0 & 1
\end{pmatrix}
$$

We observe that:

1. The diagonal elements always remain 1.
2. The bottom-left element always remains 0.
3. The top-right element equals the power n.

Therefore, we conjecture:

$$
\boxed{
A^n=\begin{pmatrix}
1 & n\\
0 & 1
\end{pmatrix}
}
$$

for every positive integer n.

## 5. Proof by Mathematical Induction

We will prove that:

$$
A^n=\begin{pmatrix}
1 & n\\
0 & 1
\end{pmatrix}
$$

for all positive integers n.

### Step 1: Base Case (n = 1)

For n = 1:

$$
A^1=\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

Using the proposed formula:

$$
\begin{pmatrix}
1 & n\\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

Both matrices are equal.

Therefore, the formula is true for n = 1.

### Step 2: Induction Hypothesis

Assume the formula is true for some
positive integer n.

That is, assume:

$$
A^n=\begin{pmatrix}
1 & n\\
0 & 1
\end{pmatrix}
$$

We must prove that the formula is also
true for n + 1.

In other words, we need to show:

$$
A^{n+1}=
\begin{pmatrix}
1 & n+1\\
0 & 1
\end{pmatrix}
$$

### Step 3: Induction Step

We know that:

$$
A^{n+1}=A^n\cdot A
$$

Using the induction hypothesis:

$$
A^{n+1}=
\begin{pmatrix}
1 & n\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

Multiply the matrices:

$$
A^{n+1}=
\begin{pmatrix}
1(1)+n(0) & 1(1)+n(1)\\
0(1)+1(0) & 0(1)+1(1)
\end{pmatrix}
$$

Simplifying:

$$
A^{n+1}=
\begin{pmatrix}
1 & 1+n\\
0 & 1
\end{pmatrix}
$$

Since 1 + n = n + 1:

$$
\boxed{
A^{n+1}=
\begin{pmatrix}
1 & n+1\\
0 & 1
\end{pmatrix}
}
$$

This is exactly the proposed formula
with n replaced by n + 1.

Therefore, if the formula is true for n,
it is also true for n + 1.

### Step 4: Induction Conclusion

We have shown that:

1. The formula is true for n = 1.
2. If the formula is true for n,
   then it is true for n + 1.

Therefore, by mathematical induction,
the formula holds for every positive integer n.

$$
\boxed{
A^n=\begin{pmatrix}
1 & n\\
0 & 1
\end{pmatrix}
}
$$

## Final Answers

$$
\boxed{
A^2=\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
}
$$

$$
\boxed{
A^3=\begin{pmatrix}
1 & 3\\
0 & 1
\end{pmatrix}
}
$$

$$
\boxed{
A^4=\begin{pmatrix}
1 & 4\\
0 & 1
\end{pmatrix}
}
$$

**General Formula:**

$$
\boxed{
A^n=\begin{pmatrix}
1 & n\\
0 & 1
\end{pmatrix},
\qquad n\geq1
}
$$

## Conclusion

The powers of A follow a simple pattern:
the diagonal elements remain 1, the
bottom-left element remains 0, and the
top-right element increases by 1 with
each multiplication.

By mathematical induction, we have proved
that the formula holds for every positive
integer n, not just the first few cases.
