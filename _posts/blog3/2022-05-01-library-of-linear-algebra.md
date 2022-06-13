---
layout: post
title: Library of Linear Algebra
date: 2022-05-01 09:05 +0530
last_modified_at: 2022-05-01 09:10:00 +0530
author: Baalateja Kataru
tags: [linear-algebra, matrices, vectors]
toc:  true
publishing: blog3
usemathjax: true
---

This is a repository of important/non-trivial proofs and derivations of ideas in Linear Algebra. This is a constantly evolving space as I'm continuously updating it.

# Post Details

- **Purpose**: notes and scribblings only
- **Difficulty**: mixed.
- **Prerequisites**: N/A

# Definitions

# Transpose

Include this: The definition of transpose is the operation of interchanging the rows and columns of a matrix. In other words, all the rows become the columns and all the columns become the rows. Thus, if the index $$ i $$ specified the $$i$$-th row and the index $$ j $$ specified the $$ j $$-th column, then after transpose, $$ i $$ specifies 

## Outer Product



## Matrix Multiplication

If $$ A $$ and $$ B $$ are

# Proofs

## Associativity for Matrix Multiplication

## Transpose of Matrix Product

Let $$ A $$ be an $$ (m \times n) $$ matrix.
Let $$ B $$ be an $$ (n \times p) $$ matrix.

We need to show that,

$$ (AB)^T = B^T A^T $$

We know the elements of $$ AB $$ are,

$$ (ab)_{ij} = \sum_{k = 1}^{n} a_{ik} b_{kj} $$

The definition of transpose is the operation of interchanging the rows and columns of a matrix. In other words, all the rows become the columns and all the columns become the rows. Thus, if the index $$ i $$ specified the $$i$$-th row and the index $$ j $$ specified the $$ j $$-th column, then after transpose, $$ i $$ specifies 

## Any Square Matrix can be written as the sum of a Symmetric and Skew-Symmetric Matrix

Let $$ A $$ be an $$ (m \times m) $$ matrix.

Our claim is,

$$ A = S + \bar{S} \tag{1} $$

Where,

$$
    \begin{align*}
        S^T &= S \\
        \bar{S}^T &= -\bar{S}
    \end{align*}
$$

Taking Transpose of both sides of $$ (1) $$

$$
    \begin{align*}
        A^T &= S^T + \bar{S}^T \\
        A^T &= S - \bar{S} \tag{2}
    \end{align*}
$$

Adding $$ (1) $$ and $$ (2) $$,

$$
    \begin{align*}
        A + A^T &= S + \bar{S} + S - \bar{S} \\
        A + A^T &= 2S \\
        S &= \frac{A + A^T}{2}
    \end{align*}
$$

Subtracting $$ (1) $$ and $$ (2) $$,

$$
    \begin{align*}
        A - A^T &= S + \bar{S} - S + \bar{S} \\
        A - A^T &= 2\bar{S} \\
        \bar{S} &= \frac{A - A^T}{2}
    \end{align*}
$$

Thus, the Symmetric and Skew-Symmetric parts can be obtained from the matrix A itself so $$ \forall \, A $$, we can construct a Symmetric and Skew-Symmetric part s.t.,

$$
    A = \frac{1}{2}(A + A^T) + \frac{1}{2}(A - A^T)
$$

Observe that,

$$
    \begin{align*}
        \left( \frac{A + A^T}{2} \right)^T &= \frac{A^T + A}{2} \\
        &= \frac{A + A^T}{2}
    \end{align*}
$$

Which is Symmetric as expected.

Similarly,

$$
    \begin{align*}
        \left( \frac{A - A^T}{2} \right)^T &= \frac{A^T - A}{2} \\
        &= -\frac{A - A^T}{2}
    \end{align*}
$$

Which is Skew-Symmetric as expected.



