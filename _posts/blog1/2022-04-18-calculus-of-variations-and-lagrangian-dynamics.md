---
layout: post
title: A Crash Course into Calculus of Variations and Lagrangian Dynamics
date: 2022-04-18 23:18 +0800
last_modified_at: 2022-04-18 01:08:25 +0800
author: Baalateja Kataru
tags: [calculus-of-variations, lagrangian-dynamics, classical-mechanics, mechanics, analytical-mechanics]
toc:  true
publishing: blog1
usemathjax: true
---

The shortest distance between any two points in space is a line. But how do we know this?

Consider $$ L(q, \dot{q}) $$

The differential of the Lagrangian is,

$$
    dL = \frac{\partial L}{ \partial q} dq + \frac{\partial L}{\partial \dot{q}} d\dot{q}
$$

Define quantities $$ p, \dot{p} $$ such that, 

$$ 
  \begin{align*} 
    \frac{\partial L}{\partial q}  &= \dot{p} \\
    \frac{\partial L}{\partial \dot{q}} &= p
  \end{align*}
$$

Thus,

$$ dL = \dot{p} dq + p d\dot{q} $$

Now, we define a quantity $$ H $$ as,

$$ H = p\dot{q} - L $$

And observe that the differential of this quantity is,

$$
  \begin{align*}
    dH &= p d\dot{q} + \dot{q}dp - dL \\ 
    dH &= p d\dot{q} + \dot{q} dp - \dot{p} dq - p d\dot{q} \\
    dH &= \dot{q} dp - \dot{p} dq
  \end{align*}
$$

If the differential of this quantity $$H$$ is written in terms of the differentials $$dp, dq$$, then it must be that $$H$$ is a function of $$p$$ and $$q$$, i.e., $$H = H(p, q)$$.

Taking the differential of $$H = H(p, q)$$ now, we observe that,

$$
  dH = \frac{\partial H}{\partial p}dp + \frac{\partial H}{\partial q}dq
$$

Comparing this with the expression for the differential we obtained before,

$$
  \frac{\partial H}{\partial p}dp + \frac{\partial H}{\partial q}dq = \dot{q} dp - \dot{p} dq
$$

Which implies that,

$$
  \begin{align*}
    \frac{\partial H}{\partial p} &= \dot{q} \\
    \frac{\partial H}{\partial q} &= -\dot{p}
  \end{align*}
$$

These are Hamilton's Equations, equivalent to Lagrange's equations and Newton's Laws for mechanics, and the variable transform $$H = p\dot{q} - L$$ and the following steps are what's called the Legendre transform. 
