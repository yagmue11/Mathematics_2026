### Exercise 3. Matrix Multiplication Dimensions

The matrix sizes are

$$A_{2\times3},\qquad B_{3\times4},\qquad C_{4\times2},\qquad D_{2\times2}.$$

For the products

$$AB,\ BA,\ BC,\ CB,\ AC,\ CA,\ AD,\ DA$$

determine whether they are defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition.

### Solution

The matrix product is defined if and only if the number of columns in the first matrix equals the number of rows in the second matrix. If a matrix of size $m \times n$ is multiplied by a matrix of size $n \times p$, the resulting matrix has size $m \times p$.

* **Product $AB$**
Defined. Matrix $A$ has $3$ columns and matrix $B$ has $3$ rows ($3 = 3$). The resulting matrix size is $2 \times 4$.
* **Product $BA$**
Undefined. Matrix $B$ has $4$ columns and matrix $A$ has $2$ rows ($4 \neq 2$).
* **Product $BC$**
Defined. Matrix $B$ has $4$ columns and matrix $C$ has $4$ rows ($4 = 4$). The resulting matrix size is $3 \times 2$.
* **Product $CB$**
Undefined. Matrix $C$ has $2$ columns and matrix $B$ has $3$ rows ($2 \neq 3$).
* **Product $AC$**
Undefined. Matrix $A$ has $3$ columns and matrix $C$ has $4$ rows ($3 \neq 4$).
* **Product $CA$**
Defined. Matrix $C$ has $2$ columns and matrix $A$ has $2$ rows ($2 = 2$). The resulting matrix size is $4 \times 3$.
* **Product $AD$**
Undefined. Matrix $A$ has $3$ columns and matrix $D$ has $2$ rows ($3 \neq 2$).
* **Product $DA$**
Defined. Matrix $D$ has $2$ columns and matrix $A$ has $2$ rows ($2 = 2$). The resulting matrix size is $2 \times 3$.