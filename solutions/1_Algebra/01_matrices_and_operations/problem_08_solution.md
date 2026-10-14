## Given

$$
A=\begin{pmatrix}
1 & 2 & -1\\
2 & 4 & 1\\
-1 & 1 & 3
\end{pmatrix}
$$

We perform the three row operations in the given order.

## 1. First Row Operation

$$
R_2\leftarrow R_2-2R_1
$$

Subtract twice the first row from the second row.

$$
R_2=(2,4,1)-2(1,2,-1)
$$

$$
R_2=(2-2,\ 4-4,\ 1+2)
$$

$$
R_2=(0,0,3)
$$

The resulting matrix is:

$$
\boxed{
A_1=\begin{pmatrix}
1 & 2 & -1\\
0 & 0 & 3\\
-1 & 1 & 3
\end{pmatrix}
}
$$

## 2. Second Row Operation

$$
R_3\leftarrow R_3+R_1
$$

Add the first row to the third row.

$$
R_3=(-1,1,3)+(1,2,-1)
$$

$$
R_3=(-1+1,\ 1+2,\ 3-1)
$$

$$
R_3=(0,3,2)
$$

The resulting matrix is:

$$
\boxed{
A_2=\begin{pmatrix}
1 & 2 & -1\\
0 & 0 & 3\\
0 & 3 & 2
\end{pmatrix}
}
$$

## 3. Third Row Operation

Interchange the second and third rows.

$$
R_2\leftrightarrow R_3
$$

Before interchange:

$$
A_2=\begin{pmatrix}
1 & 2 & -1\\
0 & 0 & 3\\
0 & 3 & 2
\end{pmatrix}
$$

After interchange:

$$
\boxed{
A_3=\begin{pmatrix}
1 & 2 & -1\\
0 & 3 & 2\\
0 & 0 & 3
\end{pmatrix}
}
$$

## 4. Reverse of Each Row Operation

### Reverse of Operation 1

Original operation:

$$
R_2\leftarrow R_2-2R_1
$$

To reverse it, add twice the first row
to the second row.

$$
\boxed{R_2\leftarrow R_2+2R_1}
$$

### Reverse of Operation 2

Original operation:

$$
R_3\leftarrow R_3+R_1
$$

To reverse it, subtract the first row
from the third row.

$$
\boxed{R_3\leftarrow R_3-R_1}
$$

### Reverse of Operation 3

Original operation:

$$
R_2\leftrightarrow R_3
$$

To reverse it, interchange the same two
rows again.

$$
\boxed{R_2\leftrightarrow R_3}
$$

## Final Answers

**After Step 1:**

$$
\boxed{
A_1=\begin{pmatrix}
1 & 2 & -1\\
0 & 0 & 3\\
-1 & 1 & 3
\end{pmatrix}
}
$$

**After Step 2:**

$$
\boxed{
A_2=\begin{pmatrix}
1 & 2 & -1\\
0 & 0 & 3\\
0 & 3 & 2
\end{pmatrix}
}
$$

**After Step 3:**

$$
\boxed{
A_3=\begin{pmatrix}
1 & 2 & -1\\
0 & 3 & 2\\
0 & 0 & 3
\end{pmatrix}
}
$$

## Summary of Reverse Operations

| Step | Original Operation | Reverse Operation |
|------|--------------------|-------------------|
| 1 | R₂ ← R₂ − 2R₁ | R₂ ← R₂ + 2R₁ |
| 2 | R₃ ← R₃ + R₁ | R₃ ← R₃ − R₁ |
| 3 | R₂ ↔ R₃ | R₂ ↔ R₃ |

## Conclusion

Elementary row operations are reversible.

- Adding a multiple of one row can be reversed
  by subtracting the same multiple.
- Subtracting a multiple of one row can be reversed
  by adding the same multiple.
- Interchanging two rows can be reversed
  by interchanging them again.

To recover the original matrix from the final matrix,
apply the inverse operations in reverse order:
first undo Step 3, then Step 2, and finally Step 1.
