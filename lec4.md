[toc]

# Math 54 Lec4

## homogenous system

$$
A\mathbf{x} = \mathbf{0}
$$

Just look at $A$ is sufficient.

## non-homohenous system

$$
A\mathbf{x} = \mathbf{b}
$$

Need to look at augmented matrix in this case.

**General: **one particular solution + general solution to homogeneous conterpart.
$$
A\mathbf{x}_1 = \mathbf{b}, A\mathbf{x}_2 = \mathbf{b} \Rightarrow A(\mathbf{x}_1 - \mathbf{x}_2) = \mathbf{0}
$$

## Span

$A$ is an $m \times n$ matrix. $A$ can be viewed as $n$ vectors in $\mathbb{R}^m$

A set of vectors $\{\mathbf{v}_1, \mathbf{v}_2, \dots, \mathbf{v}_n\}$ is called **linearly independent**, if the equation $c_1\mathbf{v}_1 + c_2\mathbf{v}_2 + \dots + c_n\mathbf{v}_n = \mathbf{0}$ has no nontrivial solution (i.e. not all $c_i =  0$). i.e. if this has only the trivial solution.

**linearly dependent** if $c_1\mathbf{v}_1 + c_2\mathbf{v}_2 + \dots + c_n\mathbf{v}_n = \mathbf{0}$ does have a nontrivial solution.

### How to tell whether indep. or dep.

Take 
$$
A = \begin{bmatrix}\mathbf{v}_1 & \mathbf{v}_2 & \dots & \mathbf{v}_n \end{bmatrix}
$$
Does $A\mathbf{x} = \mathbf{0}$ have a nonotrivial solution.

Say we have $n$ vectors in $\mathbb{R}^m$, if $n > m$, then this set of vectors is **always linearly dependent**.

 