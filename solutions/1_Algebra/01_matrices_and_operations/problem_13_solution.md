
# Exercise 13: Fibonacci Numbers and Matrix Powers

## Given

$$
F=\begin{pmatrix}
1 & 1\\
1 & 0
\end{pmatrix}
$$

We need to calculate F², F³, F⁴, and F⁵,
compare the results with the Fibonacci sequence,
and explain how matrix multiplication represents
the Fibonacci recurrence.

## 1. Calculate F²

$$
F^2=F\cdot F
$$

$$
F^2=
\begin{pmatrix}
1 & 1\\
1 & 0
\end{pmatrix}
\begin{pmatrix}
1 & 1\\
1 & 0
\end{pmatrix}
$$

Multiplying:

$$
F^2=
\begin{pmatrix}
1(1)+1(1) & 1(1)+1(0)\\
1(1)+0(1) & 1(1)+0(0)
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
F^2=\begin{pmatrix}
2 & 1\\
1 & 1
\end{pmatrix}
}
$$

## 2. Calculate F³

$$
F^3=F^2\cdot F
$$

$$
F^3=
\begin{pmatrix}
2 & 1\\
1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1\\
1 & 0
\end{pmatrix}
$$

Multiplying:

$$
F^3=
\begin{pmatrix}
2(1)+1(1) & 2(1)+1(0)\\
1(1)+1(1) & 1(1)+1(0)
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
F^3=\begin{pmatrix}
3 & 2\\
2 & 1
\end{pmatrix}
}
$$

## 3. Calculate F⁴

$$
F^4=F^3\cdot F
$$

$$
F^4=
\begin{pmatrix}
3 & 2\\
2 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1\\
1 & 0
\end{pmatrix}
$$

Multiplying:

$$
F^4=
\begin{pmatrix}
3(1)+2(1) & 3(1)+2(0)\\
2(1)+1(1) & 2(1)+1(0)
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
F^4=\begin{pmatrix}
5 & 3\\
3 & 2
\end{pmatrix}
}
$$

## 4. Calculate F⁵

$$
F^5=F^4\cdot F
$$

$$
F^5=
\begin{pmatrix}
5 & 3\\
3 & 2
\end{pmatrix}
\begin{pmatrix}
1 & 1\\
1 & 0
\end{pmatrix}
$$

Multiplying:

$$
F^5=
\begin{pmatrix}
5(1)+3(1) & 5(1)+3(0)\\
3(1)+2(1) & 3(1)+2(0)
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
F^5=\begin{pmatrix}
8 & 5\\
5 & 3
\end{pmatrix}
}
$$

## 5. Compare with the Fibonacci Sequence

The Fibonacci sequence is:

$$
0,\ 1,\ 1,\ 2,\ 3,\ 5,\ 8,\ldots
$$

Each new term is the sum of the two
previous terms.

$$
f_{n+1}=f_n+f_{n-1}
$$

From our calculations:

$$
F^1=\begin{pmatrix}
1 & 1\\
1 & 0
\end{pmatrix}
$$

$$
F^2=\begin{pmatrix}
2 & 1\\
1 & 1
\end{pmatrix}
$$

$$
F^3=\begin{pmatrix}
3 & 2\\
2 & 1
\end{pmatrix}
$$

$$
F^4=\begin{pmatrix}
5 & 3\\
3 & 2
\end{pmatrix}
$$

$$
F^5=\begin{pmatrix}
8 & 5\\
5 & 3
\end{pmatrix}
$$

We observe that the entries of each matrix
are consecutive Fibonacci numbers.

The general relationship is:

$$
\boxed{
F^n=
\begin{pmatrix}
f_{n+1} & f_n\\
f_n & f_{n-1}
\end{pmatrix}
}
$$

where f₀ = 0, f₁ = 1, and each subsequent
term is the sum of the previous two terms.

## 6. Calculate F(a, b)

Let:

$$
x=\begin{pmatrix}
a\\
b
\end{pmatrix}
$$

Then:

$$
Fx=
\begin{pmatrix}
1 & 1\\
1 & 0
\end{pmatrix}
\begin{pmatrix}
a\\
b
\end{pmatrix}
$$

Multiplying:

$$
Fx=
\begin{pmatrix}
1(a)+1(b)\\
1(a)+0(b)
\end{pmatrix}
$$

**Answer:**

$$
\boxed{
F\begin{pmatrix}
a\\
b
\end{pmatrix}
=
\begin{pmatrix}
a+b\\
a
\end{pmatrix}
}
$$

## 7. Explain the Recurrence Step

Suppose a and b are two consecutive
Fibonacci numbers, with a being the newer term.

The Fibonacci recurrence is:

$$
f_{n+1}=f_n+f_{n-1}
$$

Let:

$$
a=f_n,\qquad b=f_{n-1}
$$

Then:

$$
F\begin{pmatrix}
f_n\\
f_{n-1}
\end{pmatrix}
=
\begin{pmatrix}
f_n+f_{n-1}\\
f_n
\end{pmatrix}
$$

Using the Fibonacci recurrence:

$$
\boxed{
F\begin{pmatrix}
f_n\\
f_{n-1}
\end{pmatrix}
=
\begin{pmatrix}
f_{n+1}\\
f_n
\end{pmatrix}
}
$$

This means:

1. The first entry becomes the sum of
   the two previous terms.

2. The second entry keeps the previous
   first entry.

3. The resulting vector contains the next
   pair of consecutive Fibonacci numbers.

For example:

$$
F\begin{pmatrix}
3\\
2
\end{pmatrix}
=
\begin{pmatrix}
5\\
3
\end{pmatrix}
$$

Applying F again:

$$
F\begin{pmatrix}
5\\
3
\end{pmatrix}
=
\begin{pmatrix}
8\\
5
\end{pmatrix}
$$

Thus, each multiplication by F performs
one Fibonacci recurrence step.

## Final Answers

$$
\boxed{
F^2=\begin{pmatrix}
2 & 1\\
1 & 1
\end{pmatrix}
}
$$

$$
\boxed{
F^3=\begin{pmatrix}
3 & 2\\
2 & 1
\end{pmatrix}
}
$$

$$
\boxed{
F^4=\begin{pmatrix}
5 & 3\\
3 & 2
\end{pmatrix}
}
$$

$$
\boxed{
F^5=\begin{pmatrix}
8 & 5\\
5 & 3
\end{pmatrix}
}
$$

**General Formula:**

$$
\boxed{
F^n=
\begin{pmatrix}
f_{n+1} & f_n\\
f_n & f_{n-1}
\end{pmatrix}
}
$$

**Matrix-Vector Multiplication:**

$$
\boxed{
F\begin{pmatrix}
a\\
b
\end{pmatrix}
=
\begin{pmatrix}
a+b\\
a
\end{pmatrix}
}
$$

## Conclusion

The powers of the matrix F contain consecutive
Fibonacci numbers.

Multiplying F by a vector containing two
consecutive Fibonacci terms generates the
next term by adding them and preserves
the newer term for the following step.

Therefore, matrix multiplication provides
a way to represent the Fibonacci recurrence.
