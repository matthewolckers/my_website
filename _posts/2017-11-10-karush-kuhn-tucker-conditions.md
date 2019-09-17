---
layout: post
title:  "How to remember the Karush-Kuhn-Tucker first order conditions"
date:   2017-11-10
tags:
---
I teach the maths refresher and microeconomics tutorial for the [PSME program](https://www.univ-paris1.fr/diplomes/psme/). Students need to maximize utility functions or profit functions and minimize expenditure functions or cost functions---but subject to constraints. I have trouble remembering the signs and direction of inequalities in the Karush-Kuhn-Tucker first order conditions. This blog post proposes a method to remember the first order conditions that should suffice for all the problems my students will tackle.

*Put a ceiling on max and a floor on min. Constraints are negative (because we would rather be free). And Lambda always does the opposite.*

### Maximize
Let's start with maximization.

Max $f(x,y)$ subject to $g(x,y) \leq 0, x \geq 0, y \geq0 $.

$$
L(x,y,\lambda) = f(x,y) - \lambda (g(x,y))
$$

The first order conditions are:

$$
\begin{align*}
\frac{\partial L}{\partial x} \leq 0 & & x \geq 0 & & x \frac{\partial L}{\partial x} = 0 \\
\frac{\partial L}{\partial y} \leq 0 & & y \geq 0 & & y \frac{\partial L}{\partial y} = 0 \\
\frac{\partial L}{\partial \lambda} \geq 0 & & \lambda \geq 0 & & \lambda \frac{\partial L}{\partial y} = 0 \\
\end{align*}
$$

Four points to remember:
  - Since we are maximizing, I wrote the constraint $g(x,y) \leq 0$ as a ceiling (with a less than or equal inequality).
  - $\frac{\partial L}{\partial x}$ and $\frac{\partial L}{\partial y}$  is less than or equal to zero (which is the same inequality as the ceiling).
  - $\frac{\partial L}{\partial \lambda}$ has the opposite sign inequality to $\frac{\partial L}{\partial x}$ and $\frac{\partial L}{\partial y}$
  - $\lambda \geq 0$

### Minimize
Now for the case I always get mixed up... MINIMIZATION!

Min $f(x,y)$ subject to $g(x,y) \geq 0 , x \geq 0, y \geq0 $.

$$
L(x,y,\lambda) = f(x,y) - \lambda (g(x,y))
$$

The first order conditions are:

$$
\begin{align*}
\frac{\partial L}{\partial x} \geq 0 & & x \geq 0 & & x \frac{\partial L}{\partial x} = 0 \\
\frac{\partial L}{\partial y} \geq 0 & & y \geq 0 & & y \frac{\partial L}{\partial y} = 0 \\
\frac{\partial L}{\partial \lambda} \leq 0 & & \lambda \geq 0 & & \lambda \frac{\partial L}{\partial y} = 0 \\
\end{align*}
$$

Five points to remember:
  - The Langrangian stays the same with the constraint entering as a negative.
  - Since we are minimizing, I wrote the constraint $g(x,y) \geq 0$ as a floor (with a greater than or equal to inequality).
  - $\frac{\partial L}{\partial x}$ and $\frac{\partial L}{\partial y}$  is greater than or equal to zero (which is the same inequality as the floor).
  - Again, $\frac{\partial L}{\partial \lambda}$ has the opposite sign inequality to $\frac{\partial L}{\partial x}$ and $\frac{\partial L}{\partial y}$
  - And again, $\lambda \geq 0$

### How do I remember this?

*Put a ceiling on max and a floor on min. Constraints are negative (because we would rather be free). And Lambda always does the opposite.*

### More details

If you would like more details, read chapter 13 of [Chiang and Wainwright](https://books.google.fr/books/about/Fundamental_Methods_of_Mathematical_Econ.html?id=QWOeQgAACAAJ).
