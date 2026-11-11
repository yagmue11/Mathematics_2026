### Exercise 12. Homogeneous System
Solve

$$
\begin{cases}
x+2y-z=0, \\
2x+4y-2z=0, \\
x-y+2z=0.
\end{cases}
$$

Give all solutions in parametric form and explain why $(0,0,0)$ always satisfies a homogeneous system.

### Exercise 12. Solution

The second equation is twice the first. Subtracting the first equation from the third reduces the system to

$$
\begin{cases}
x+2y-z=0, \\
-3y+3z=0. \\
\end{cases}
$$

The second equation gives $z=y$. Substituting into the first gives $x=-y$. Taking $y=s$ as the free parameter gives all solutions:

$$
(x,y,z)=(-s,s,s), \qquad s\in\mathbb{R}.
$$

In a homogeneous linear system, each equation has a linear combination of the unknowns on the left and zero on the right. Setting every unknown to zero makes each term vanish, so $(0,0,0)$ always satisfies the system. Here it corresponds to $s=0$.