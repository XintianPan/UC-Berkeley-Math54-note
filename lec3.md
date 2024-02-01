# Vectors

With any collection of vectors: $\{v_1, v_2, \dots, v_n\}$, consider a linear combination of these vectors: $c_1v_1 + c_2v_2 + \dots + c_nv_n$ where each $c_i \in \mathbb{R}$.

Do these create the "full space"? If not, then what?

Say you have $n$ vectors in $\mathbb{R}^m$. Consider the matrix $A$, $m \times n$, whose columns are those $n$ vectors. Can these vectors have a linear combination $b$, for some $b$ in $\mathbb{R}^m$?

That boils down to: is the system
$$
A\mathbf{x} = \mathbf{b}
$$
consistent or not? 

For $\{v_1, v_2, \dots, v_n\}$, the set of linear combinations of the $v_i$s are the **span** of the set.

$A\mathbf{x}$'s meaning:
$$
\begin{aligned}
A & = & \begin{bmatrix}
 a_{11} & a_{12} & \dots & a_{1n} \\
 a_{21} & a_{22} & \dots  & \dots \\
 \vdots & \vdots  & \ddots  & \vdots \\
 a_{m1} & \dots  & \dots & a_{mn}
 \end{bmatrix}
\end{aligned}
$$

## Four equivalent statements:

1. $\forall b \in \mathbb{R}^m$, $A\mathbf{x} = \mathbf{b}$ has a solution
2. Each $b \in \mathbb{R}^m$ is a linear combinations of columns of $A$
3. Columns of $A$ span $\mathbb{R}^m$
4. $A$ has a pivot position in every row

If it doesn't span $\mathbb{R}^m$, how do we find/express the span, i.e. find which $b$ for which $A\mathbf{x} = \mathbf{b}$ is possible.

## Homogeneous System

$$
A\mathbf{x} = \mathbf{0}
$$

Put $A$ in row echelon form to check the solution set.