[toc]

# Math 54 Lec6

## Linear Transformation

### one-to-one

$T: \mathbb{R}^n \to \mathbb{R}^m$ linear transformation with associated matrix $A$. This is one-to-one if and only if $A\mathbf{x} = \mathbf{0}$ has only the trivial solution.

Which means this is one-to-one exactly when the columns of $A$ are linearly independent.

### onto

This is onto exactly when the columns of $A$ span $\mathbb{R}^m$. (i.e. $A\mathbf{x} = \mathbf{b}$ has solution for $\forall \mathbf{b} \in \mathbb{R}^m$) 

### composition of linear transformations

$S:\mathbb{R}^p \to \mathbb{R}^n,T:\mathbb{R}^n \to \mathbb{R}^m$ are linear transformations. Then $T \circ S:\mathbb{R}^p \to \mathbb{R}^m$ is linear transformation as well.

$S \circ T$ might not be defined (need $p = m$)

#### Proof :

$$
\begin{aligned}
T \circ S(c\mu + d\nu) & = T[S(c\mu + d\nu)] \\
& = T[c\cdot S(\mu) + d\cdot S(\nu)] \\
& = c \cdot [T\circ S](\mu) + d \cdot [T \circ S](\nu) \\
& = c \cdot (T\circ S)(\mu) + d \cdot (T\circ S)(\nu) \\
&\Rightarrow  T \circ S\text{ is a linear transformation}
\end{aligned}
$$

## Matrix Multiplication

### terminology

Say
$$
\begin{aligned}
A & = [a_{ij}]_{1 \leqslant i \leqslant m, 1 \leqslant j \leqslant n} \\
& = \begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n} \\
a_{21} & {a_22} & \dots  & a_{2n}\\
\vdots & \vdots & \ddots & \vdots\\
a_{m1} & \dots & \dots & a_{mn}
\end{bmatrix}
\end{aligned}
$$
$a_{11}, a_{22}, \dots a_{ii}, \dots$ are the diagonal entries.

When $A$ is a ==square matrix==, a **diagonal matrix** is any matrix where any non-diagonal entry is $0$.

$A + B$ only defined if $A$ and $B$ are same size.

$A \cdot B$ only defined if # of **columns** of $A$ is same as # of **row** in $B$.

 

### Computation of $AB$