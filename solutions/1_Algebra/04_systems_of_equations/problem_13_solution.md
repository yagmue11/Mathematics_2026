### Exercise 13. Does Every Equation Add New Information?
Consider the system

$$
x_1+x_2=10,\qquad x_2+x_3=8,\qquad x_1-x_3=2.
$$

Solve it and check whether all three equations are independently necessary to describe the solution set. If one follows from the others, show this by calculation.

> **Why this exercise:** teaches how to recognize redundant equations within a system.

### Exercise 13. Solution

Subtracting the second equation from the first gives

$$
(x_1+x_2)-(x_2+x_3)=10-8,
$$

which simplifies to $x_1-x_3=2$. Thus the third equation follows from the first two, and those two equations alone describe the full solution set.

Taking $x_2=s$ as the free parameter, the first equation gives $x_1=10-s$ and the second gives $x_3=8-s$. Hence all solutions are

$$
(x_1,x_2,x_3)=(10-s,s,8-s), \qquad s\in\mathbb{R}.
$$