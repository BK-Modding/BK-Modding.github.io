---
layout: post
title: Covariant Formulation of Classical Electrodynamics using Relativity and Tensor Calculus
date: 2022-06-13 21:58 +0530
last_modified_at: 2022-06-13 21:58:00 +0530
author: Baalateja Kataru
tags: [covariant-physics, electromagnetism, relativity, tensors]
toc:  true
publishing: blog1
usemathjax: true
---

We attempt to formulate Maxwell's Equations and Classical Electrodynamics in a manner such that they are invariant under the Lorentz transformations of relativity theory.

# Post Details

- **Purpose**: Notes, will be made into a full blog post later.
- **Difficulty**: Advanced.
- **Prerequisites**: Classical Electromagnetism, Special Relativity and Relativistic Mechanics, Tensor Calculus.

# Introduction

<!--Fluff missing here, 
1. Talk about Oersted's goal to unify electric and magnetic fields -->

<!-- Maxwell's equations are a set of four equations that describe in a compact manner the interactions between the electric and magnetic fields and their sources. Einstein's theory of special relativity  -->

Relativity theory was a logical outcome of Classical Electromagnetic theory in the early 1900s so it's not surprising that Maxwell's equations find an elegant form in the language of relativity and tensor calculus associated with it.

# Convention

In this blog post, we will follow the natural units convention and set $$ c = 1 $$, thereby treating mass and energy as the same quantity.

Maxwell's equations predict that,

$$
  c = \frac{1}{\sqrt{\mu_0 \nu_0}}
$$

So according to our convention,

$$
  \begin{align*}
    1 &= \frac{1}{\sqrt{\mu_0, \nu_0}} \\
    \therefore \boxed{\mu_0 &= \frac{1}{\nu_0}}
  \end{align*}
$$