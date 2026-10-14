## Given

$$
A_{2\times3},\quad B_{3\times4},\quad
C_{4\times2},\quad D_{2\times2}
$$

## Rule

Matrix multiplication is defined when the number of columns
of the first matrix equals the number of rows of the second.

$$
(m\times n)(n\times p)=(m\times p)
$$

The inner dimensions must match, and the outer dimensions
determine the size of the resulting matrix.

## 1. AB

$$
AB=(2\times3)(3\times4)
$$

Since 3 = 3, multiplication is defined.

$$
\boxed{AB: 2\times4}
$$

## 2. BA

$$
BA=(3\times4)(2\times3)
$$

Since 4 ≠ 2, multiplication is not defined.

## 3. BC

$$
BC=(3\times4)(4\times2)
$$

Since 4 = 4, multiplication is defined.

$$
\boxed{BC: 3\times2}
$$

## 4. CB

$$
CB=(4\times2)(3\times4)
$$

Since 2 ≠ 3, multiplication is not defined.

## 5. AC

$$
AC=(2\times3)(4\times2)
$$

Since 3 ≠ 4, multiplication is not defined.

## 6. CA

$$
CA=(4\times2)(2\times3)
$$

Since 2 = 2, multiplication is defined.

$$
\boxed{CA: 4\times3}
$$

## 7. AD

$$
AD=(2\times3)(2\times2)
$$

Since 3 ≠ 2, multiplication is not defined.

## 8. DA

$$
DA=(2\times2)(2\times3)
$$

Since 2 = 2, multiplication is defined.

$$
\boxed{DA: 2\times3}
$$

## Final Answers

| Product | Defined? | Result Size |
|---------|----------|-------------|
| AB | Yes | 2 × 4 |
| BA | No | — |
| BC | Yes | 3 × 2 |
| CB | No | — |
| AC | No | — |
| CA | Yes | 4 × 3 |
| AD | No | — |
| DA | Yes | 2 × 3 |

## Conclusion

Matrix multiplication is possible only when the number
of columns in the first matrix equals the number of rows
in the second matrix.

The size of the result is determined by the outer dimensions.
