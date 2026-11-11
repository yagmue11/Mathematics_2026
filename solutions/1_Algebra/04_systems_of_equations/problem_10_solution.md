### Exercise 10. A Polynomial Through Three Points
Find a polynomial $p(x)=ax^2+bx+c$ whose graph passes through $(0,1)$, $(1,3)$, and $(2,9)$. Reduce the problem to a system of equations and check the result by substituting all three points.

### Solution

The conditions $p(0)=1$, $p(1)=3$, and $p(2)=9$ give the system

$$
\begin{cases}
c=1, \\
a+b+c=3, \\
4a+2b+c=9. \\
\end{cases}
$$

Substituting $c=1$ into the last two equations and dividing the last equation by $2$ gives

$$
\begin{cases}
a+b=2, \\
2a+b=4. \\
\end{cases}
$$

Subtracting the first equation from the second gives $a=2$. It follows that $b=0$, so the polynomial is

$$
p(x)=2x^2+1.
$$

Substitution verifies all three points.

$$
\begin{aligned}
p(0)&=2(0)^2+1=1, \\
p(1)&=2(1)^2+1=3, \\
p(2)&=2(2)^2+1=9.
\end{aligned}
$$