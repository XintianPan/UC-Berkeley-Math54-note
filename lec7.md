[toc]

# Math 54 Lec7

## Recap

Linear transformations $T: \mathbb{R}^n \to \mathbb{R}^m\text{ (matrix $A$)}, S: \mathbb{R}^p \to \mathbb{R}^n\text{ (matrix $B$)}$

Then $T \circ S$ has matrix $A \cdot B$

## Transpose

Very important counterpart of any matrix $A$, denoted by $A^T$

This switches the rows and columns of $A$ (i.e. $i$-th row of $A$ becomes $i$-th column of $A^T$). If $A$ is $m \times n$, then $A^T$ is $n \times m$.

### properties

- $(A + B)^T = A^T + B^T$
- $(AB)^T = B^TA^T$

#### Proof of $(AB)^T = B^TA^T$

Consider the $ij$-th entry in $(AB)^T$. That is the $ji$-th entry in $AB$ which is the $j$-th row of $A$ times the $i$-th column in $B$.

Now consider the $ij$-entry in $B^TA^T$. That is the $i$-th row in $B^T$($i$-th column in $B$) times $j$-th column in $A^T$($j$-th column in $A$).

## Identity matrix

For $n \times n$ matrix, $I_n$ is the **identity matrix**, which has $1$s for all diagonal entries. $0$ for all non-diagonal entries.

==$I$ for short if context is clear.==

### Key property

For any $n \times n$ matrix $A$, we have $A \cdot I_n = I_n \cdot A = A$.

## Inverse (For square matrix)

For an $n \times n$ matrix $A$, the **"inverse"** of $A$(if it exists) is denoted $A^{-1}$ has the property that
$$
A\cdot A^{-1} = A^{-1}\cdot A = I_n
$$

### Left inverse of matrix equals to Right inverse of matrix

Say we find $B$ for which $BA = I_n$. Is $AB = I_n$ guaranteed?

Without assuming that say there is also some $C$ where $AC = I_n$

Then $BAC = BI_n \Rightarrow I_nC = B \Rightarrow C = B$

### Inverse is unique

Say we have $I_n = AB = AC$

### Terminology 

A square matrix is **invertible/nonsingular** if it has an inverse, otherwise **singular**.

$A = \begin{bmatrix}a & b \\ c & d\end{bmatrix}$, then the **determinant** of $A$ is $ad - bc$. And we have 
$$
A^{-1} = \frac{1}{ad - bc}\begin{bmatrix}d & -b \\ -c & a\end{bmatrix}
$$
Naturally requires $ad - bc \neq 0$

If $ad - bc = 0 \to \frac{a}{b} = \frac{c}{d}$

### Properties

- $(A^{-1})^{-1} = A$
- $(AB)^{-1} = B^{-1}A^{-1}$

