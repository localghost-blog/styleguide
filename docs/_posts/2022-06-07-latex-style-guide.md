---
title:  $\LaTeX$ Style Guide
categories: LaTeXguide
katex: true
---

# Source File Formatting

## Preamble

Todo.

# Language

This parts follows from [$\LaTeX$ Style Guide for EE 364B](https://web.stanford.edu/class/ee364b/latex_templates/template_notes.pdf) written by Stephen Boyd, Ernest K. Ryu and Neal Parikh.

## Write good english

Always write good English, “even” when the subject is mathematics. 
This includes correct grammar, word choice, punctuation, spelling, phrasing, and common sense. 
A classic on this topic, is Strunk and White[^SW07].

## Keep the reader in mind

Perhaps the most important principle of good writing is to keep the reader in mind: 
What do they know so far? 
What do they expect next and why?
Do they have sufficient motivation for stated results? 
As part of this, make sure you know what level of reader you are writing for and stay consistent with that level. 
If the reader is expected to know convex analysis, do not keep defining standard concepts like subgradients.

## Write to allow skipping over formulas

Many readers will first read through the paper ignoring or skipping all but the simplest formulas. 
Your sentences and overall paper should flow smoothly, and make sense, when all but the simplest formulas are replaced by “blah” or a similar placeholder. 
As a related point, do not simply display a list of formulas or equations in a row; tie the concepts together with a running commentary.

## Be precise with your language

The sentence 

> Let $x^*$ be the solution to the optimization problem.

implicitly asserts that the solution is unique. 

If the solution is not unique or need not be unique, write, 

> Let $x^*$ be a solution to the optimization problem. 

Similarly, do not refer to “solving” an expression, as this is meaningless. 
You can solve an equation or set of equations, evaluate an expression or function, or check that an equation or inequality holds.

## Use the editorial we when appropriate

The word “we” is often useful to avoid passive voice, which can sometimes be awkward, or the use of “I” or “one”, which should be avoided. 
However, be careful not to overuse “we”, as it can become a very bad habit.

> Often Bad: We can see that Theorem 1 implies Corollary 2.
>
> Good: Theorem 1 implies Corollary 2.

In general, use whatever phrasing makes the sentence cleaner and less clunky. 
To quote Strunk and White, “Omit needless words.”

## Punctuation in equations

An equation is part of a sentence, 
and you may need to include a comma or a period at the end of an equation as a result, whether or not you are using inline or display math style. 
For example:

> We next discuss how to solve the problem
>
> \\[ \text{minimize}\\ (1/2) \\|Ax - b\\|_2^2, \\]
>
> where $x \in \mathbb R^n$ is the optimization variable.

## Don’t start a sentence with a symbol

This hurts readability:

> Bad: $f$ is smooth.
>
> Good: The function $f$ is smooth.

> Bad: $x^n - a$ has $n$ distinct zeros.
>
> Good: The polynomial $x^n - a$ has $n$ distinct zeros.

Similarly, don’t start a sentence with a reference.

## Use words to separate symbols in different formulas

If it might confuse the reader visually or in the actual meaning of the sentence, 
use words to break apart formulas:

> Bad: The sequences $x_1, x_2, \dots$, $y_1, y_2, \dots$ are Cauchy.
>
> OK: The sequences $x_1, x_2, \dots$, and $y_1, y_2, \dots$, are Cauchy.
>
> Good: The sequence $(x_i)$ and $(y_i)$ are Cauchy.

> OK: The image of $S$ under $f$, $f(S) = \\{x \mid x \in S\\}$, is convex.
>
> Good: The image of $S$ under $f$, given by $f(S) = \\{x \mid x \in S\\}$, is convex.

Do not insert superfluous words if the meaning is clear.

> OK: Consider the function $f + g + h$, where 
$f : \mathbb R^n \to \mathbb R$, $g: \mathbb R^m \to \mathbb R$, $h: \mathbb R^p \to S^n$ are closed proper convex functions.
>
> Good: Consider the function $f + g + h$, where 
$f: \mathbb R^n \to \mathbb R$, $g: \mathbb R^m \to \mathbb R$, $h: \mathbb R^p \to S^n$ are closed proper convex.

# References

[^SW07]: Strunk Jr, W., & White, E. B. (2007). The Elements of Style Illustrated. Penguin.