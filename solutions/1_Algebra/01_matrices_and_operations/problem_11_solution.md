### Solution

**1. Computation of $AB$ and $BA$**

First, compute the product $AB$:

$$AB = \begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} a & b \\ c & d \\ \end{pmatrix} = \begin{pmatrix} a+c & b+d \\ c & d \\ \end{pmatrix}$$

Next, compute the product $BA$:

$$BA = \begin{pmatrix} a & b \\ c & d \\ \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix} = \begin{pmatrix} a & a+b \\ c & c+d \\ \end{pmatrix}$$

**2. Equating the Products**

For the matrices to commute, the condition $AB = BA$ must hold. Equating the corresponding entries of the two resulting matrices yields a system of equations:

$$\begin{cases} a+c = a, \\ b+d = a+b, \\ c = c, \\ d = c+d. \end{cases}$$

Analyzing the equations step by step:

* From the first equation, subtracting $a$ from both sides gives $c = 0$.
* From the second equation, subtracting $b$ from both sides gives $d = a$.
* The third equation is a trivial identity.
* The fourth equation, $d = c+d$, simplifies to $c = 0$, which confirms the first result.

Thus, the conditions are exactly $c = 0$ and $d = a$. There are no restrictions on the parameters $a$ and $b$, meaning they can be any real numbers.

**3. General Form of Matrix $B$**

By applying the derived conditions $c = 0$ and $d = a$ to the original matrix $B$, we find that the general form of all matrices that commute with $A$ is:

$$B = \begin{pmatrix} a & b \\ 0 & a \\ \end{pmatrix}$$